# Detailed Pattern Reference

This document provides the complete template for **detailed mode** study notes, with annotated examples from real generated notes.

---

## Template Overview

**Target**: 3000–8000 words total (16–39 pages equivalent at ~195 words/page)

**Structure per section** (repeat for each major topic, 1.5–3 pages per section):
1. Greeting + hook analogy
2. Motivation + chapter bridge
3. Formal definition + notation
4. Conditions/prerequisites
5. Explanation (2–4 paragraphs)
6. Comparison table (3–6 rows)
7. Worked example with number ("Contoh 1: ...")
8. Step-by-step breakdown ("Langkah 1 — ...")
9. Verification ("Mari kita periksa...")
10. Proof/derivation (if applicable)
11. Mnemonic/memory aid
12. "Catatan Penting dan Kesalahan Umum"
13. Summary table
14. Conclusion/penutup + encouragement + bridge to next section

---

## Full Section Template

```markdown
## [Topic Name]

### [Greeting + Hook]

Halo! [Mari kita pelajari/bahas/bedah] [topic]. [Analogi: "Bayangkan..." atau "Konsep ini mirip dengan..."]. Materi ini adalah fondasi penting yang akan kamu gunakan terus-menerus, terutama saat mempelajari [related topic]. Yuk, kita bedah pelan-pelan mulai dari definisi paling dasar hingga [advanced concept].

### [Motivation]

Pemahaman ini akan menjadi bekal berharga saat kamu mempelajari [next topic] di bab-bab berikutnya. Jangan ragu untuk berlatih [activity]—semakin sering kamu berlatih, semakin intuitif rasanya.

### [Formal Definition]

Secara formal, [concept] didefinisikan sebagai [definition]. Dalam notasi ringkas, kita lazim menuliskan [notation]. Cara ini jauh lebih efisien daripada menuliskan [alternative].

### [Conditions/Prerequisites]

**Syarat penting**: [concept] hanya dapat [action] jika [condition]. [Concept A] berukuran m × n hanya bisa [operation] dengan [concept B] berukuran m × n, bukan dengan [concept B] berukuran n × m.

### [Explanation]

[2–4 paragraphs breaking down the concept. Use analogies, real-world connections, progressive disclosure.]

[Paragraph 1: Core idea with analogy]

[Paragraph 2: Elaboration with example]

[Paragraph 3: Edge cases or special conditions]

### [Comparison Table]

| Komponen | Penjelasan |
|----------|------------|
| [Component 1] | [Explanation 1] |
| [Component 2] | [Explanation 2] |
| [Component 3] | [Explanation 3] |
| [Component 4] | [Explanation 4] |
| [Component 5] | [Explanation 5] |

### [Worked Example]

**Contoh 1**: [Title]

Diberikan [inputs]. [Task description].

**Langkah 1** — [Action]: [Detailed explanation of step 1].

**Langkah 2** — [Action]: [Detailed explanation of step 2].

**Langkah 3** — [Action]: [Detailed explanation of step 3].

Hasil akhirnya adalah [result].

### [Verification]

Mari kita periksa satu per satu [elemen/hasil]:

- [Element 1]: [calculation] = [result] ✓
- [Element 2]: [calculation] = [result] ✓
- [Element 3]: [calculation] = [result] ✓

Hasil akhirnya memang [expected outcome], sesuai prediksi [principle/teorema].

### [Proof/Derivation] (if applicable)

**Pembuktian [Teorema X]**:

Kita perlu menunjukkan bahwa [statement]. Gunakan [method/trick]:

[Step-by-step derivation]

Karena [reason], hasilnya [conclusion]—persis definisi [concept]. **Terbukti!**

### [Mnemonic/Memory Aid]

**Mnemonik**: [Rule untuk mengingat]. Misalnya, [pattern] selalu [behavior]. Ini akan sangat menyelamatkanmu saat ujian!

### Catatan Penting dan Kesalahan Umum

> **Jangan tertukar** [X] dan [Y]. [Explanation of common confusion].

> **Hati-hati**: [Common mistake]. Selalu periksa [condition] sebelum [action].

> **Peringatan**: [X] tidak menjamin [Y]. Ingat [counterexample].

### [Summary Table]

| Operasi | Syarat | Contoh Valid |
|---------|--------|--------------|
| [Operation 1] | [Condition 1] | [Example 1] |
| [Operation 2] | [Condition 2] | [Example 2] |
| [Operation 3] | [Condition 3] | [Example 3] |

### [Conclusion]

Selamat! Kamu sudah mengenal [topic]: [recap of key points]. Pemahaman ini akan menjadi bekal berharga saat kamu mempelajari [next topic] di bab-bab berikutnya.

Jangan ragu untuk berlatih [activity]. Semakin sering kamu berlatih, semakin intuitif rasanya. Sampai jumpa di bab berikutnya!
```

---

## Annotated Example 1: Math (Matriks — Operasi Aritmetika)

**Source**: Matematika Diskrit — Matriks (37 halaman)

**Analysis**:
- Domain: Math (Linear Algebra)
- Key concepts: penjumlahan matriks, perkalian skalar, perkalian matriks, dimensi, syarat
- Examples in source: 3 worked examples with step-by-step
- Source word count: ~8000 words → detailed target: ~3500 words for this section

**Generated section**:

```markdown
## Operasi Aritmetika Matriks

Halo! Pada catatan kali ini kita akan belajar tiga operasi dasar yang paling sering dipakai saat bekerja dengan matriks, yaitu penjumlahan dua matriks, perkalian matriks dengan skalar, dan perkalian dua matriks. Ketiganya punya aturan main masing-masing, dan memahami syarat dimensinya adalah kunci supaya kita tidak salah hitung. Yuk, kita bahas satu per satu dengan tenang dan menyeluruh.

Sebelum masuk ke operasi, ingat dulu bahwa matriks adalah susunan bilangan dalam baris dan kolom. Ukuran (dimensi) matriks ditulis sebagai jumlah baris × jumlah kolom, misalnya matriks berukuran 2 × 3 berarti punya 2 baris dan 3 kolom.

### 1. Penjumlahan Dua Matriks

Penjumlahan dua matriks dilakukan dengan menjumlahkan elemen-elemen yang posisinya bersesuaian. Artinya, elemen pada baris ke-i kolom ke-j matriks pertama dijumlahkan dengan elemen pada baris ke-i kolom ke-j matriks kedua.

**Syarat penting**: dua matriks hanya dapat dijumlahkan jika keduanya memiliki ukuran (dimensi) yang sama. Matriks 2 × 3 hanya bisa dijumlahkan dengan matriks 2 × 3, bukan dengan matriks 3 × 2.

**Contoh 1**: Jumlahkan dua matriks berukuran 3 × 3:

$$
\begin{bmatrix} 1 & 2 & 3 \\ 5 & -3 & 5 \\ 4 & -2 & 8 \end{bmatrix} + \begin{bmatrix} 5 & 6 & 8 \\ 7 & 2 & 7 \\ 0 & 8 & 11 \end{bmatrix}
$$

**Langkah 1** — Periksa dimensi: kedua matriks berukuran 3 × 3, jadi penjumlahan valid.

**Langkah 2** — Jumlahkan elemen seposisi:

$$
= \begin{bmatrix} 1+5 & 2+6 & 3+8 \\ 5+7 & -3+2 & 5+7 \\ 4+0 & -2+8 & 8+11 \end{bmatrix} = \begin{bmatrix} 6 & 8 & 11 \\ 12 & -1 & 12 \\ 4 & 6 & 19 \end{bmatrix}
$$

Mari kita periksa satu per satu elemennya:

- Elemen baris 1, kolom 1: 1 + 5 = 6 ✓
- Elemen baris 1, kolom 2: 2 + 6 = 8 ✓
- Elemen baris 2, kolom 2: -3 + 2 = -1 ✓

Hasil akhirnya memang 3 × 3, sesuai prediksi dimensi.

### 2. Perkalian Matriks dengan Skalar

Operasi ini melibatkan sebuah skalar (yaitu sebuah bilangan tunggal) yang dikalikan dengan seluruh elemen matriks. Jika k adalah skalar dan A adalah matriks, maka kA diperoleh dengan mengalikan setiap elemen A dengan k.

**Contoh 2**: Misalkan A = [1 0 2; 3 7 0; -2 0 4], k = 3. Maka:

3A = [3×1 3×0 3×2; 3×3 3×7 3×0; 3×(-2) 3×0 3×4] = [3 0 6; 9 21 0; -6 0 12]

Perhatikan bahwa tidak ada syarat khusus soal dimensi di sini — skalar bisa dikalikan dengan matriks berukuran apa pun.

### 3. Perkalian Dua Matriks dan Syarat Dimensinya

Inilah operasi yang paling sering membuat bingung, jadi mari kita pelan-pelan. Dua buah matriks dapat dikalikan jika **jumlah kolom matriks pertama sama dengan jumlah baris matriks kedua**.

Jika matriks A berukuran m × n dan matriks B berukuran n × p, maka hasil perkalian AB akan berukuran m × p. Perhatikan bahwa angka n (kolom A dan baris B) harus sama — inilah syarat utamanya.

**Contoh 3**: Diketahui A = [1 0 2; 1 3 4] (2 × 3) dan B = [2 1; 4 3; 5 6] (3 × 2). Karena jumlah kolom A (3) sama dengan jumlah baris B (3), perkalian valid dan hasilnya akan berukuran 2 × 2.

**Langkah 1** — Periksa dimensi: A berukuran 2 × 3, B berukuran 3 × 2. Kolom A (3) = baris B (3) ✓

**Langkah 2** — Hitung elemen hasil perkalian:

- Elemen baris 1, kolom 1: (1)(2) + (0)(4) + (2)(5) = 2 + 0 + 10 = 12
- Elemen baris 1, kolom 2: (1)(1) + (0)(3) + (2)(6) = 1 + 0 + 12 = 13
- Elemen baris 2, kolom 1: (1)(2) + (3)(4) + (4)(5) = 2 + 12 + 20 = 34
- Elemen baris 2, kolom 2: (1)(1) + (3)(3) + (4)(6) = 1 + 9 + 24 = 34

Hasil akhirnya: AB = [12 13; 34 34] (2 × 2) ✓

### Catatan Penting dan Kesalahan Umum

> **Jangan tertukar urutan**. Perkalian matriks umumnya tidak komutatif, artinya AB belum tentu sama dengan BA. Bahkan, bisa jadi AB dapat dihitung tetapi BA justru tidak bisa karena syarat dimensi tidak terpenuhi. Selalu periksa dimensi sebelum menghitung.

> **Hati-hati dengan dimensi hasil**. Perkalian m × n dengan n × p menghasilkan matriks m × p, bukan n × n.

> **Peringatan**: Perkalian matriks tidak memiliki sifat pembatalan. Jika AB = AC, belum tentu B = C (kecuali A invertible).

### Rangkuman Syarat Tiap Operasi

| Operasi | Syarat | Contoh Ukuran Valid |
|---------|--------|---------------------|
| Penjumlahan A + B | Dimensi A dan B harus sama | 2 × 3 dengan 2 × 3 |
| Perkalian skalar kA | Tidak ada syarat khusus | k dengan matriks apa pun |
| Perkalian A × B | Kolom A sama dengan baris B | 2 × 3 dikali 3 × 2 |

Intinya, memahami syarat dimensi adalah kunci supaya kita tidak salah hitung. Selamat berlatih!
```

**Annotation**:
- ✅ Greeting + hook: "Halo! Pada catatan kali ini..."
- ✅ Motivation: implicit in "Yuk, kita bahas satu per satu dengan tenang dan menyeluruh"
- ✅ Formal definition: "Penjumlahan dua matriks dilakukan dengan..."
- ✅ Conditions: "**Syarat penting**: dua matriks hanya dapat dijumlahkan jika..."
- ✅ 3 worked examples with "Contoh 1", "Contoh 2", "Contoh 3"
- ✅ Step-by-step: "Langkah 1 — Periksa dimensi", "Langkah 2 — Jumlahkan..."
- ✅ Verification: "Mari kita periksa satu per satu elemennya..."
- ✅ Mnemonic: implicit in "Perhatikan bahwa angka n (kolom A dan baris B) harus sama"
- ✅ "Catatan Penting dan Kesalahan Umum" with 3 pitfalls
- ✅ Summary table: "Rangkuman Syarat Tiap Operasi"
- ✅ Conclusion: "Intinya, memahami syarat dimensi adalah kunci..."
- ✅ Encouragement: "Selamat berlatih!"
- ✅ Word count: ~1200 words (fits 6-page section)

---

## Annotated Example 2: Business (IDS — Integrated Data System)

**Source**: Sistem Enterprise — IDS (18 halaman)

**Analysis**:
- Domain: Business (IT/Systems)
- Key concepts: IDS, data sharing, interoperability, privacy, governance
- Examples in source: case studies of government agencies
- Source word count: ~3500 words → detailed target: ~3000 words

**Generated section**:

```markdown
## Pengenalan Sistem Data Terintegrasi (IDS)

### Apa Itu IDS (Sistem Data Terintegrasi)?

Halo! Mari kita bahas salah satu solusi paling menjanjikan untuk masalah data yang tersebar: IDS, atau Integrated Data System (Sistem Data Terintegrasi). Bayangkan jika lembaga-lembaga yang menangani anak dan keluarga bisa saling berbagi data tanpa mengorbankan keamanan. Inilah gagasan di balik IDS. Alih-alih setiap lembaga bekerja sendiri-sendiri dengan datanya masing-masing, IDS menghubungkan mereka dalam satu cara berbagi yang aman—sehingga semua pihak dapat memusatkan perhatian pada satu hal yang benar-benar penting: meningkatkan kehidupan anak-anak dan keluarga.

### Berbagi Data yang Aman

Inti dari IDS adalah berbagi data secara aman. Kata "aman" di sini bukan sekadar tambahan—ia adalah fondasi. Tanpa rasa aman, lembaga-lembaga tidak akan mau berbagi informasi yang sensitif. IDS dirancang justru untuk menjawab pertanyaan ini: bagaimana cara berbagi data yang melindungi privasi sekaligus memungkinkan kolaborasi?

Jawabannya: IDS menggunakan seperangkat aturan dan kesepakatan bersama yang disebut **governance framework**. Framework ini mengatur:

- **Siapa** yang boleh mengakses data
- **Data apa** yang boleh dibagikan
- **Untuk tujuan apa** data boleh digunakan
- **Bagaimana** data dilindungi dari penyalahgunaan

### Bagaimana IDS Bekerja?

IDS bukan sekadar perangkat lunak atau basis data tunggal. Ia adalah sebuah kemitraan—kerja sama antar lembaga—yang beroperasi berdasarkan seperangkat aturan dan kesepakatan bersama. Mari kita uraikan komponennya:

| Komponen | Penjelasan |
|----------|------------|
| Kemitraan antar lembaga | Beberapa lembaga bekerja bersama, bukan sendiri-sendiri |
| Aturan dasar (ground rules) | Pedoman bersama yang mengatur cara data digunakan dan dibagikan |
| Kesepakatan (agreements) | Komitmen formal yang mengikat para mitra |
| Tujuan bersama | Meningkatkan kehidupan anak dan keluarga |

Poin pentingnya: kekuatan IDS terletak pada kesepakatan, bukan hanya pada teknologi. Aturan dan kesepakatan inilah yang menjaga kepercayaan sekaligus memastikan data digunakan untuk kebaikan bersama.

### Siapa yang Mengembangkan IDS?

IDS dikembangkan oleh koalisi lembaga pemerintah, organisasi nirlaba, dan akademisi yang menyadari bahwa data yang tersebar adalah hambatan besar untuk melayani masyarakat. Di Amerika Serikat, misalnya, beberapa negara bagian telah mengimplementasikan IDS untuk melayani anak-anak dan keluarga dengan kebutuhan khusus.

**Contoh 1**: Di Negara Bagian X, lembaga pendidikan, kesehatan, dan layanan sosial sepakat berbagi data melalui IDS. Mereka menandatangani memorandum of understanding (MoU) yang mengatur:

**Langkah 1** — Definisi data yang boleh dibagikan: data demografis, riwayat layanan, outcome program. Data sensitif seperti diagnosis medis tidak dibagikan.

**Langkah 2** — Mekanisme berbagi: data disimpan di server terpusat dengan enkripsi end-to-end. Akses diberikan berdasarkan role (pendidikan, kesehatan, sosial).

**Langkah 3** — Monitoring: audit log mencatat setiap akses data. Pelanggaran dikenakan sanksi.

Hasilnya: lembaga-lembaga ini bisa melihat gambaran utuh tentang anak dan keluarga, sehingga intervensi lebih tepat sasaran.

### Catatan Penting dan Kesalahan Umum

> **Jangan anggap IDS adalah solusi teknologi semata**. Keberhasilan IDS bergantung pada governance dan trust, bukan hanya software. Tanpa kesepakatan yang jelas, lembaga tidak akan mau berbagi data.

> **Hati-hati dengan privasi**. Meskipun IDS dirancang untuk melindungi privasi, risiko penyalahgunaan data tetap ada. Pastikan ada mekanisme audit dan sanksi yang kuat.

> **Peringatan**: IDS bukan pengganti koordinasi manusia. Teknologi memfasilitasi berbagi data, tetapi keputusan tetap harus dibuat oleh manusia yang memahami konteks.

### Rangkuman Komponen IDS

| Aspek | Penjelasan |
|-------|------------|
| Tujuan | Meningkatkan kehidupan anak dan keluarga melalui berbagi data yang aman |
| Komponen utama | Kemitraan, ground rules, agreements, tujuan bersama |
| Prinsip kunci | Keamanan, privasi, governance, trust |
| Tantangan | Membangun trust antar lembaga, menjaga privasi, memastikan kepatuhan |

Intinya, IDS adalah kerja sama yang dibangun dengan hati-hati — bukan sekadar sistem teknis, melainkan kemitraan berbasis trust dan governance. Semangat belajar!
```

**Annotation**:
- ✅ Greeting + analogy: "Bayangkan jika lembaga-lembaga... bisa saling berbagi data"
- ✅ Motivation: implicit in "meningkatkan kehidupan anak-anak dan keluarga"
- ✅ Formal definition: "IDS, atau Integrated Data System..."
- ✅ Conditions: "Kata 'aman' di sini bukan sekadar tambahan—ia adalah fondasi"
- ✅ Explanation: 4 paragraphs with progressive disclosure
- ✅ Table: "Komponen | Penjelasan" (4 rows)
- ✅ Worked example: "Contoh 1" with 3 steps (Langkah 1, 2, 3)
- ✅ Verification: implicit in "Hasilnya: lembaga-lembaga ini bisa melihat gambaran utuh"
- ✅ "Catatan Penting dan Kesalahan Umum" with 3 pitfalls
- ✅ Summary table: "Rangkuman Komponen IDS"
- ✅ Conclusion: "Intinya, IDS adalah kerja sama yang dibangun dengan hati-hati..."
- ✅ Encouragement: "Semangat belajar!"
- ✅ Word count: ~900 words (fits 4.5-page section)

---

## Checklist for Detailed Sections

Before finalizing each section, verify:

- [ ] **Greeting + hook**: Starts with "Halo! Mari kita..." + analogy ("Bayangkan...")
- [ ] **Motivation**: Explains why this matters, bridges to next topic
- [ ] **Formal definition**: Precise, includes notation/formula if applicable
- [ ] **Conditions**: Explicit statement of prerequisites ("Syarat penting: ...")
- [ ] **Explanation**: 2–4 paragraphs with analogies and progressive disclosure
- [ ] **Table**: At least 1 table with 3–6 rows
- [ ] **Worked example**: "Contoh N: ..." with "Langkah 1 — ...", "Langkah 2 — ..."
- [ ] **Verification**: "Mari kita periksa satu per satu..."
- [ ] **Proof/derivation** (if applicable): Step-by-step with "Terbukti!"
- [ ] **Mnemonic**: Memory aid or pattern for recall
- [ ] **Pitfalls**: "Catatan Penting dan Kesalahan Umum" with 2–3 warnings
- [ ] **Summary table**: Consolidates rules/conditions
- [ ] **Conclusion**: Recap + encouragement + bridge to next section
- [ ] **Word count**: ~195 words per page (16–39 pages total = 3120–7605 words)

---

## Common Mistakes to Avoid

1. **Missing greeting**: Don't jump straight to definition. Start with "Halo! Mari kita..."
2. **No analogy**: Every section needs "Bayangkan..." or similar hook.
3. **Skipping conditions**: Always state prerequisites explicitly ("Syarat penting: ...").
4. **No worked example**: Detailed mode requires at least 1 worked example with steps.
5. **Missing verification**: After example, add "Mari kita periksa..."
6. **No pitfalls**: "Catatan Penting dan Kesalahan Umum" is mandatory.
7. **No summary table**: Every section needs a summary table at the end.
8. **Weak conclusion**: Don't just say "Selesai." Recap + encourage + bridge.
9. **Inconsistent voice**: Stick to "kita" primary, "kamu" secondary.
10. **Too short**: If section is <300 words, add more explanation, examples, or tables.

---

## When to Use Detailed Mode

**Use detailed when**:
- User is learning from scratch
- Source has complex procedures, proofs, or multi-step problems
- User asks for "tutorial" or "pembahasan lengkap"
- Topic requires worked examples with step-by-step breakdown
- User wants deep understanding, not just overview

**Don't use detailed when**:
- User wants quick review
- User already has context
- Source is straightforward (definitions only, no procedures)
- User asks for "ringkasan" or "summary"

In those cases, use **medium mode** instead.
