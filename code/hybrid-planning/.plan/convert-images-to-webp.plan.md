# Plan: Image to WebP Conversion Script

**Version:** 1.0
**Status:** COMPLETE
**Created:** 2026-05-30
**Estimated Steps:** 3

---

## 1. Context & Goals

> Create a reliable, cross-platform script to recursively find and convert common image formats (`.png`, `.jpg`, `.jpeg`) to `.webp`. The script will use Node.js and the `sharp` library for fast, high-quality image processing. It will traverse directories, convert files, and optionally allow for deleting the original files to save space.

**Out of Scope:** 
- Converting SVGs or animated GIFs.
- Real-time image optimization for a web server (this is a static build/utility script).
- Integration into a specific build pipeline (Webpack/Vite) — this is a standalone utility.

---

## 2. Affected Files Map

### Created

- `scripts/convert-to-webp.mjs` — The standalone Node.js script to perform the conversion.
- `package.json` (modified/created) — To ensure `sharp` and `glob` dependencies are listed if not already present.

### Modified

- None

### Deleted

- None (Original images will be kept by default unless specified).

---

## 3. Architectural Design

### 3.1 Component / Module Hierarchy

- `scripts/convert-to-webp.mjs`:
  - Uses `glob` to find all target images.
  - Uses `sharp` to read the image buffer and output a `.webp` file.
  - Exposes CLI flags (e.g., `--dir` to specify the target directory, `--delete` to remove originals).

---

## 4. Strict Contract Definitions

### 4.1 CLI Arguments Interface

```ts
interface ScriptOptions {
    targetDir: string;      // Default: './public/images' or './'
    deleteOriginals: boolean; // Default: false
    quality: number;        // Default: 80
}
```

---

## 5. Edge Cases & Security Audit

| #   | Scenario                            | Expected Behavior | Mitigation |
| --- | ----------------------------------- | ----------------- | ---------- |
| 1   | Target directory does not exist     | Script exits gracefully with a warning | Check `fs.existsSync(dir)` before running |
| 2   | Image is already `.webp`            | Skip file | Glob pattern only matches `.jpg`, `.jpeg`, `.png` |
| 3   | File permission denied              | Log error for that specific file and continue | Try-catch block around the `sharp()` execution |
| 4   | `sharp` module not installed        | Script fails immediately | Provide `npm install` instructions in the script execution step |
| 5   | Corrupted input image               | Log error, skip to next file | Catch `sharp` processing errors |
**Status:** COMPLETE

---

## 6. Step-by-Step Execution Checklist

- [x] **Step 1** — `package.json` — Add/install `sharp` and `glob` dependencies.
- [x] **Step 2** — `scripts/convert-to-webp.mjs` — Create the conversion script, implement argument parsing and directory traversal.
- [x] **Step 3** — `scripts/convert-to-webp.mjs` — Add `sharp` conversion logic, error handling, and terminal output logging.
---

## 7. Rollback Plan

- Files to delete: `scripts/convert-to-webp.mjs`
- Revert changes to `package.json` (remove `sharp`, `glob`).
- Delete any generated `.webp` files (can be done with a simple shell command if needed).

---

## 8. Validation Criteria

- [ ] Manual test: Run the script on a test directory containing `.jpg` and `.png` files.
- [ ] Verification: `.webp` files are successfully generated alongside the originals.
- [ ] Verification: The script handles invalid files without crashing.
