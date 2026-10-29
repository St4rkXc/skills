# Medium Pattern Reference

This document provides the complete template for **medium mode** study notes, with annotated examples from real generated notes.

---

## Template Overview

**Target**: 900–2800 words total (8–14 pages equivalent at ~160 words/page)

**Structure per section** (repeat for each major topic):
1. Section title + subtitle (question format)
2. Definition (1–2 paragraphs)
3. Comparison table (2–4 rows)
4. Bullet list (3–4 items)
5. Concrete example (1 brief)
6. Recap (1 sentence)
7. Source citation (if applicable)
8. Encouragement (optional)

---

## Full Section Template

```markdown
## [Topic Name]

### [Subtitle Question]?

[1–2 paragraph definition. Answer "what is it?" and "why does it matter?" directly. No preamble. Use em dash for apposition. Quote key terms + English in parens on first mention.]

[Optional: 1 more paragraph expanding on importance or context.]

| Aspek | Penjelasan |
|-------|------------|
| [Aspect 1] | [Explanation 1] |
| [Aspect 2] | [Explanation 2] |
| [Aspect 3] | [Explanation 3] |

[Bullet list of 3–4 key points:]

- [Point 1: characteristic, feature, or step]
- [Point 2: characteristic, feature, or step]
- [Point 3: characteristic, feature, or step]
- [Point 4: characteristic, feature, or step]

**Contoh**: [1 brief real-world example. Not a long worked problem. Just 1–2 sentences showing application.]

Intinya, [1-sentence recap summarizing the core takeaway].

[Optional: "Menurut [Author/Org] ([Year]), [concept]..."]

[Optional: "Semangat belajar!" or "Fondasi ini akan berguna di bab berikutnya."]
```

---

## Annotated Example 1: Business (CRM)

**Source**: Sistem Enterprise — Manajemen Hubungan Pelanggan (CRM)

**Analysis**:
- Domain: Business
- Key concepts: pemasaran, penjualan, layanan purna jual, CRM, SFA
- Examples in source: garansi, konsultasi, penanganan keluhan
- Source word count: ~1200 words → medium target: ~900 words

**Generated section**:

```markdown
## Konsep Layanan Purna Jual

### Pengertian Layanan Purna Jual

Halo! Mari kita bahas konsep dasar layanan purna jual. Secara sederhana, layanan purna jual (*after sales service*) adalah layanan yang diberikan perusahaan kepada pelanggan setelah penjualan terjadi. Menurut Philip Kotler (2002), layanan purna jual merupakan aktivitas yang dijalankan setelah produk dikirimkan kepada konsumen.

### Cakupan Aktivitas

Layanan ini mencakup berbagai kegiatan layanan pelanggan dan ikatan hubungan (*relationship ties*) yang bertujuan memastikan pelanggan merasa puas terhadap produk atau jasa organisasi.

| Aspek | Penjelasan |
|-------|------------|
| Waktu | Setelah produk dikirim ke konsumen |
| Bentuk | Layanan pelanggan dan ikatan hubungan |
| Tujuan | Memastikan kepuasan pelanggan |

**Contoh**: garansi perbaikan, layanan konsultasi penggunaan produk, dan penanganan keluhan pelanggan.

Intinya, layanan purna jual menjaga hubungan baik dan kepuasan setelah pembelian.

Semangat belajar!
```

**Annotation**:
- ✅ Greeting opener: "Halo! Mari kita bahas..."
- ✅ Definition direct to point (2 sentences)
- ✅ Source citation: "Menurut Philip Kotler (2002)..."
- ✅ Key term with English: "layanan purna jual (*after sales service*)"
- ✅ Table with 3 rows (Aspek | Penjelasan)
- ✅ Concrete example (1 sentence, real-world)
- ✅ Recap: "Intinya, ..."
- ✅ Encouragement: "Semangat belajar!"
- ✅ Word count: ~150 words (fits 1-page section)

---

## Annotated Example 2: Math (Relasi & Komposisi)

**Source**: Matematika Diskrit — Relasi dan Komposisi

**Analysis**:
- Domain: Math (Discrete)
- Key concepts: relasi biner, komposisi, relasi ekuivalen, poset, klosur
- Examples in source: komposisi relasi, pembuktian relasi ekuivalen
- Source word count: ~1600 words → medium target: ~1200 words

**Generated section**:

```markdown
## Komposisi Relasi: Definisi dan Konsep Dasar

### Apa Itu Komposisi Relasi?

Halo! Yuk kita pelajari komposisi relasi. Konsep ini mirip dengan "menyambung" dua perjalanan: dari titik awal ke titik tengah, lalu lanjut ke titik akhir.

### Definisi Formal

Misalkan R adalah relasi dari himpunan A ke himpunan B, dan S adalah relasi dari himpunan B ke himpunan C. Komposisi R dan S, dinotasikan S ∘ R, adalah relasi dari A ke C yang didefinisikan oleh:

S ∘ R = {(a, c) ∣ a ∈ A, c ∈ C, dan untuk beberapa b ∈ B, (a, b) ∈ R dan (b, c) ∈ S}

### Urutan Penerapan

Perhatikan urutannya dengan saksama:

1. Terapkan R terlebih dahulu — dari A ke B, menghasilkan pasangan (a, b).
2. Baru kemudian terapkan S — dari B ke C, menghasilkan pasangan (b, c).
3. Hasil akhirnya adalah pasangan (a, c) dari A ke C.

Meskipun R diterapkan lebih dulu, notasinya ditulis S ∘ R (dibaca "S setelah R"). Ini karena notasi dibaca dari kanan ke kiri, seperti fungsi komposisi.

| Komponen | Peran |
|----------|-------|
| A | Himpunan asal |
| B | Himpunan perantara |
| C | Himpunan tujuan |
| R | Relasi A → B |
| S | Relasi B → C |
| S∘R | Relasi A → C |

**Contoh**: Diberikan A = {1, 2, 3}, B = {2, 4, 6}, C = {s, t}. Jika R = {(1, 2), (2, 4)} dan S = {(2, t), (4, s)}, maka S ∘ R = {(1, t), (2, s)}.

Intinya, komposisi relasi menggabungkan dua relasi melalui elemen perantara.

Semangat belajar!
```

**Annotation**:
- ✅ Analogy hook: "mirip dengan 'menyambung' dua perjalanan"
- ✅ Formal definition with notation
- ✅ Numbered list for steps (1, 2, 3)
- ✅ Table with 6 rows (Komponen | Peran)
- ✅ Brief example (1 sentence with concrete sets)
- ✅ Recap + encouragement
- ✅ Word count: ~200 words (fits 1-page section)

---

## Annotated Example 3: CS (Sistem Operasi)

**Source**: Lecture slides on Process Management

**Analysis**:
- Domain: Computer Science
- Key concepts: process, thread, scheduling, context switch, PCB
- Examples in source: multitasking, time-sharing
- Source word count: ~1800 words → medium target: ~1400 words

**Generated section**:

```markdown
## Process vs. Thread

### Apa Perbedaan Process dan Thread?

Halo! Mari kita bedah dua konsep fundamental dalam sistem operasi: process dan thread. Keduanya sering dianggap sama, padahal berbeda mendasar—process adalah unit eksekusi independen dengan ruang memori sendiri, sedangkan thread adalah unit eksekusi ringan di dalam process yang berbagi memori.

### Process

Process adalah program yang sedang dieksekusi. Setiap process memiliki:

- **Ruang memori terpisah**: code, data, heap, stack milik sendiri
- **Resource terpisah**: file descriptor, socket, signal handler
- **PCB (Process Control Block)**: struktur data yang menyimpan state process (PID, register, program counter, status)
- **Overhead tinggi**: context switch antar-process mahal karena harus swap memori

| Aspek | Penjelasan |
|-------|------------|
| Definisi | Program yang sedang dieksekusi |
| Memori | Ruang memori independen |
| Komunikasi | IPC (Inter-Process Communication) diperlukan |
| Overhead | Tinggi (context switch lambat) |

**Contoh**: Saat kamu membuka browser, OS membuat process baru dengan PID unik. Browser punya memori sendiri, tidak bisa akses memori aplikasi lain langsung.

### Thread

Thread adalah unit eksekusi terkecil di dalam process. Satu process bisa punya banyak thread yang:

- **Berbagi memori**: code, data, heap milik process induk
- **Stack terpisah**: setiap thread punya stack sendiri untuk local variables
- **Context switch cepat**: karena berbagi memori, switch antar-thread lebih ringan
- **Komunikasi mudah**: thread dalam process yang sama bisa komunikasi via shared memory

| Aspek | Penjelasan |
|-------|------------|
| Definisi | Unit eksekusi terkecil dalam process |
| Memori | Berbagi dengan process induk |
| Komunikasi | Langsung via shared memory |
| Overhead | Rendah (context switch cepat) |

**Contoh**: Dalam aplikasi web server, setiap request ditangani oleh thread terpisah. Thread-thread ini berbagi code dan data server, tapi punya stack sendiri untuk local variables.

Intinya, process = isolasi + overhead tinggi; thread = sharing + overhead rendah.

Semangat belajar!
```

**Annotation**:
- ✅ Two sub-topics in one section (Process, Thread) with comparison
- ✅ Em dash for apposition: "process adalah...—process adalah..."
- ✅ Key term with explanation: "PCB (Process Control Block)"
- ✅ Two tables (one per sub-topic)
- ✅ Bullet lists with bold lead-ins
- ✅ Concrete examples (browser, web server)
- ✅ Recap with contrast: "process = isolasi + overhead tinggi; thread = sharing + overhead rendah"
- ✅ Word count: ~350 words (fits 2-page section)

---

## Checklist for Medium Sections

Before finalizing each section, verify:

- [ ] **Subtitle is a question**: "Apa Itu X?", "Mengapa X Krusial?", "Bagaimana X Bekerja?"
- [ ] **Definition is direct**: No "Pada bagian ini kita akan membahas..." preamble
- [ ] **Table present**: At least 1 table with 2–4 rows
- [ ] **Bullet list**: 3–4 items summarizing key points
- [ ] **Example is brief**: 1–2 sentences, real-world application
- [ ] **Recap sentence**: Starts with "Intinya, ..."
- [ ] **Encouragement**: Ends with "Semangat belajar!" or similar
- [ ] **Word count**: ~160 words per page (8–14 pages total = 1280–2240 words)

---

## Common Mistakes to Avoid

1. **Too much preamble**: Don't start with "Pada bagian ini kita akan membahas..." — go straight to definition.
2. **Missing table**: Every section needs a table. If source has no table, create one.
3. **Long examples**: Medium examples should be 1–2 sentences, not multi-step worked problems.
4. **No recap**: Always end with "Intinya, ..." sentence.
5. **Inconsistent voice**: Don't switch between "kita", "kamu", "Anda" randomly.
6. **Missing encouragement**: End with "Semangat belajar!" or "Selamat berlatih!"
7. **Too formal**: Use tutor voice, not academic tone. "Yuk, kita pelajari..." not "Pada sub-bab ini..."

---

## When to Use Medium Mode

**Use medium when**:
- User wants quick review before exam
- User already has context from lectures
- Source material is straightforward (definitions, concepts, no complex procedures)
- User asks for "ringkasan" or "summary"

**Don't use medium when**:
- User is learning from scratch
- Source has complex procedures, proofs, or multi-step problems
- User asks for "tutorial" or "pembahasan lengkap"
- Topic requires worked examples with step-by-step breakdown

In those cases, use **detailed mode** instead.
