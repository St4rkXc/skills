# Example Notes Index

This folder contains **21 real extracted notes** from actual AI-generated study materials. Each file has YAML metadata header with `mode`, `pages`, and `words` fields.

**Usage**: When generating notes, read 2–3 examples matching the chosen mode (medium or detailed). Do NOT read all files — that's ~630KB and will overflow context.

---

## Medium Mode (7 files)

**Target**: 900–2800 words (8–14 pages)

| File | Domain | Pages | Words |
|------|--------|-------|-------|
| Akuntansi-Keuangan.md | Business | 12 | 1,518 |
| Business-Process.md | Business | 8 | 1,748 |
| CRM.md | Business | 8 | 868 |
| Kecerdasan-Buatan.md | Business | 9 | 1,431 |
| Limit.md | Math | 14 | 2,823 |
| Matriks-Part-2.md | Math | 10 | 1,665 |
| Supply-Chain.md | Business | 8 | 1,211 |

**Total**: 7 files, 69 pages, 11,264 words

---

## Detailed Mode (14 files)

**Target**: 3000–8000 words (16–39 pages)

| File | Domain | Pages | Words |
|------|--------|-------|-------|
| Bilangan-Real.md | Math | 35 | 7,358 |
| Enterprise-System.md | Business | 20 | 3,457 |
| Functional-Areas.md | Business | 17 | 3,142 |
| Fungsi.md | Math | 37 | 7,904 |
| Himpunan-Part-2.md | Math | 34 | 7,208 |
| Himpunan.md | Math | 18 | 3,283 |
| IDS-Integrated-Data.md | Business | 18 | 3,522 |
| Integrated-System.md | Business | 20 | 3,515 |
| Kekontinuan.md | Math | 16 | 3,012 |
| Logic-Part-2.md | Math | 35 | 7,049 |
| Logic.md | Math | 39 | 7,126 |
| Matriks.md | Math | 37 | 8,118 |
| Pertidaksamaan-Mutlak.md | Math | 37 | 8,133 |
| Turunan.md | Math | 22 | 3,737 |

**Total**: 14 files, 385 pages, 76,564 words

---

## Domain Distribution

| Domain | Medium | Detailed | Total |
|--------|--------|----------|-------|
| Math | 2 | 10 | 12 |
| Business | 5 | 4 | 9 |
| CS | 0 | 0 | 0 |

---

## How to Use

**For AI**: Before generating notes, run:
```bash
# List medium examples
grep -l "mode: medium" references/examples/*.md

# List detailed examples
grep -l "mode: detailed" references/examples/*.md
```

Then read 2–3 files matching the chosen mode and domain.

**For human**: Browse the tables above to find examples by domain and mode.
