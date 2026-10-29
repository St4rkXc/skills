---
name: thetold-er
description: Generate comprehensive study notes from source materials (PDF, PPT, DOCX, MD, TXT) in two modes — medium (ringkasan padat) or detailed (tutorial lengkap). Triggers when user runs /thetold-er or says "buat catatan medium", "generate detailed notes", "ubah materi ini jadi catatan", "extract dan buat catatan", "make study notes from this". Outputs structured markdown (ready for Notion import) with tutor voice, analogies, examples, tables, and encouragement. Supports any subject — math, business, CS, science, humanities.
---

# TheTold-Er: Study Notes Generator

A skill for transforming source materials (lecture slides, textbooks, articles, PDFs, presentations, documents) into structured study notes with two depth levels: **medium** (concise summaries) and **detailed** (comprehensive tutorials). The output preserves the tutor voice, pedagogical structure, and encouragement patterns of effective learning materials while adapting to any subject domain.

## Why this matters

Raw source materials are often dense, unstructured, or optimized for delivery rather than retention. Students need notes that:
- Extract core concepts without losing nuance
- Provide worked examples and step-by-step explanations
- Use analogies and real-world connections
- Include tables, comparisons, and visual structure
- Motivate with encouragement and clear progression

This skill bridges the gap between "information dump" and "learnable material" by enforcing proven pedagogical patterns observed in effective tutoring.

## Triggers

Activate this skill when:
- User inputs `/thetold-er` command
- User says: "buat catatan medium", "buat catatan detailed", "generate study notes", "ubah materi ini jadi catatan", "extract dan buat catatan", "make notes from this PDF/PPT/DOCX"
- User provides source material (PDF, PPT, DOCX, MD, TXT) and asks for notes/summaries
- User mentions "medium mode" or "detailed mode" in context of note-taking

---

## Workflow

The skill executes in four phases: **Extract → Analyze → Choose Mode → Generate**.

---

## Phase 0: Extract Source Material

If input is already plain text or markdown, skip to Phase 1.

For PDF/PPT/DOCX:
1. **PDF**: Use `pdftotext -layout -enc UTF-8` (or equivalent) to extract text preserving layout. Count pages via form-feed characters (`\x0c`).
2. **PPT/PPTX**: Extract text from each slide. Note slide numbers as page boundaries.
3. **DOCX**: Extract paragraphs preserving heading hierarchy if available.
4. **Images/Diagrams**: If source contains critical diagrams not extractable as text, note "[Diagram: description]" placeholder and inform user.

**Output of Phase 0**: Clean text with page/slide boundaries marked. Store in working memory or temp file.

---

## Phase 1: Analyze Source Material

Before generating notes, understand the input:

1. **Subject domain**: Math, business, CS, science, humanities, etc.
2. **Content type**: Definitions, procedures, theories, case studies, proofs, examples.
3. **Structure**: Does source have chapters/sections? Headings? Numbered lists?
4. **Key concepts**: Identify 5–10 core terms/concepts that must appear in output.
5. **Examples/worked problems**: Note any examples, case studies, or step-by-step solutions in source.
6. **Formulas/diagrams**: Flag mathematical formulas, code snippets, or diagrams that need special handling (LaTeX, code blocks, or descriptive placeholders).
7. **Source length**: Estimate word count of extracted text. This informs output length targets.

**Output of Phase 1**: Brief analysis summary (internal, not shown to user unless asked):
```
Domain: [subject]
Key concepts: [list]
Examples in source: [count]
Formulas/diagrams: [count]
Source word count: [N]
```

---

## Phase 2: Choose Mode

Ask user (or infer from context):

**Medium mode** (default if unspecified):
- Target: 900–2800 words (equivalent to 8–14 pages at ~160 words/page)
- Use when: user wants quick review, already has context, needs concise summaries
- Output: 1 section per major topic, each ~1 page

**Detailed mode**:
- Target: 3000–8000 words (equivalent to 16–39 pages at ~195 words/page)
- Use when: user is learning from scratch, needs deep understanding, wants worked examples
- Output: 1 section per major topic, each 1.5–3 pages

**Proportional scaling**: If source material is very short (<1000 words), scale down proportionally. If source is very long (>10,000 words), scale up but cap at 8000 words for detailed.

Confirm mode with user before generating:
```
Saya akan membuat catatan [medium/detailed] dari materi ini. Target panjang: [X]–[Y] kata. Lanjut?
```

---

## Phase 3: Generate Notes

Follow the pattern for chosen mode (see `references/medium-pattern.md` or `references/detailed-pattern.md`).

**Output format**: Markdown (ready for Notion import). Use:
- `#` for main title (topic name)
- `##` for section headings
- `###` for sub-sections
- `| tabel |` for comparison tables
- `-` for bullet lists
- `1.` for numbered lists
- `**bold**` for emphasis
- `*italic*` for key terms on first mention
- `> blockquote` for important notes or warnings
- `$$...$$` for LaTeX math (if Notion supports) or plain text formulas

**Branding**: First line of output: `Stark Dox Knowledge`

**Language**: Bahasa Indonesia, formal-santai, tutor voice. See shared language rules below.

---

## Shared Language Rules (Both Modes)

### Voice & Tone
- **Primary pronoun**: "kita" (inclusive, ~5–9 per 1000 words)
- **Secondary pronoun**: "kamu" (direct address, ~1–2.5 per 1000 words)
- **"Anda"**: Only if source material uses it (formal context)
- **Zero slang**: No "lu/gue/bro/gan"
- **Zero emoji**: No decorative symbols

### Sentence Structure
- **Average length**: 15–20 words per sentence
- **Em dash "—"**: Use for apposition/clarification (e.g., `pemasaran adalah "memenuhi kebutuhan secara menguntungkan"— mengubah kebutuhan...`)
- **Key terms**: Quote + English in parentheses on first mention (e.g., `layanan purna jual (after sales service)`)
- **Rhetorical questions**: 2–3 per 1000 words (e.g., "Mengapa ini penting?", "Pernah dengar ungkapan...?")

### Section Openers
- `Halo! Mari kita [pelajari/bedah/bahas]...`
- `Yuk, kita [pelajari/bedah] satu per satu.`
- `Bayangkan [analogi/situasi]...`
- `Pernah dengar [pertanyaan retoris]?`
- `Intinya, [recap]...`

### Section Closers
- `Intinya, [1-sentence summary].`
- `Semangat belajar!`
- `Selamat berlatih!`
- `Sampai jumpa di bab berikutnya!`
- `Jangan ragu untuk berlatih [aktivitas]. Semakin sering kamu [aktivitas], semakin [outcome].`

### Tables
- **Minimum 1 table per section** in both modes
- Format: `| Aspek | Penjelasan |` or `| Komponen | Peran |`
- Use for: comparisons, component lists, step summaries, rule summaries

### Cross-References (Detailed Only)
- Reference earlier examples: "Seperti pada Contoh 3..."
- Reference prior sections: "Sampai di sini kita sudah paham bahwa [X]. Nah, sekarang..."
- Bridge to next section: "Bekal ini akan berguna saat kamu mempelajari [Y] di bab berikutnya."

---

## Medium Pattern

**Target**: 900–2800 words total. Each section ≈ 1 page (~160 words).

### Section Structure (repeat per major topic)

1. **Section title** (topic name)
2. **Subtitle** (question format): "Mengapa [X] Krusial?" or "Apa Itu [X]?"
3. **Definition** (1–2 short paragraphs): Direct to point, no preamble. Answer "what is it?" and "why does it matter?" in 2–3 sentences.
4. **Comparison table** (2–4 rows): `| Aspek | Penjelasan |` or `| Komponen | Peran |`. Compare aspects, list components, or summarize key attributes.
5. **Bullet list** (3–4 items): Key points, characteristics, or steps. Use `-` format.
6. **Concrete example** (1 brief example): Real-world application, not a long worked problem. E.g., "Contoh: garansi perbaikan, layanan konsultasi penggunaan produk, dan penanganan keluhan pelanggan."
7. **Recap** (1 sentence): "Intinya, [X] menjaga [outcome] dan [outcome]."
8. **Source citation** (if applicable): "Menurut [Author/Org] ([Year]), [concept]..."
9. **Encouragement** (optional): "Semangat belajar!" or "Fondasi ini akan berguna di bab berikutnya."

### What Medium Includes
- Definitions + "what/why" + 1 example
- Tables for visual structure
- Bullet summaries
- Occasional source citations

### What Medium Excludes
- Proofs/derivations
- Step-by-step worked examples (just 1 brief example)
- Numbered "Langkah 1, Langkah 2" sequences
- "Catatan Penting dan Kesalahan Umum" sections
- Mnemonics/memory aids
- Cross-references between sections
- Bridges to next chapter

### Example Medium Section

```markdown
## Mengapa Pemasaran dan Penjualan Krusial?

Pemasaran mencakup penciptaan, komunikasi, penyampaian, dan pertukaran penawaran yang bernilai bagi pelanggan, mitra, dan masyarakat. Penjualan adalah transaksi pertukaran barang, jasa, atau aset dengan uang. Pendapatan di atas laba. Prinsipnya: "There must be a top line for there to be a bottom line." Tanpa permintaan yang cukup, fungsi keuangan, operasional, dan akuntansi tak berarti banyak—perusahaan tak bisa mencetak laba.

Pemasaran juga berperan dalam:

- Memperkenalkan produk baru agar diterima pasar.
- Mendorong penyempurnaan produk yang sudah ada.
- Menciptakan lapangan kerja dan membangun permintaan.
- Menopang tanggung jawab sosial perusahaan melalui nilai bagi masyarakat.

Singkatnya, pemasaran dan penjualan adalah mesin yang menghidupkan seluruh fungsi bisnis lainnya.

| Aspek | Penjelasan |
|-------|------------|
| Pemasaran | Mengidentifikasi kebutuhan, menciptakan penawaran, berkomunikasi dengan pasar |
| Penjualan | Transaksi pertukaran, konversi prospek menjadi pelanggan |
| Purna jual | Layanan setelah penjualan, menjaga kepuasan pelanggan |

Contoh: Sebuah perusahaan teknologi meluncurkan produk baru. Tim pemasaran melakukan riset pasar, merancang kampanye, dan membangun kesadaran merek. Tim penjualan menghubungi prospek, mendemonstrasikan produk, dan menutup kesepakatan. Tim purna jual menangani keluhan, memberikan garansi, dan membangun hubungan jangka panjang.

Intinya, pemasaran dan penjualan adalah mesin yang menghidupkan seluruh fungsi bisnis lainnya.
```

---

## Detailed Pattern

**Target**: 3000–8000 words total. Each section ≈ 1.5–3 pages (~195 words/page).

### Section Structure (repeat per major topic)

1. **Greeting + hook analogy** (1 paragraph): "Halo! Mari kita bahas [topic]. Bayangkan [analogi/situasi]..." or "Halo! Selamat datang di [topic]. Materi ini adalah fondasi penting yang akan kamu gunakan terus-menerus..."
2. **Motivation** (1–2 sentences): Why this matters, how it connects to prior/next chapters. "Pemahaman ini akan menjadi bekal berharga saat kamu mempelajari [Y] di bab-bab berikutnya."
3. **Formal definition** (1 paragraph): Precise, includes notation/formula if applicable. For non-math: exact terminology, framework, or model from source.
4. **Conditions/prerequisites** (explicit statement): "Syarat penting: [X] hanya dapat [Y] jika [Z]." or "Sebelum masuk ke [topic], ingat dulu bahwa..."
5. **Explanation** (2–4 paragraphs): Break down concept step-by-step. Use analogies, real-world connections, and progressive disclosure (simple → complex).
6. **Comparison table** (3–6 rows): `| Komponen | Penjelasan |` or `| Operasi | Syarat | Contoh |`. More detailed than medium.
7. **Worked example with number** (1–2 examples): "Contoh 1: [Title]" → "Langkah 1 — [action]", "Langkah 2 — [action]" → "Hasil akhirnya adalah [outcome]." For non-math: case study walkthrough with same step structure (input → proses → hasil).
8. **Verification** (1 paragraph): "Mari kita periksa satu per satu [elemen/hasil]..." or "Perhatikan bahwa [X] memang [Y], sesuai dengan [prinsip/teorema]."
9. **Proof/derivation** (if applicable): "Pembuktian [Teorema X]" → "Langkah 1 — [action]", "Langkah 2 — [action]" → "Terbukti!" For non-math: "Mengapa ini benar?" reasoning with logical flow.
10. **Mnemonic/memory aid** (1–2 sentences): "Mnemonik: [rule]" or "Kaidah tanda: [pattern]" or "Ingat saja: [shortcut]."
11. **"Catatan Penting dan Kesalahan Umum"** (1 section): Bullet list of pitfalls. "Jangan tertukar [X] dan [Y]." "Hati-hati: [common mistake]." "Peringatan: [X] tidak menjamin [Y]."
12. **Summary table** (1 table): "Rangkuman Syarat Tiap Operasi" or "Ringkasan Konsep Kunci". Consolidates rules, conditions, or key points.
13. **Conclusion/penutup** (1 paragraph): Recap main points, encouragement, bridge to next section. "Selamat! Kamu sudah mengenal [topic]. Pemahaman ini akan menjadi bekal berharga saat kamu mempelajari [next topic]. Sampai jumpa di bab berikutnya!"

### What Detailed Includes
- Everything in medium, plus:
- Greeting + analogy hook
- Motivation + chapter bridges
- Formal definitions + notation
- Conditions/prerequisites
- Step-by-step worked examples ("Langkah 1, Langkah 2")
- Proofs/derivations (or "mengapa ini benar" reasoning)
- Mnemonics/memory aids
- "Catatan Penting dan Kesalahan Umum"
- Cross-references ("Seperti pada Contoh 3", "Sampai di sini kita sudah paham...")
- Summary tables

### What Detailed Excludes
- Nothing from medium is excluded; detailed is additive

### Example Detailed Section

```markdown
## Operasi Aritmetika Matriks

Halo! Pada catatan kali ini kita akan belajar tiga operasi dasar yang paling sering dipakai saat bekerja dengan matriks, yaitu penjumlahan dua matriks, perkalian matriks dengan skalar, dan perkalian dua matriks. Ketiganya punya aturan main masing-masing, dan memahami syarat dimensinya adalah kunci supaya kita tidak salah hitung. Yuk, kita bahas satu per satu dengan tenang dan menyeluruh.

Sebelum masuk ke operasi, ingat dulu bahwa matriks adalah susunan bilangan dalam baris dan kolom. Ukuran (dimensi) matriks ditulis sebagai jumlah baris × jumlah kolom, misalnya matriks berukuran 2 × 3 berarti punya 2 baris dan 3 kolom.

### 1. Penjumlahan Dua Matriks

Penjumlahan dua matriks dilakukan dengan menjumlahkan elemen-elemen yang posisinya bersesuaian. Artinya, elemen pada baris ke-i kolom ke-j matriks pertama dijumlahkan dengan elemen pada baris ke-i kolom ke-j matriks kedua.

**Syarat penting**: dua matriks hanya dapat dijumlahkan jika keduanya memiliki ukuran (dimensi) yang sama. Matriks 2 × 3 hanya bisa dijumlahkan dengan matriks 2 × 3, bukan dengan matriks 3 × 2.

**Contoh 1**: Jumlahkan dua matriks berukuran 3 × 3:

$$
\begin{bmatrix} 1 & 2 & 3 \\ 5 & -3 & 5 \\ 4 & -2 & 8 \end{bmatrix} + \begin{bmatrix} 5 & 6 & 8 \\ 7 & 2 & 7 \\ 0 & 8 & 11 \end{bmatrix} = \begin{bmatrix} 1+5 & 2+6 & 3+8 \\ 5+7 & -3+2 & 5+7 \\ 4+0 & -2+8 & 8+11 \end{bmatrix} = \begin{bmatrix} 6 & 8 & 11 \\ 12 & -1 & 12 \\ 4 & 6 & 19 \end{bmatrix}
$$

Lihat bagaimana setiap pasangan elemen yang seposisi dijumlahkan langsung? Itulah inti dari operasi penjumlahan matriks — sederhana dan konsisten, selama ukurannya cocok.

### Catatan Penting dan Kesalahan Umum

- **Jangan tertukar urutan**. Perkalian matriks umumnya tidak komutatif, artinya AB belum tentu sama dengan BA. Bahkan, bisa jadi AB dapat dihitung tetapi BA justru tidak bisa karena syarat dimensi tidak terpenuhi. Selalu periksa dimensi sebelum menghitung.
- **Perhatikan dimensi hasil**. Perkalian m × n dengan n × p menghasilkan matriks m × p, bukan n × n.
- **Hati-hati dengan tanda negatif**. Saat mengalikan atau menjumlahkan elemen negatif, pastikan tanda minus tidak hilang.

### Rangkuman Syarat Tiap Operasi

| Operasi | Syarat | Contoh Ukuran Valid |
|---------|--------|---------------------|
| Penjumlahan A + B | Dimensi A dan B harus sama | 2 × 3 dengan 2 × 3 |
| Perkalian skalar kA | Tidak ada syarat khusus | k dengan matriks apa pun |
| Perkalian A × B | Kolom A sama dengan baris B | 2 × 3 dikali 3 × 2 |

Intinya, memahami syarat dimensi adalah kunci supaya kita tidak salah hitung. Selamat berlatih!
```

---

## Output Structure

### File Format
- **Filename**: `[Topic]-[Mode]-Notes.md` (e.g., `Matriks-Detailed-Notes.md`, `Pemasaran-Medium-Notes.md`)
- **Encoding**: UTF-8
- **Line endings**: LF (Unix-style)

### Document Structure

```markdown
Stark Dox Knowledge

# [Main Topic Title]

## [Section 1 Title]
### [Subtitle question]
[Content following pattern]

## [Section 2 Title]
### [Subtitle question]
[Content following pattern]

...

## Penutup
[Final encouragement + summary]
```

### Markdown Elements

- **Headings**: `#` main title, `##` sections, `###` sub-sections
- **Tables**: `| Column | Column |` with `|---|---|` separator
- **Lists**: `-` bullets, `1.` numbered
- **Emphasis**: `**bold**` for key terms, `*italic*` for first mention of technical terms
- **Blockquotes**: `>` for important notes, warnings, or "Catatan Penting"
- **Math**: `$$...$$` for block equations, `$...$` for inline (if Notion supports LaTeX)
- **Code**: ` ```language ... ``` ` for code snippets (if applicable)

### Notion Compatibility

Output is optimized for Notion import:
- Use standard markdown syntax
- Avoid HTML tags
- Use `$$...$$` for math (Notion renders LaTeX)
- Tables use pipe syntax (Notion converts to native tables)
- Headings use `#` syntax (Notion converts to heading blocks)

---

## Quality Checklist

Before delivering output, verify:

- [ ] **Length target met**: Medium 900–2800 words, Detailed 3000–8000 words (or proportional)
- [ ] **All key concepts covered**: 5–10 core terms from Phase 1 analysis appear in output
- [ ] **Tables present**: Minimum 1 table per section
- [ ] **Examples included**: Medium has 1 brief example per section; Detailed has 1–2 worked examples with steps
- [ ] **Language correct**: "kita" dominant, "kamu" secondary, no slang, no emoji
- [ ] **Section openers/closers**: Each section starts with greeting/hook and ends with encouragement
- [ ] **Cross-references** (Detailed only): At least 2–3 cross-references per 1000 words
- [ ] **Mnemonics** (Detailed only): At least 1 mnemonic/memory aid per major concept
- [ ] **Pitfalls** (Detailed only): "Catatan Penting dan Kesalahan Umum" section present
- [ ] **Markdown valid**: No broken tables, no unclosed code blocks, no invalid syntax
- [ ] **Branding**: First line is "Stark Dox Knowledge"

---

## References

For detailed pattern templates and examples, see:
- `references/medium-pattern.md` — Full medium template with annotated examples
- `references/detailed-pattern.md` — Full detailed template with annotated examples
- `references/extraction-guide.md` — How to handle different input formats (PDF, PPT, DOCX)

### Example Notes (references/examples/)

The `references/examples/` folder contains **21 real extracted notes** (7 medium, 14 detailed) from actual AI-generated study materials across math, business, and CS domains.

**Each example file has a YAML metadata header**:
```yaml
---
mode: medium | detailed
pages: [number]
words: [count]
---
```

**MANDATORY: Before generating notes, read examples matching the chosen mode**:

1. **List available examples**:
   ```bash
   # For medium mode
   grep -l "mode: medium" references/examples/*.md
   
   # For detailed mode
   grep -l "mode: detailed" references/examples/*.md
   ```

2. **Read 2–3 examples** from the chosen mode to internalize the pattern:
   - For **medium**: Read files with `mode: medium` header
   - For **detailed**: Read files with `mode: detailed` header
   - Prefer examples from the **same domain** as the user's input (math, business, CS)

3. **Do NOT read all 21 examples** — that's ~630KB and will overflow context. Only read examples matching the chosen mode.

**Example selection by domain**:
- **Math**: `Week_1_Bilangan_Real`, `Week_5_Matriks`, `Week_6_Turunan`, `Diskrit_Week 6 Matriks part 2`
- **Business**: `Sistem_Enterprise_*`, `Week 1 Enterprise System`, `Week 2 Business Process`
- **CS**: `Week 1 Logic`, `Week_2_Logic_2`, `Week_3_HimpunanNotes`

**Why this matters**: Reading real examples ensures output matches the proven pattern. The examples demonstrate exact phrasing, table structure, encouragement style, and section flow.

---

## Common Pitfalls

1. **Too short**: If output is under target word count, add more examples, tables, or explanations.
2. **Too formal**: Avoid academic tone. Use "kita" and "kamu" to create tutor-student rapport.
3. **Missing tables**: Every section needs at least 1 table. If source has no table, create one summarizing key points.
4. **No examples**: Medium needs 1 brief example per section; Detailed needs 1–2 worked examples with steps.
5. **Broken markdown**: Test tables render correctly. Ensure `|---|---|` separator is present.
6. **Inconsistent voice**: Don't switch between "kita", "kamu", and "Anda" randomly. Stick to "kita" primary, "kamu" secondary.
7. **Missing encouragement**: Every section should end with "Semangat belajar!" or similar.

---

## Example Prompts

**User**: "Buat catatan medium dari PDF ini tentang sistem operasi."
**Skill**: Extracts PDF → Analyzes (domain: CS, key concepts: process, thread, scheduling, memory) → Confirms medium mode (target 1500 words) → Generates notes with 5 sections (Process, Thread, Scheduling, Memory, File System), each with definition, table, bullets, example, recap.

**User**: "Generate detailed notes from this PPT about marketing."
**Skill**: Extracts PPT → Analyzes (domain: business, key concepts: 4P, segmentation, positioning, branding) → Confirms detailed mode (target 5000 words) → Generates notes with 6 sections, each with greeting, analogy, definition, conditions, explanation, table, worked example (case study), verification, mnemonic, pitfalls, summary table, conclusion.

**User**: "Ubah materi ini jadi catatan."
**Skill**: Asks "Medium atau detailed?" → User says "detailed" → Proceeds with workflow.

---

## Final Notes

This skill is designed to be **comprehensive but flexible**. The patterns are based on analysis of 21 real study notes (7 medium, 14 detailed) across math, business, and CS domains. The structure works for any subject because it focuses on **pedagogical principles** (definition → example → recap → encouragement) rather than domain-specific content.

When in doubt, err on the side of **more explanation, more examples, more tables**. Students prefer over-explained notes to under-explained notes.

Good luck, and selamat mengajar!
