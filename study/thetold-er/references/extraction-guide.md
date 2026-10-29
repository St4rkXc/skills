# Extraction Guide

This document provides instructions for extracting text from various input formats (PDF, PPT, DOCX, MD, TXT) to prepare for note generation.

---

## Overview

The extraction phase converts source materials into clean, structured text that can be analyzed and transformed into study notes. The goal is to preserve content fidelity while removing formatting noise.

**Key principles**:
- **Content fidelity**: Do not alter, summarize, or omit any content during extraction
- **Structure preservation**: Maintain page/slide boundaries, heading hierarchy, and list structure
- **Encoding**: Always use UTF-8 to preserve special characters (math symbols, diacritics, etc.)
- **Layout**: Preserve spatial relationships (tables, columns) when possible

---

## PDF Extraction

### Tool: pdftotext (poppler-utils)

**Command**:
```bash
pdftotext -layout -enc UTF-8 input.pdf output.txt
```

**Flags**:
- `-layout`: Preserve spatial layout (tables, columns). Use this for notes with tables or multi-column content.
- `-enc UTF-8`: Ensure proper encoding for special characters.
- `-raw`: Alternative to `-layout`. Preserves reading order but loses spatial layout. Use for single-column text-heavy PDFs.

**Page counting**:
```bash
# Count pages via form-feed characters
python -c "print(open('output.txt').read().count('\x0c'))"

# Or use pdfinfo (if available)
pdfinfo input.pdf | grep Pages
```

**Handling errors**:
- "Unknown font tag" warnings: Common for PDFs with embedded fonts. Usually safe to ignore—text is still extracted correctly.
- Missing characters (shown as `?` or `\ufffd`): Indicates font encoding issue. Try `-raw` flag or alternative extraction tool.
- Garbled text: PDF may be image-based (scanned). Use OCR tool (tesseract) instead.

### Alternative: Python libraries

If pdftotext unavailable or insufficient:

```python
# PyPDF2 (basic extraction)
import PyPDF2
with open('input.pdf', 'rb') as f:
    reader = PyPDF2.PdfReader(f)
    text = ''
    for page in reader.pages:
        text += page.extract_text() + '\n\x0c'  # Add form-feed as page separator

# pdfplumber (better for tables)
import pdfplumber
with pdfplumber.open('input.pdf') as pdf:
    text = ''
    for page in pdf.pages:
        text += page.extract_text(layout=True) + '\n\x0c'
```

### Verification

After extraction, verify:
- [ ] Page count matches PDF page count
- [ ] No garbled text (check for `\ufffd` replacement characters)
- [ ] Tables are readable (columns aligned)
- [ ] Special characters preserved (math symbols, diacritics)
- [ ] Word count is reasonable (compare to PDF file size: ~100 words per KB for text-heavy PDFs)

---

## PPT/PPTX Extraction

### Tool: python-pptx

**Installation**:
```bash
pip install python-pptx
```

**Extraction script**:
```python
from pptx import Presentation

prs = Presentation('input.pptx')
text = ''
for i, slide in enumerate(prs.slides, 1):
    slide_text = f'--- Slide {i} ---\n'
    for shape in slide.shapes:
        if hasattr(shape, 'text'):
            slide_text += shape.text + '\n'
    text += slide_text + '\n\x0c'  # Form-feed as slide separator

with open('output.txt', 'w', encoding='utf-8') as f:
    f.write(text)
```

**Handling notes**:
```python
# Extract speaker notes
for slide in prs.slides:
    if slide.has_notes_slide:
        notes = slide.notes_slide.notes_text_frame.text
        # Append to slide text
```

**Handling tables**:
```python
for shape in slide.shapes:
    if shape.has_table:
        table = shape.table
        for row in table.rows:
            row_text = ' | '.join(cell.text for cell in row.cells)
            slide_text += row_text + '\n'
```

### Alternative: LibreOffice conversion

Convert PPTX to PDF, then extract:
```bash
libreoffice --headless --convert-to pdf input.pptx
pdftotext -layout input.pdf output.txt
```

### Verification

After extraction, verify:
- [ ] Slide count matches PPTX slide count
- [ ] All text from shapes extracted (check for missing content)
- [ ] Tables converted to readable format
- [ ] Speaker notes included (if relevant)
- [ ] Images/diagrams noted as placeholders

---

## DOCX Extraction

### Tool: python-docx

**Installation**:
```bash
pip install python-docx
```

**Extraction script**:
```python
from docx import Document

doc = Document('input.docx')
text = ''
for para in doc.paragraphs:
    # Preserve heading hierarchy
    if para.style.name.startswith('Heading'):
        level = int(para.style.name.split()[-1])
        text += '#' * level + ' ' + para.text + '\n\n'
    else:
        text += para.text + '\n'

# Extract tables
for table in doc.tables:
    for row in table.rows:
        row_text = ' | '.join(cell.text for cell in row.cells)
        text += row_text + '\n'
    text += '\n'

with open('output.txt', 'w', encoding='utf-8') as f:
    f.write(text)
```

### Alternative: Pandoc conversion

Convert DOCX to Markdown:
```bash
pandoc input.docx -o output.md
```

### Verification

After extraction, verify:
- [ ] Heading hierarchy preserved (H1, H2, H3)
- [ ] Tables converted to Markdown format
- [ ] Lists preserved (bullets, numbered)
- [ ] Special formatting noted (bold, italic, underline)
- [ ] Images/diagrams noted as placeholders

---

## Markdown (MD) Input

If input is already Markdown, no extraction needed. Proceed to Phase 1 (Analyze).

**Preprocessing** (optional):
- Normalize line endings: `dos2unix input.md`
- Remove frontmatter (YAML metadata) if present
- Ensure UTF-8 encoding

---

## Plain Text (TXT) Input

If input is plain text, minimal preprocessing:
- Ensure UTF-8 encoding
- Detect page boundaries (if marked with form-feeds or "--- Page N ---")
- Detect heading hierarchy (if marked with ALL CAPS or underlines)

---

## Handling Images and Diagrams

If source contains critical images/diagrams not extractable as text:

1. **Note placeholder**: Insert `[Diagram: description]` in extracted text
2. **Inform user**: "Source contains N diagrams that could not be extracted. I've noted their locations. If you need these diagrams described, please provide alt text or descriptions."
3. **Proceed with text**: Continue note generation using available text content

**Example**:
```
[Diagram: Flowchart showing process A → B → C with decision points]

The process begins with [input] and proceeds through three stages...
```

---

## Handling Mathematical Formulas

If source contains mathematical formulas:

1. **LaTeX notation**: If source uses LaTeX (e.g., `$E = mc^2$`), preserve as-is
2. **Unicode math**: If source uses Unicode symbols (e.g., `∑`, `∫`, `√`), preserve as-is
3. **Image-based formulas**: If formulas are images, note placeholder: `[Formula: description]`

**Example**:
```
The quadratic formula is:

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

where a, b, c are coefficients.
```

---

## Handling Code Snippets

If source contains code:

1. **Preserve language**: Detect language (Python, Java, SQL, etc.)
2. **Use code blocks**: Wrap in ```language ... ```
3. **Preserve indentation**: Maintain whitespace for readability

**Example**:
```python
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
```

---

## Quality Checklist

Before proceeding to Phase 1 (Analyze), verify extraction quality:

- [ ] **Encoding**: UTF-8, no garbled characters
- [ ] **Completeness**: All text extracted (compare word count to source size)
- [ ] **Structure**: Page/slide boundaries marked, headings preserved
- [ ] **Tables**: Readable format (pipe-delimited or aligned columns)
- [ ] **Special content**: Math, code, diagrams handled appropriately
- [ ] **Placeholders**: Missing content noted with `[...]` markers

---

## Common Issues and Solutions

### Issue: PDF text is garbled or missing
**Solution**: 
- Try `-raw` flag instead of `-layout`
- Use alternative tool (pdfplumber, PyPDF2)
- If image-based PDF, use OCR (tesseract)

### Issue: PPTX tables not extracted
**Solution**:
- Check if table is actually a table shape (not image)
- Use python-pptx `shape.has_table` check
- If table is image, note placeholder

### Issue: DOCX headings not detected
**Solution**:
- Check paragraph style names (may not be "Heading 1", "Heading 2")
- Use heuristic: detect ALL CAPS or underlined text as headings
- Manual review may be needed

### Issue: Math formulas not readable
**Solution**:
- If LaTeX, preserve as-is
- If Unicode, preserve as-is
- If image-based, note placeholder and inform user

### Issue: Code snippets lose formatting
**Solution**:
- Use code blocks with language tag
- Preserve indentation (use monospace font in output)
- Check for line wrapping issues

---

## Example Extraction Workflow

**User provides**: `lecture-slides.pptx` (20 slides, includes tables and diagrams)

**Step 1**: Extract text
```bash
python extract_pptx.py lecture-slides.pptx output.txt
```

**Step 2**: Verify extraction
```bash
# Check slide count
grep -c "--- Slide" output.txt  # Should be 20

# Check for missing content
wc -w output.txt  # Should be ~2000-4000 words for 20 slides

# Check for placeholders
grep -c "\[Diagram:" output.txt  # Note how many diagrams missing
```

**Step 3**: Inform user
```
Extracted 20 slides (~3000 words). Found 3 diagrams that could not be extracted. 
Proceeding with text content. If you need diagrams described, please provide alt text.
```

**Step 4**: Proceed to Phase 1 (Analyze)

---

## Final Notes

Extraction is the foundation of the note-generation pipeline. Poor extraction leads to poor notes. Always verify extraction quality before proceeding.

When in doubt, err on the side of **preserving more content** rather than less. It's easier to trim excess during note generation than to recover lost content.

Good luck, and selamat mengekstrak!
