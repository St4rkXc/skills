---
mode: detailed
pages: 37
words: 8118
---

pelajarin.ai

                                                                      1
Pengantar Matriks

Halo! Selamat datang di bab pertama tentang matriks. Materi ini adalah fondasi
penting yang akan kamu gunakan terus-menerus, terutama saat mempelajari
matematika diskrit, relasi, dan fungsi. Yuk, kita bedah pelan-pelan mulai dari definisi
paling dasar hingga jenis-jenis matriks khusus.

Apa Itu Matriks?
Secara sederhana, matriks adalah susunan skalar elemen-elemen dalam bentuk
baris dan kolom. Bayangkan seperti tabel atau grid angka yang tertata rapi. Setiap
angka di dalamnya disebut elemen atau skalar.

Sebuah matriks A yang berukuran m baris dan n kolom (ditulis m × n) memiliki bentuk

umum:

a11 a12 ⋯ a1n

        a21 a22 ⋯ a2n
A=

⋮⋮            ⋮

am1 am2 ⋯ amn

Di sini, indeks pertama (i) menunjukkan baris dan indeks kedua (j) menunjukkan
kolom. Jadi, aij adalah elemen yang terletak di baris ke-i dan kolom ke-j.

Notasi dan Ukuran Matriks

Dalam notasi ringkas, kita lazim menuliskan matriks dengan A = [aij ]. Cara ini jauh

lebih efisien daripada menuliskan seluruh elemen satu per satu.

Ukuran matriks ditentukan oleh jumlah baris dan kolomnya. Misalnya, matriks

berukuran 3 × 4 berarti memiliki 3 baris dan 4 kolom, sehingga total ada 12 elemen.

Perhatikan contoh berikut:

        2506
A= 8 7 5 4

        3118

2
Matriks di atas berukuran 3 × 4. Baris pertama berisi 2, 5, 0, 6, sedangkan kolom

pertama berisi 2, 8, 3. Memahami posisi baris dan kolom ini penting agar kamu tidak
tertukar saat melakukan operasi matriks nanti.

Matriks Bujursangkar

Matriks bujursangkar adalah matriks yang berukuran n × n, artinya jumlah barisnya
sama dengan jumlah kolomnya. Contohnya matriks 2 × 2, 3 × 3, atau 4 × 4.

Matriks bujursangkar punya peran istimewa karena memiliki diagonal utama — yaitu

elemen-elemen a11, a22, a33, … , ann yang membentang dari kiri atas ke kanan bawah.

Diagonal ini akan sering muncul di jenis-jenis matriks khusus berikutnya.

Matriks Simetri

Matriks simetri adalah matriks bujursangkar yang memenuhi syarat aij = aji untuk
setiap i dan j. Artinya, elemen di baris ke-i kolom ke-j sama dengan elemen di baris
ke-j kolom ke-i. Kalau kamu lipat matriks ini secara diagonal, kedua sisi akan saling

menutupi dengan rapi.

Contoh matriks simetri:

    2506

A=  5  8  7  4
    0  7  3  1

    6418

Coba perhatikan bahwa a12 = 5 dan a21 = 5, lalu a13 = 0 dan a31 = 0, dan seterusnya.

Itulah tanda matriks simetri.

Jenis-Jenis Matriks Khusus
Dalam pembahasan matematika, terdapat beberapa matriks khusus yang perlu kamu
kenali. Berikut rangkumannya:
1. Matriks Diagonal
Matriks diagonal adalah matriks bujursangkar yang semua elemennya bernilai nol,
kecuali elemen pada diagonal utamanya. Contohnya:

       3
                                                    100
                                            D= 0 2 0

                                                    003

Perhatikan bahwa semua elemen di luar diagonal utama adalah nol, sedangkan
diagonal utamanya berisi 1, 2, dan 3.
2. Matriks Identitas

Matriks identitas, dilambangkan dengan I, adalah matriks diagonal dengan semua

elemen diagonalnya bernilai 1. Matriks ini istimewa karena berperan seperti angka "1"

pada perkalian matriks. Contoh matriks identitas berukuran 3 × 3:

                                                    100
                                            I= 0 1 0

                                                    001

3. Matriks Segitiga Atas dan Segitiga Bawah
Matriks segitiga atas adalah matriks bujursangkar yang semua elemen di bawah
diagonal utamanya bernilai nol. Contohnya:

                                                    141
                                            U= 0 3 5

                                                    004

Sebaliknya, matriks segitiga bawah memiliki semua elemen di atas diagonal utama
bernilai nol:

                                                    200
                                            L= 6 4 0

                                                    241

4. Matriks Transpose

                                                                                4
Matriks transpose diperoleh dengan mempertukarkan baris dan kolom suatu matriks.
Baris pertama menjadi kolom pertama, baris kedua menjadi kolom kedua, dan

seterusnya. Transpose dari matriks A ditulis AT .

Sebagai ilustrasi, jika:

                 A  =  [1  2  3]  ,                   1  4
                        4  5  6      maka AT = 2         5
                                                         6
                                                      3

Hubungan penting: jika AT = A, maka A adalah matriks simetri. Jadi, konsep

transpose dan simetri saling berkaitan erat.

5. Matriks Zero-One (0/1)

Matriks zero-one, atau matriks biner, adalah matriks yang setiap elemennya hanya
bernilai 0 atau 1. Matriks jenis ini sangat berguna dalam matematika diskrit, khususnya
untuk merepresentasikan relasi, graf, dan jaringan. Contohnya:

                                      101
                              B= 0 1 0

                                      110

Ringkasan Cepat            Ciri Utama

  Jenis Matriks            Jumlah baris = jumlah kolom (n × n)
  Bujursangkar             aij = aji atau AT = A
  Simetri
  Diagonal                 Semua elemen nol kecuali diagonal utama
  Identitas                Diagonal utama bernilai 1, sisanya 0
  Segitiga atas            Elemen di bawah diagonal utama = 0

                                     5
Segitiga bawah  Elemen di atas diagonal utama = 0
Transpose
Zero-one        Baris dan kolom dipertukarkan (AT )

                Setiap elemen hanya 0 atau 1

Penutup

Selamat! Kamu sudah mengenal dasar-dasar matriks: definisi, notasi A = [aij ],
ukuran m × n, serta berbagai jenis matriks khusus. Pemahaman ini akan menjadi

bekal berharga saat kamu mempelajari operasi matriks, relasi, dan fungsi di bab-bab
berikutnya.

Jangan ragu untuk berlatih menuliskan matriks dan mengidentifikasi jenis-jenisnya.
Semakin sering kamu berlatih, semakin intuitif rasanya. Sampai jumpa di bab
berikutnya!

                6
Operasi Aritmetika Matriks

Halo! Pada catatan kali ini kita akan belajar tiga operasi dasar yang paling sering
dipakai saat bekerja dengan matriks, yaitu penjumlahan dua matriks, perkalian
matriks dengan skalar, dan perkalian dua matriks. Ketiganya punya aturan main
masing-masing, dan memahami syarat dimensinya adalah kunci supaya kita tidak
salah hitung. Yuk, kita bahas satu per satu dengan tenang dan menyeluruh.

Sebelum masuk ke operasi, ingat dulu bahwa matriks adalah susunan bilangan dalam
baris dan kolom. Ukuran (dimensi) matriks ditulis sebagai jumlah baris × jumlah

kolom, misalnya matriks berukuran 2 × 3 berarti punya 2 baris dan 3 kolom. Dalam

materi sumber juga dikenal istilah matriks 0/1 (zero-one), yaitu matriks yang seluruh
elemennya hanya bernilai 0 atau 1. Matriks jenis ini nanti sering muncul, misalnya saat
membahas relasi.

Secara umum, operasi yang biasa dilakukan terhadap matriks meliputi:

  • Operasi penjumlahan 2 buah matriks.

  • Operasi perkalian 2 buah matriks.

  • Operasi perkalian matriks dengan skalar.

Mari kita telaah ketiganya.

1. Penjumlahan Dua Matriks

Penjumlahan dua matriks dilakukan dengan menjumlahkan elemen-elemen yang

posisinya bersesuaian. Artinya, elemen pada baris ke-i kolom ke-j matriks pertama
dijumlahkan dengan elemen pada baris ke-i kolom ke-j matriks kedua.

Syarat penting: dua matriks hanya dapat dijumlahkan jika keduanya memiliki ukuran

(dimensi) yang sama. Matriks 2 × 3 hanya bisa dijumlahkan dengan matriks 2 × 3,
bukan dengan matriks 3 × 2.

Perhatikan contoh berikut. Kita jumlahkan dua matriks berukuran 3 × 3:

1 2 3 56 8     1+5 2+6 3+8          6 8 11

5 −3 5 + 7 2 7 = 5 + 7 −3 + 2 5 + 7 = 12 −1 12

4 −2 8 0 8 11  4 + 0 −2 + 8 8 + 11  4 6 19

               7
Lihat bagaimana setiap pasangan elemen yang seposisi dijumlahkan langsung? Itulah
inti dari operasi penjumlahan matriks — sederhana dan konsisten, selama ukurannya
cocok.

2. Perkalian Matriks dengan Skalar

Operasi ini melibatkan sebuah skalar (yaitu sebuah bilangan tunggal) yang dikalikan

dengan seluruh elemen matriks. Jika k adalah skalar dan A adalah matriks, maka kA
diperoleh dengan mengalikan setiap elemen A dengan k.

Sebagai contoh, misalkan

         1 02
A= 3 7 0 , k=3

        −2 0 4

Maka perkalian skalar 3A adalah:

3×1 3×0 3×2                          3 06

3A = 3 × 3 3 × 7 3 × 0 = 9 21 0

3 × (−2) 3 × 0 3 × 4                 −6 0 12

Perhatikan bahwa pada baris pertama hasilnya 3 × 1 = 3, 3 × 0 = 0, dan 3 × 2 = 6.

Pola yang sama berlaku untuk seluruh elemen. Tidak ada syarat khusus soal dimensi di
sini — skalar bisa dikalikan dengan matriks berukuran apa pun, karena setiap elemen
diperlakukan secara mandiri.

3. Perkalian Dua Matriks dan Syarat Dimensinya

Inilah operasi yang paling sering membuat bingung, jadi mari kita pelan-pelan. Dua
buah matriks dapat dikalikan jika jumlah kolom matriks pertama sama dengan
jumlah baris matriks kedua.

Jika matriks A berukuran m × n dan matriks B berukuran n × p, maka hasil perkalian
AB akan berukuran m × p. Perhatikan bahwa angka n (kolom A dan baris B) harus

sama — inilah syarat utamanya. Jika tidak sama, perkalian tidak dapat dilakukan
sama sekali.

                                  8
Cara menghitung elemen hasil: elemen pada baris ke-i kolom ke-j dari AB diperoleh
dengan mengalikan elemen-elemen baris ke-i matriks A dengan elemen-elemen
kolom ke-j matriks B, lalu menjumlahkan hasilnya (mirip seperti dot product).

Mari kita kerjakan contoh dari sumber. Diketahui:

                     A   =   [1  0  2]  ,          2  1
                              1  3  4      B= 4       3
                                                      5
                                                   6

Matriks A berukuran 2 × 3 dan B berukuran 3 × 2. Karena jumlah kolom A (3) sama
dengan jumlah baris B (3), perkalian valid dan hasilnya akan berukuran 2 × 2.

                     AB  =  [1   0  2]  2  1  =  [14     11]
                             1   3  4   4  3      26     30
                                        6  5

Mari kita periksa satu per satu elemennya agar makin paham.

  • Elemen baris 1, kolom 1: 1 × 2 + 0 × 4 + 2 × 6 = 2 + 0 + 12 = 14.
  • Elemen baris 1, kolom 2: 1 × 1 + 0 × 3 + 2 × 5 = 1 + 0 + 10 = 11.
  • Elemen baris 2, kolom 1: 1 × 2 + 3 × 4 + 4 × 6 = 2 + 12 + 24 = 26.
  • Elemen baris 2, kolom 2: 1 × 1 + 3 × 3 + 4 × 5 = 1 + 9 + 20 = 30.
Hasil akhirnya memang 2 × 2, sesuai prediksi dimensi m × p.

Rangkuman Syarat Tiap Operasi

Supaya mudah diingat, berikut tabel ringkasannya.

Operasi              Syarat                              Contoh Ukuran Valid

Penjumlahan A + B    Dimensi A dan B harus sama          2 × 3 dengan 2 × 3

Perkalian skalar kA  Tidak ada syarat khusus             k dengan matriks apa pun

Perkalian A × B      Kolom A sama dengan baris B         2 × 3 dikali 3 × 2

                                        9
Catatan Penting dan Kesalahan Umum
  • Jangan tertukar urutan. Perkalian matriks umumnya tidak komutatif, artinya AB
    belum tentu sama dengan BA. Bahkan, bisa jadi AB dapat dihitung tetapi BA

    justru tidak bisa karena syarat dimensi tidak terpenuhi. Selalu periksa dimensi
    sebelum menghitung.

  • Perhatikan dimensi hasil. Perkalian m × n dengan n × p menghasilkan matriks
    m × p. Kebiasaan memprediksi ukuran hasil ini sangat membantu untuk mengecek

    apakah perhitungan kita masuk akal.
  • Penjumlahan bersifat elemen-per-elemen, sedangkan perkalian matriks

    melibatkan kombinasi baris-kolom. Keduanya adalah dua hal yang berbeda,
    jangan dicampur.

Kaitan dengan Materi Berikutnya

Matriks erat kaitannya dengan konsep relasi. Dalam pembahasan relasi, kita
menghubungkan anggota dua himpunan menggunakan pasangan terurut (ordered

pairs) (a, b) dengan a ∈ A dan b ∈ B. Relasi biner R antara himpunan A dan B
adalah himpunan bagian dari A × B, ditulis R ⊆ (A × B). Himpunan A disebut
daerah asal (domain) dan himpunan B disebut daerah tujuan (kodomain).

Relasi semacam ini, terutama untuk relasi pada matriks 0/1, sering direpresentasikan
dengan matriks dan operasinya berkaitan erat dengan perkalian matriks — itulah
mengapa operasi aritmetika matriks penting untuk dikuasai lebih dulu. Tapi untuk
sekarang, pastikan dulu kamu nyaman dengan penjumlahan, perkalian skalar, dan
perkalian matriks. Latihan sedikit setiap hari akan membuat semuanya terasa alami.
Semangat belajar!

                                                                               10
Definisi dan Contoh Relasi Biner

Definisi Relasi Biner

Halo! Selamat datang di bab yang sangat penting dalam matematika diskrit. Di sini
kita akan membahas salah satu konsep paling fundamental, yaitu relasi biner. Konsep
ini menjadi dasar bagi banyak topik lanjutan, jadi mari kita pelajari dengan santai
namun menyeluruh.
Secara intuitif, relasi biner adalah aturan yang menghubungkan elemen-elemen dari
dua himpunan. Misalnya, relasi "mahasiswa mengambil mata kuliah" menghubungkan
himpunan mahasiswa dengan himpunan mata kuliah. Mari kita formalisasikan
gagasan ini.

Definisi formal: Misalkan A dan B adalah dua himpunan. Relasi biner R dari A ke B
adalah himpunan bagian dari hasil kali Kartesius A × B. Dengan kata lain, R ⊆ A × B.
Setiap elemen R berbentuk pasangan terurut (a, b) dengan a ∈ A dan b ∈ B.

Notasi, Domain, dan Kodomain
Ketika (a, b) merupakan anggota relasi R, kita menuliskan beberapa notasi yang

ekuivalen:

  • (a, b) ∈ R
  • a R b (dibaca "a berelasi dengan b")
Sebaliknya, jika (a, b) bukan anggota R, kita menulis (a, b) ∈/ R atau a R b.

Dua istilah penting yang wajib kamu kuasai:

  • Domain (daerah asal) adalah himpunan A, yaitu himpunan semua elemen

    pertama dari pasangan terurut.

  • Kodomain (daerah tujuan) adalah himpunan B, yaitu himpunan semua elemen

    kedua.

Contoh 1: Mahasiswa dan Mata Kuliah
Misalkan A = {Amir, Budi, Cecep} dan B = {IF221, IF251, IF342, IF323}.
Hasil kali Kartesius A × B terdiri atas 3 × 4 = 12 pasangan terurut, yaitu:

A × B = {(Amir, IF221), (Amir, IF251), (Amir, IF342), (Amir, IF323), (Budi, IF221), … , (Cec

                                                                                11
Sekarang, misalkan R adalah relasi yang menyatakan mata kuliah yang diambil oleh

mahasiswa pada semester ganjil:

R = {(Amir, IF251), (Amir, IF323), (Budi, IF221), (Budi, IF251), (Cecep, IF323)}

Perhatikan bahwa R ⊆ A × B. Himpunan A adalah domain, dan B adalah kodomain.

Sebagai ilustrasi notasi:

  • (Amir, IF251) ∈ R, sehingga kita boleh menulis Amir R IF251.
  • (Amir, IF342) ∈/ R, sehingga Amir R IF342.

Contoh 2: Relasi "Habis Membagi"
Misalkan P = {2, 3, 4} dan Q = {2, 4, 8, 9, 15}. Kita definisikan relasi R dari P ke Q

dengan aturan:

                          (p, q) ∈ R jika p habis membagi q

Artinya, p habis membagi q apabila q dibagi p tidak bersisa. Mari kita periksa satu per

satu:

p                q yang habis dibagi p      Pasangan

2                2, 4, 8                    (2, 2), (2, 4), (2, 8)

3                9, 15                      (3, 9), (3, 15)

4                4, 8                       (4, 4), (4, 8)

Maka diperoleh:

                 R = {(2, 2), (2, 4), (4, 4), (2, 8), (4, 8), (3, 9), (3, 15)}

                                        12
Relasi pada Sebuah Himpunan

Ada kasus khusus yang sangat sering muncul: ketika relasi menghubungkan sebuah
himpunan dengan dirinya sendiri. Ini disebut relasi pada himpunan.

Definisi: Relasi pada himpunan A adalah himpunan bagian dari A × A. Notasinya
R ⊆ A × A.

Contoh 5: Faktor Prima

Misalkan A = {2, 3, 4, 8, 9} dan relasi R pada A didefinisikan oleh (x, y) ∈ R jika x
adalah faktor prima dari y.
Mari kita periksa untuk setiap y:

  • y = 2: faktor primanya 2 → (2, 2)
  • y = 3: faktor primanya 3 → (3, 3)
  • y = 4: faktor primanya 2 → (2, 4)
  • y = 8: faktor primanya 2 → (2, 8)
  • y = 9: faktor primanya 3 → (3, 9)

Sehingga:

                              R = {(2, 2), (2, 4), (2, 8), (3, 3), (3, 9)}

Contoh 3: Relasi Mahasiswa dan Nilai

Sebagai gambaran tambahan, bayangkan relasi dari himpunan mahasiswa ke

himpunan nilai {A, B, C, D, E}. Jika Andi mendapat nilai A dan Budi mendapat nilai B,
maka pasangan (Andi, A) dan (Budi, B) menjadi anggota relasi tersebut. Ini

menunjukkan bahwa relasi biner dapat memodelkan banyak situasi nyata.

Cara Merepresentasikan Relasi

Selain ditulis sebagai himpunan pasangan terurut, relasi dapat divisualisasikan
dengan beberapa cara:

  1. Diagram Panah — Dua lingkaran mewakili domain (kiri) dan kodomain (kanan).

    Sebuah panah ditarik dari a ke b jika (a, b) ∈ R.

 2. Tabel — Kolom pertama menyatakan domain, kolom kedua menyatakan kodomain.

                                                                               13
 3. Matriks — Jika A = {a1, … , am} dan B = {b1, … , bn}, relasi disajikan sebagai
    matriks M = [mij ] berukuran m × n.

 4. Graf Berarah (Digraph) — Khusus untuk relasi pada sebuah himpunan. Tiap elemen

    digambarkan sebagai simpul, dan tiap pasangan terurut (a, b) ∈ R digambarkan
    sebagai busur dari a ke b. Perlu dicatat, graf berarah tidak digunakan untuk relasi

    antar dua himpunan berbeda.

Ringkasan Konsep Kunci
  • Relasi biner dari A ke B adalah R ⊆ A × B.
  • Notasi a R b setara dengan (a, b) ∈ R.
  • Domain = A, kodomain = B.
  • Relasi pada himpunan A berarti R ⊆ A × A.

  • Relasi dapat direpresentasikan lewat diagram panah, tabel, matriks, atau graf
    berarah.

Dengan memahami definisi dan contoh-contoh di atas, kamu sudah memiliki fondasi
kuat untuk mempelajari sifat-sifat relasi seperti refleksif, simetris, dan transitif pada
bab berikutnya. Selamat belajar, dan jangan ragu untuk berlatih membuat relasi
sendiri dari himpunan-himpunan di sekitarmu!

                                                                               14
Representasi Relasi

Representasi Relasi Biner

Halo! Setelah kita memahami apa itu relasi biner, pertanyaan berikutnya adalah:
bagaimana cara menuliskannya agar mudah dibaca dan dianalisis? Ada empat cara
utama yang akan kita pelajari, yaitu diagram panah, tabel, matriks, dan graf berarah.
Setiap cara punya kelebihan masing-masing, dan memilih representasi yang tepat
bisa sangat membantu ketika kita memeriksa sifat-sifat relasi.

1. Representasi Relasi dengan Diagram Panah
Diagram panah adalah cara paling visual. Kita gambar dua kelompok simpul

(himpunan asal dan himpunan tujuan), lalu tarik panah dari elemen a ke elemen b
untuk setiap pasangan terurut (a, b) yang menjadi anggota relasi.

  • Jika himpunan asal dan tujuan sama (relasi pada satu himpunan), kita cukup
    menggambar satu kelompok simpul.

  • Pasangan (a, b) digambarkan sebagai panah dari a menuju b.
  • Pasangan (a, a) digambarkan sebagai gelang atau kalang (loop), yaitu panah

    yang keluar dari simpul a dan kembali ke simpul a itu sendiri.

Diagram panah sangat intuitif untuk himpunan berukuran kecil, tetapi menjadi
berantakan jika anggotanya banyak.

2. Representasi Relasi dengan Tabel
Representasi tabel menyusun relasi dalam bentuk baris dan kolom. Cara paling umum
adalah tabel keanggotaan dengan:

  • Baris mewakili elemen pertama dari pasangan (domain).
  • Kolom mewakili elemen kedua (kodomain).
  • Sel diisi nilai 1 jika pasangan tersebut ada dalam relasi, dan 0 jika tidak.

Selain itu, relasi juga bisa ditampilkan sebagai tabel dua kolom sederhana yang

mendaftar setiap pasangan (a, b). Tabel dua kolom ini berguna untuk melihat relasi

baris per baris, misalnya saat memeriksa apakah sifat menghantar terpenuhi.

3. Representasi Relasi dengan Matriks

Jika himpunan A = {a1, a2, … , an}, relasi pada A dapat dinyatakan sebagai matriks
n × n (matriks berukuran n kali n), sebut saja M , dengan aturan:

                                                                               15
mij = {1,      jika (ai, aj) ∈ R
           0,  jika (ai, aj) ∈/ R

Beberapa catatan penting:

  • Elemen diagonal utama mii bernilai 1 jika (ai, ai) ∈ R. Inilah dasar pemeriksaan

    sifat refleksif: relasi bersifat refleksif jika dan hanya jika semua elemen diagonal

    utamanya bernilai 1, yaitu mii = 1 untuk i = 1, 2, … , n.

  • Matriks ini disebut matriks Boolean karena hanya berisi 0 dan 1.

  • Kelebihan matriks adalah mudah diolah secara komputasional, misalnya untuk
    mencari komposisi relasi.

4. Representasi Relasi dengan Graf Berarah (Digraph)
Graf berarah (directed graph atau disingkat digraph) adalah representasi yang
menggabungkan kekuatan diagram panah dengan struktur graf. Aturannya:

  • Setiap elemen himpunan digambarkan sebagai simpul (vertex).

  • Setiap pasangan terurut (a, b) ∈ R digambarkan sebagai busur berarah dari
    simpul a ke simpul b.

  • Simpul a disebut simpul asal (initial vertex) dan simpul b disebut simpul tujuan

    (terminal vertex).

  • Pasangan (a, a) dinyatakan dengan busur dari simpul a ke dirinya sendiri. Busur

    semacam ini disebut gelang atau kalang (loop).

Graf berarah dari relasi yang bersifat refleksif dicirikan oleh adanya gelang pada
setiap simpulnya.

Contoh Lengkap Representasi Relasi
Mari kita lihat sebuah contoh agar keempat representasi di atas terasa nyata. Misalkan

R = {(a, a), (a, b), (b, a), (b, c), (b, d), (c, a), (c, d), (d, b)} adalah relasi pada
himpunan {a, b, c, d}.
Sebagai graf berarah, relasi ini digambarkan dengan empat simpul a, b, c, d:

  • Gelang pada a (karena ada (a, a)).
  • Busur a → b dan b → a.

               16
  • Busur b → c dan b → d.
  • Busur c → a dan c → d.
  • Busur d → b.
Matriksnya berukuran 4 × 4 dengan baris dan kolom berurutan a, b, c, d:

   a  b      c  d

a  1  1      0  0

b  1  0      1  1

c  1  0      0  1

d  0  1      0  0

Dari matriks ini kita langsung bisa membaca bahwa relasi tersebut tidak refleksif,

karena elemen diagonal untuk b, c, dan d bernilai 0 (hanya (a, a) yang ada).

Mengapa Representasi Ini Penting?
Keempat representasi saling melengkapi dan membantu kita memeriksa sifat-sifat
relasi biner, seperti:

  • Refleksif — relasi R pada himpunan A disebut refleksif jika (a, a) ∈ R untuk setiap
    a ∈ A. Relasi tidak refleksif jika ada a ∈ A sedemikian sehingga (a, a) ∈/ R. Pada

    matriks, ini tampak dari diagonal utama yang semuanya bernilai 1; pada graf
    berarah, tampak dari gelang di setiap simpul.

  • Menghantar (transitif) — relasi R disebut menghantar jika setiap kali (a, b) ∈ R
    dan (b, c) ∈ R, maka berlaku (a, c) ∈ R untuk a, b, c ∈ A.

Mari kita lihat beberapa contoh sifat menghantar pada A = {1, 2, 3, 4}:

  • R = {(2, 1), (3, 1), (3, 2), (4, 1), (4, 2), (4, 3)} bersifat menghantar.

  • R = {(1, 1), (2, 3), (2, 4), (4, 2)} tidak menghantar karena (2, 4) ∈ R dan (4, 2) ∈
    R, tetapi (2, 2) ∈/ R; begitu juga (4, 2) dan (2, 3) ∈ R, tetapi (4, 3) ∈/ R.

  • R = {(1, 1), (2, 2), (3, 3), (4, 4)} jelas menghantar.

         17
  • R = {(1, 2), (3, 4)} menghantar, sebab tidak ada pasangan (a, b) ∈ R dan
    (b, c) ∈ R yang membuat syaratnya gagal. Relasi yang hanya berisi satu elemen,
    seperti R = {(4, 5)}, juga selalu menghantar.

Sebagai catatan tambahan, relasi "habis membagi" pada himpunan bilangan bulat
positif bersifat refleksif, karena setiap bilangan bulat positif habis dibagi oleh dirinya

sendiri, sehingga (a, a) ∈ R untuk setiap a. Sebaliknya, relasi seperti "x lebih besar dari
y", "x + y = 5", dan "3x + y = 10" pada bilangan bulat positif tidak refleksif, karena
misalnya (2, 2) bukan anggota dari ketiganya.

Rangkuman Cepat

Representasi  Bentuk                      Kelebihan

Diagram       Simpul dan panah            Paling visual untuk himpunan kecil
panah

Tabel         Baris dan kolom berisi      Mudah dibaca per pasangan
Matriks       0/1                         Mudah diolah secara komputasional

              Matriks Boolean n × n

Graf berarah  Simpul dan busur            Menampilkan struktur sekaligus sifat
                                          refleksif

Dengan menguasai keempat representasi ini, kamu akan lebih mudah menganalisis
relasi dan memeriksa sifat-sifatnya. Selamat belajar, dan jangan ragu berlatih
menggambar graf berarah dari berbagai relasi — semakin sering, semakin cepat
kamu mengenali polanya!

                                      18
Sifat-sifat Relasi Biner

Halo! Pada catatan kali ini kita akan menjelajahi empat sifat penting yang dimiliki
sebuah relasi biner: refleksif, menghantar (transitive), setangkup (symmetric), dan
tolak setangkup (antisymmetric). Kita juga akan melihat bagaimana sifat-sifat ini
tampak pada matriks representasi dan graf berarah. Yuk, kita mulai!

Relasi Menghantar (Transitive)
Sebuah relasi disebut menghantar jika setiap kali ada pasangan (a, b) dan (b, c) di
dalam relasi, maka pasangan (a, c) juga harus ada di dalam relasi. Dengan kata lain,
relasi ini "merambat" dari a ke c melalui b.

Contoh klasik yang sangat bagus adalah relasi "habis membagi" pada himpunan
bilangan bulat positif. Mari kita buktikan mengapa relasi ini menghantar.

Misalkan a habis membagi b dan b habis membagi c. Maka terdapat bilangan positif m
dan n sedemikian sehingga:

                                        b = ma dan c = nb

Substitusikan b ke persamaan c, kita peroleh:

                                         c = n(ma) = (nm)a

Karena nm adalah bilangan bulat positif, maka a habis membagi c. Jadi, relasi "habis

membagi" terbukti menghantar. Keren, bukan?
Contoh Relasi Menghantar dan Tidak Menghantar

Perhatikan tiga relasi berikut pada himpunan bilangan bulat positif N:
  • R : x lebih besar dari y. Relasi ini menghantar karena jika x > y dan y > z, maka
    pasti x > z.
  • S : x + y = 6. Relasi ini tidak menghantar. Sebagai contoh, (4, 2) dan (2, 4) adalah
    anggota S, tetapi (4, 4) bukan anggota S karena 4 + 4 = 8 = 6.
  • T = {(1, 7), (2, 4), (3, 1)}. Relasi ini tidak menghantar.

                                                                               19
Ciri Relasi Menghantar pada Matriks dan Graf
Menariknya, relasi yang bersifat menghantar tidak mempunyai ciri khusus pada
matriks representasinya. Jadi kita tidak bisa langsung menebak sifat menghantar
hanya dengan melihat pola matriksnya.
Namun, pada graf berarah, sifat menghantar punya ciri yang jelas: jika ada busur

berarah dari a ke b dan dari b ke c, maka harus juga terdapat busur berarah dari a ke c.

Relasi Setangkup (Symmetric)
Relasi R pada himpunan A disebut setangkup jika untuk setiap (a, b) ∈ R, maka
(b, a) ∈ R untuk semua a, b ∈ A. Sederhananya, arah relasi bisa dibolak-balik.
Sebaliknya, relasi tidak setangkup jika terdapat (a, b) ∈ R tetapi (b, a) ∈/ R.

Contoh Relasi Setangkup

Misalkan A = {1, 2, 3, 4}. Perhatikan relasi:

                      R = {(1, 1), (1, 2), (2, 1), (2, 2), (2, 4), (4, 2), (4, 4)}

Relasi ini setangkup karena jika (a, b) ∈ R maka (b, a) juga ∈ R. Perhatikan bahwa
(1, 2) dan (2, 1) keduanya ada, begitu juga (2, 4) dan (4, 2).
Sebagai perbandingan, relasi R = {(1, 1), (2, 3), (2, 4), (4, 2)} tidak setangkup karena
(2, 3) ∈ R, tetapi (3, 2) ∈/ R.

Relasi Tolak Setangkup (Antisymmetric)
Relasi R pada himpunan A disebut tolak setangkup jika untuk semua a, b ∈ A, kondisi
(a, b) ∈ R dan (b, a) ∈ R hanya terpenuhi jika a = b.

Dengan kata lain, jika dua elemen berbeda memiliki relasi dua arah, maka relasi
tersebut tidak tolak setangkup. Secara formal: relasi tidak tolak setangkup jika ada

elemen berbeda a dan b sedemikian sehingga (a, b) ∈ R dan (b, a) ∈ R.

Contoh Relasi Tolak Setangkup

Kembali pada A = {1, 2, 3, 4}:
  • R = {(1, 1), (2, 2), (3, 3)} bersifat tolak setangkup karena satu-satunya pasangan
    yang "bolak-balik" adalah pasangan dengan elemen yang sama (1 = 1, 2 = 2, 3 =
    3). Menariknya, relasi ini juga setangkup!

                                                                               20
• R = {(1, 1), (1, 2), (2, 2), (2, 3)} bersifat tolak setangkup karena (1, 1) ∈ R dengan
 1 = 1, dan (2, 2) ∈ R dengan 2 = 2. Namun relasi ini tidak setangkup karena
 (1, 2) ∈ R tetapi (2, 1) ∈/ R, dan (2, 3) ∈ R tetapi (3, 2) ∈/ R.

• R = {(1, 1), (2, 4), (3, 3), (4, 2)} tidak tolak setangkup karena 2 = 4 tetapi (2, 4)
 dan (4, 2) keduanya anggota R.

• R = {(1, 1), (2, 2), (2, 3), (3, 2), (4, 2), (4, 4)} tidak setangkup dan tidak tolak

  setangkup.

Hubungan Tidak Setangkup dan Tolak Setangkup

Ini bagian yang sering membingungkan, jadi perhatikan baik-baik ya!
Tidak setangkup dan tolak setangkup adalah dua hal yang berbeda, bukan kebalikan
satu sama lain. Sebuah relasi bisa jadi:

  • Setangkup sekaligus tolak setangkup: hanya jika semua pasangannya berbentuk

    (a, a), seperti {(1, 1), (2, 2), (3, 3)}.
  • Setangkup tetapi tidak tolak setangkup: seperti relasi yang memiliki (2, 4) dan

    (4, 2) dengan 2 = 4.
  • Tolak setangkup tetapi tidak setangkup: seperti {(1, 1), (1, 2), (2, 2), (2, 3)}.

  • Tidak keduanya: relasi yang memiliki beberapa pasangan "bolak-balik" dengan
    elemen berbeda, tetapi juga memiliki pasangan satu arah yang tidak lengkap.

Sifat            Definisi Inti

Menghantar       (a, b), (b, c) ∈ R ⇒ (a, c) ∈ R

Setangkup        (a, b) ∈ R ⇒ (b, a) ∈ R

Tolak setangkup  (a, b), (b, a) ∈ R ⇒ a = b

Menentukan Sifat Relasi dari Matriks dan Graf Berarah

Saat menghadapi soal, kita bisa menentukan sifat relasi dengan dua alat bantu:
Dari matriks representasi:

  • Setangkup: matriksnya simetris terhadap diagonal utama. Jika entri mij = 1, maka
    mji = 1.

                 21
  • Tolak setangkup: untuk i = j, tidak boleh mij = 1 dan mji = 1 secara bersamaan.

    Diagonal utama bebas.
  • Menghantar: tidak ada ciri khusus pada matriks, jadi harus diperiksa pasangan

    demi pasangan.
Dari graf berarah:

  • Menghantar: jika ada busur a → b dan b → c, maka harus ada busur a → c.
  • Setangkup: setiap busur a → b harus disertai busur balik b → a.

  • Tolak setangkup: tidak boleh ada dua busur berlawanan arah antara dua simpul
    berbeda.

Penutup

Empat sifat ini — menghantar, setangkup, dan tolak setangkup (plus refleksif) — adalah
fondasi penting dalam memahami relasi biner. Kuncinya adalah selalu memeriksa
definisi dengan teliti, lalu memanfaatkan ciri matriks atau graf untuk mempercepat
analisis. Jangan tertukar antara "tidak setangkup" dan "tolak setangkup" ya —
keduanya berbeda! Selamat belajar, dan teruslah berlatih dengan contoh-contoh
baru.

                                                                               22
Contoh Analisis Sifat Relasi

Analisis Sifat Relasi: Refleksif, Menghantar, Setangkup, dan Tolak-
Setangkup

Halo! Di bab ini kita akan belajar bagaimana cara menentukan sifat-sifat sebuah
relasi. Alih-alih hanya menghafal definisi, kita akan langsung membedah beberapa
contoh nyata — mulai dari relasi berbasis rumus, relasi dari graf berarah, hingga relasi
dari matriks. Yuk, kita mulai!

Mengingat Kembali Empat Sifat Dasar
Sebelum masuk ke contoh, mari samakan persepsi tentang keempat sifat ini:

  • Refleksif: setiap elemen terhubung dengan dirinya sendiri, yaitu (a, a) ∈ R untuk
    semua a di himpunan.

  • Menghantar (transitif): jika (a, b) ∈ R dan (b, c) ∈ R, maka harus berlaku (a, c) ∈
    R.

  • Setangkup (simetris): jika (a, b) ∈ R, maka (b, a) ∈ R.
  • Tolak-setangkup (antisimetris): jika (a, b) ∈ R dan (b, a) ∈ R, maka harus a = b.

Kunci penting yang sering membuat mahasiswa bingung: "tidak setangkup" tidak
selalu berarti "tolak-setangkup"! Keduanya adalah sifat yang berbeda dan bisa saja
sebuah relasi tidak memiliki keduanya sama sekali, seperti yang akan kita lihat nanti.

Contoh 1: Relasi dengan Rumus R = {(x, y) ∣ x3 = y}

Misalkan x ∈ Z dan y ∈ Z. Kita uji satu per satu keempat sifatnya.
Refleksif? Tidak. Kita butuh (x, x) ∈ R, artinya x3 = x. Ini hanya benar untuk x =
−1, 0, 1. Untuk x = 2, kita punya 23 = 8 = 2, sehingga (2, 2) ∈/ R. Karena ada elemen

yang gagal, relasi ini tidak refleksif.

Menghantar? Tidak. Andaikan x3 = y dan y3 = z. Substitusi memberi z = (x3)3 = x9.
Untuk transitif, kita butuh x3 = z, yaitu x3 = x9 — yang jelas tidak berlaku umum. Jadi

relasi ini tidak menghantar.

Setangkup? Tidak. Ambil (2, 8) ∈ R karena 23 = 8. Namun (8, 2) ∈/ R karena 83 =
512 = 2. Jadi tidak setangkup.

                                                                               23
Tolak-setangkup? Ya. Jika x3 = y dan y3 = x keduanya berlaku, maka x9 = x, yang
hanya mungkin untuk x = y pada bilangan bulat. Karena itu, relasi ini tolak-

setangkup.

Contoh 2: Relasi "Habis Membagi" pada Bilangan Bulat Positif
Relasi "a habis membagi b" adalah contoh klasik yang sangat informatif.

  • Tidak setangkup: 2 habis membagi 4, tetapi 4 tidak habis membagi 2. Jadi (2, 4) ∈
    R namun (4, 2) ∈/ R.

  • Tolak-setangkup: jika a habis membagi b dan b habis membagi a, maka satu-
    satunya kemungkinan adalah a = b. Contohnya, 4 habis membagi 4, dan jelas 4 =
    4.

Perhatikan bahwa satu relasi bisa tidak setangkup sekaligus tolak-setangkup —
keduanya tidak saling meniadakan!

Contoh 3: Relasi yang "Tidak Keduanya"

Ambil R = {(1, 1), (2, 2), (2, 3), (3, 2), (4, 2), (4, 4)}.
  • Tidak setangkup karena (4, 2) ∈ R tetapi (2, 4) ∈/ R.
  • Tidak tolak-setangkup karena (2, 3) ∈ R dan (3, 2) ∈ R, tetapi 2 = 3.

Inilah bukti nyata bahwa sebuah relasi bisa gagal pada kedua sifat sekaligus. Jangan
pernah menyamakan keduanya!

Contoh 4: Tiga Relasi pada Bilangan Bulat Positif N

Tinjau R : x > y, S : x + y = 6, dan T : 3x + y = 10.

Relasi    Setangkup? Alasan         Tolak-           Alasan
                                    setangkup?

R : x > y Tidak  5 > 3 tetapi 3 >                   Jika x > y dan y > x,
                                                     mustahil kecuali x = y
                                                 Ya

                 5

S :x+     Ya     (4, 2) dan (2, 4)  Tidak            (4, 2) ∈ S dan
                 keduanya di S                       (2, 4) ∈ S tetapi 4 = 2
y=6

T : 3x +  Tidak  (3, 1) ∈ T tetapi  Ya               Jika 3x + y = 10 dan
y = 10                                               3y + x = 10, maka
                 (1, 3) ∈/ T                         x=y

                              24
Contoh ini menunjukkan bahwa setangkup dan tolak-setangkup bisa muncul dalam
kombinasi apa pun — bahkan sebuah relasi dapat memiliki keduanya, salah satu saja,
atau tidak keduanya.
Contoh 5: Analisis dari Graf Berarah

Misalkan graf merepresentasikan relasi R pada himpunan A = {1, 2, 3, 4, 5} dengan:

                  R = {(1, 1), (1, 2), (2, 1), (2, 3), (3, 3), (4, 3), (5, 4), (5, 5)}

  • Refleksif? Tidak, karena (2, 2) ∈/ R dan (4, 4) ∈/ R. Graf tidak memiliki loop di simpul

    2 dan 4.

  • Menghantar? Tidak, karena (1, 2) ∈ R dan (2, 3) ∈ R, tetapi (1, 3) ∈/ R. Perhatikan
    juga jalur (5, 4) → (4, 3) yang tidak "dilanjutkan" ke (5, 3).

  • Setangkup? Tidak, karena (2, 3) ∈ R tetapi (3, 2) ∈/ R (tidak ada panah balik).
  • Tolak-setangkup? Tidak, karena (1, 2) ∈ R dan (2, 1) ∈ R dengan 1 = 2. Ada

    panah dua arah antar simpul berbeda.
Cara Membaca Sifat dari Graf Berarah
Agar analisis dari graf jadi lebih cepat, gunakan panduan praktis ini:

  • Refleksif: cek apakah setiap simpul memiliki loop (panah menunjuk dirinya sendiri).
  • Menghantar: telusuri setiap jalur panjang dua langkah — pastikan selalu ada "jalan

    pintas" langsung dari simpul awal ke simpul akhir.

  • Setangkup: setiap panah dari a ke b harus punya pasangan panah balik dari b ke a.

  • Tolak-setangkup: tidak boleh ada dua panah berlawanan arah antar dua simpul
    yang berbeda.

Cara Membaca Sifat dari Matriks Representasi

Jika relasi disajikan sebagai matriks M berukuran n × n dengan entri 0/1, kita bisa

membacanya lewat pola berikut:

  • Refleksif: semua entri diagonal utama (Mii) harus bernilai 1.
  • Setangkup: matriks harus simetris terhadap diagonal, yaitu Mij = Mji untuk

    semua i, j.

                                                                               25
  • Tolak-setangkup: untuk setiap i = j, tidak boleh Mij = 1 dan Mji = 1 secara
    bersamaan. Dengan kata lain, jika Mij = 1 maka Mji = 0.

  • Menghantar: matriks kuadrat M 2 tidak boleh memiliki entri 1 di posisi yang bernilai 0
    di M — yakni, jika ada jalur panjang dua, harus ada jalur panjang satu.

Pendekatan matriks ini sangat berguna ketika himpunan relasinya besar dan lebih
efisien diperiksa secara komputasional.

Contoh 6: Relasi Kecil R = {(1, 2), (2, 3), (1, 3)}

Mari uji secara manual:

  • Tidak setangkup: (1, 2) ∈ R tetapi (2, 1) ∈/ R.
  • Tolak-setangkup: tidak ada satupun pasangan berlawanan arah (a, b) dan (b, a)

    dengan a = b. Karena tidak ada pasangan seperti itu, syarat tolak-setangkup

    terpenuhi secara otomatis (vacuously true).

Relasi kecil ini adalah contoh bagus untuk memahami perbedaan kedua konsep
secara konkret.

Latihan Menentukan Sifat Relasi
Cobalah tebak sifat-sifat relasi berikut tanpa melihat jawaban terlebih dahulu:

  1. R = {(1, 1), (1, 3), (3, 1), (3, 3)} pada {1, 2, 3}.
 2. R = {(a, b) ∣ a ≤ b} pada bilangan bulat.
 3. R = {(a, b) ∣ a ⋅ b > 0} pada bilangan bulat tak nol.

Petunjuk jawaban:

  1. Tidak refleksif (tidak ada (2, 2)), menghantar, setangkup, tidak tolak-setangkup
    karena (1, 3) dan (3, 1) dengan 1 = 3.

 2. Refleksif, menghantar, tidak setangkup (misalnya 2 ≤ 3 tetapi 3 ≤ 2), tolak-

    setangkup.

 3. Tidak refleksif jika 0 tak diikutsertakan pada himpunan positif — sesuaikan domain;
    setangkup dan menghantar; tidak tolak-setangkup karena (−2, 3) dan (3, −2)

    keduanya anggota.

Rangkuman Cepat
Analisis sifat relasi selalu berpijak pada definisi formal, tetapi alat bantu graf dan
matriks membuat pemeriksaan jauh lebih cepat. Ingat tiga jebakan tersering: (1)

                                                                               26
refleksif hanya butuh satu simpul gagal untuk gugur; (2) menghantar harus diperiksa
untuk semua jalur dua langkah; dan (3) setangkup berbeda dari tolak-setangkup —
keduanya bisa hadir bersama, salah satu saja, atau tidak keduanya. Dengan latihan
berulang, membaca sifat relasi akan menjadi refleks bagi kamu. Semangat!

                                                                               27
Relasi Inversi

Memahami Relasi Inversi

Halo, teman-teman! Setelah kita berkenalan dengan berbagai sifat relasi seperti
refleksif, setangkup, tolak-setangkup, dan menghantar, sekarang saatnya kita
mempelajari sesuatu yang baru namun sangat berkaitan erat: relasi inversi. Konsep ini
ibarat "membalik arah" sebuah relasi. Kalau sebelumnya kita bicara tentang pasangan

(a, b), kini kita akan bicara tentang pasangan (b, a). Menarik, bukan? Mari kita bedah

bersama-sama dengan santai tapi tetap teliti.

Definisi Relasi Invers
Misalkan R adalah relasi dari himpunan A ke himpunan B. Perhatikan kata "dari" dan
"ke" di sini — artinya arah relasi itu jelas, yaitu dari anggota A menuju anggota B.
Invers dari relasi R, yang dilambangkan dengan R−1, adalah relasi dari B ke A yang

didefinisikan oleh:

                                     R−1 = {(b, a) ∣ (a, b) ∈ R}

Mari kita baca definisi ini dengan cermat:

  • Setiap pasangan terurut (a, b) yang ada di dalam R akan menghasilkan pasangan
    terurut baru (b, a) yang masuk ke dalam R−1.

  • Jadi, kalau R memetakan dari A ke B, maka R−1 memetakan dari B ke A. Arahnya

    benar-benar dibalik.
  • Anggota-anggota yang terlibat tetap sama; hanya urutannya yang ditukar.

Dengan kata lain, untuk memperoleh R−1, kita cukup menukar posisi setiap pasangan
pada relasi R. Sesederhana itu! Tidak ada operasi rumit seperti perkalian atau

penjumlahan — hanya pertukaran urutan.

   Catatan penting: Jika R adalah relasi pada himpunan A (artinya domain dan
   kodomainnya sama, yaitu A ke A), maka R−1 juga merupakan relasi pada
   himpunan A itu sendiri. Inversi tidak mengubah himpunan dasarnya, hanya

   membalik arah pasangannya.

                                                                               28
Contoh: Invers Relasi "Habis Membagi"

Mari kita kerjakan sebuah contoh konkret agar pemahaman kita makin kokoh.
Misalkan:

  • P = {2, 3, 4}
  • Q = {2, 4, 8, 9, 15}
Kita definisikan relasi R dari P ke Q dengan aturan:

                              (p, q) ∈ R jika p habis membagi q

Maksud "habis membagi" di sini adalah q dibagi p menghasilkan bilangan bulat tanpa
sisa, atau dengan kata lain q adalah kelipatan dari p.
Sekarang kita periksa setiap anggota P terhadap setiap anggota Q:
Untuk p = 2:

  • 2 habis membagi 2 ✔ → (2, 2) ∈ R
  • 2 habis membagi 4 ✔ → (2, 4) ∈ R
  • 2 habis membagi 8 ✔ → (2, 8) ∈ R
  • 2 tidak habis membagi 9 ✘
  • 2 tidak habis membagi 15 ✘
Untuk p = 3:
  • 3 tidak habis membagi 2 ✘
  • 3 tidak habis membagi 4 ✘
  • 3 tidak habis membagi 8 ✘
  • 3 habis membagi 9 ✔ → (3, 9) ∈ R
  • 3 habis membagi 15 ✔ → (3, 15) ∈ R
Untuk p = 4:
  • 4 tidak habis membagi 2 ✘
  • 4 habis membagi 4 ✔ → (4, 4) ∈ R
  • 4 habis membagi 8 ✔ → (4, 8) ∈ R

                                                                               29
  • 4 tidak habis membagi 9 ✘
  • 4 tidak habis membagi 15 ✘
Maka relasi R secara lengkap adalah:

                     R = {(2, 2), (2, 4), (2, 8), (3, 9), (3, 15), (4, 4), (4, 8)}

Untuk memperoleh R−1, kita tinggal membalik setiap pasangan:

                    R−1 = {(2, 2), (4, 2), (8, 2), (9, 3), (15, 3), (4, 4), (8, 4)}

Perhatikan bahwa R−1 sekarang merupakan relasi dari Q ke P . Relasi ini dapat
dinyatakan dengan aturan: (q, p) ∈ R−1 jika q habis dibagi oleh p, atau setara dengan
"p habis membagi q" dari sudut pandang yang terbalik. Inilah keindahan relasi inversi —

ia menceritakan hubungan yang sama, tetapi dari perspektif arah yang berlawanan.

Matriks Representasi Relasi Invers

Nah, sekarang kita masuk ke bagian yang mungkin paling memuaskan secara
matematis. Sebelumnya kita telah mempelajari bahwa sebuah relasi pada himpunan
berhingga dapat direpresentasikan sebagai matriks berisi 0 dan 1, di mana:

  • mij = 1 jika (ai, aj ) ∈ R
  • mij = 0 jika (ai, aj ) ∈/ R
Bagaimana dengan matriks untuk R−1? Ada sebuah hubungan yang sangat elegan:

                                  Matriks(R−1) = [Matriks(R)]T

Matriks representasi relasi invers R−1 adalah transpose dari matriks relasi asal R.

Transpose matriks, seperti yang kita ketahui, adalah operasi menukar baris menjadi

kolom dan sebaliknya. Secara formal, jika M = [mij ] adalah matriks relasi R, maka
matriks relasi R−1 adalah N = [nij ] dengan:

                                                                               30
                 nij = mji

Ini masuk akal sekali! Karena pasangan (a, b) menjadi (b, a) pada relasi invers, maka
entri pada baris i kolom j bertukar posisi dengan entri pada baris j kolom i. Itulah

persis yang dilakukan transpose.

Ilustrasi Sederhana

Misalkan relasi R pada himpunan A = {1, 2, 3} memiliki matriks:

                            110
                 MR = 0 1 1

                            101

Maka matriks untuk R−1 adalah transpose-nya:

                                       101
                 MR−1 = MRT = 1 1 0

                                       011

Coba perhatikan entri m12 = 1 pada MR. Ini berarti (1, 2) ∈ R. Pada MR−1 , entri yang
bersesuaian adalah n21 = 1, yang berarti (2, 1) ∈ R−1. Benar sekali, bukan?

Tabel Ringkasan Konsep

Konsep           Penjelasan

R dari A ke B    Relasi dengan arah dari anggota A menuju anggota B

R−1              Relasi dari B ke A hasil pembalikan pasangan

Definisi formal  R−1 = {(b, a) ∣ (a, b) ∈ R}

Cara memperoleh  Tukar urutan setiap pasangan terurut pada R

                             31
Domain dan kodomain   Bertukar: domain R−1 = kodomain R, dan sebaliknya
Matriks representasi  Matriks R−1 = transpose matriks R
Hubungan entri        nij = mji untuk setiap i, j

Insight Tambahan: Kapan R−1 = R?

Ada satu pengamatan menarik yang layak kita renungkan. Kapan sebuah relasi

bersifat self-inverse, artinya R−1 = R? Jawabannya terjadi tepat ketika relasi tersebut
setangkup (simetris). Ingat, relasi setangkup berarti jika (a, b) ∈ R maka (b, a) ∈ R.

Nah, kondisi inilah yang membuat himpunan pasangannya tidak berubah saat dibalik,

sehingga R−1 = R.

Konsekuensinya, matriks suatu relasi setangkup akan selalu sama dengan
transposenya, yaitu matriks yang simetris terhadap diagonal utamanya. Hubungan ini

menjelaskan mengapa sifat setangkup tadi diuji dengan membandingkan mij dan
mji — kita sesungguhnya sedang membandingkan matriks relasi dengan

transposenya!

Rangkuman Akhir

Mari kita ikat semua yang sudah kita pelajari:

  • Relasi inversi R−1 mendefinisikan ulang relasi R dengan cara membalik arah
    setiap pasangan: dari (a, b) menjadi (b, a).

  • Secara formal, R−1 = {(b, a) ∣ (a, b) ∈ R}, dan ia merupakan relasi dari B ke A.
  • Untuk mendapatkan R−1, cukup tukar posisi setiap pasangan pada R; himpunan

    anggotanya tidak berubah.

  • Matriks relasi R−1 adalah transpose dari matriks relasi R, karena penukaran

    pasangan berkorespondensi langsung dengan penukaran baris dan kolom.

  • Relasi akan bersifat self-inverse (R−1 = R) jika dan hanya jika relasi itu setangkup.

Dengan memahami relasi inversi, kalian kini memiliki alat tambahan untuk
menganalisis relasi dari dua arah sekaligus. Konsep transpose matriks yang tadinya
terasa terpisah kini terhubung indah dengan dunia relasi. Teruslah berlatih membalik
pasangan dan menyusun matriksnya, karena semakin sering kalian melakukannya,
semakin intuitif konsep ini terasa. Selamat belajar, dan sampai jumpa di bab
berikutnya!

                      32
Mengkombinasikan Relasi

Mengapa Relasi Bisa "Dikombinasikan"?

Halo! Sebelum kita masuk ke operasi himpunan pada relasi, mari kita ingat satu fakta
penting: relasi biner pada dasarnya adalah himpunan pasangan terurut. Karena
setiap relasi adalah himpunan, maka semua operasi himpunan yang sudah kita kenal
— irisan, gabungan, selisih, dan beda setangkup — otomatis juga bisa diterapkan pada
relasi. Inilah ide kunci di balik topik "Mengkombinasikan Relasi".

Dengan kata lain, kita tidak perlu aturan baru yang rumit. Semua sifat himpunan yang
sudah kita pelajari tetap berlaku, hanya saja anggotanya kali ini berupa pasangan

terurut seperti (2, 4) atau (3, 9), bukan angka tunggal.

Definisi Formal: Operasi Himpunan pada Relasi
Misalkan R1 dan R2 masing-masing adalah relasi dari himpunan A ke himpunan B.

Maka keempat operasi berikut:

          R1 ∩ R2, R1 ∪ R2, R1 − R2, R1 ⊕ R2

semuanya juga merupakan relasi dari A ke B. Fakta ini penting dan akan kita bahas

lagi di bagian sifat tertutup.

Mari kita bedah arti masing-masing operasi, dengan (a, b) sebagai anggota

himpunan relasi:

Operasi   Notasi  Arti untuk pasangan (a, b)

Irisan    R1 ∩ R2 (a, b) ∈ R1 dan (a, b) ∈ R2

Gabungan  R1 ∪ R2 (a, b) ∈ R1 atau (a, b) ∈ R2 (atau keduanya)

Selisih   R1 − R2 (a, b) ∈ R1 tetapi (a, b) ∈/ R2

Beda Setangkup R1 ⊕ R2 (a, b) ada di tepat salah satu himpunan, tidak di keduanya

                  33
Perhatikan bahwa beda setangkup bisa dipandang sebagai gabungan dikurangi

irisan: R1 ⊕ R2 = (R1 ∪ R2) − (R1 ∩ R2).
Contoh Konkret
Agar lebih jelas, mari ambil relasi dari A = {1, 2, 3} ke B = {a, b}. Misalkan:

  • R1 = {(1, a), (2, b), (3, a)}
  • R2 = {(1, a), (2, a), (3, a)}

Sekarang kita hitung keempat operasinya:
Irisan — pasangan yang muncul di keduanya:

                                      R1 ∩ R2 = {(1, a), (3, a)}

Gabungan — semua pasangan dari keduanya (yang kembar ditulis sekali):

                             R1 ∪ R2 = {(1, a), (2, a), (2, b), (3, a)}

Selisih — milik R1 saja (buang yang ada di R2):

                                          R1 − R2 = {(2, b)}

Sebaliknya, R2 − R1 = {(2, a)}, sebab (2, a) ada di R2 tetapi tidak di R1.

Beda setangkup — pasangan yang hanya ada di salah satu:

                                      R1 ⊕ R2 = {(2, a), (2, b)}

Coba cocokkan dengan rumus (R1 ∪ R2) − (R1 ∩ R2): hasil gabungan sebelumnya

dikurangi irisan menghasilkan himpunan yang sama, bukan?

                                                                               34
Sifat Tertutup (Closure)

Konsep penting di sini adalah sifat tertutup. Dikatakan tertutup karena hasil operasi
tetap "berada di dalam" jenis objek yang sama.

  • Jika R1 dan R2 keduanya relasi dari A ke B, maka R1 ∩ R2, R1 ∪ R2, R1 − R2, dan
    R1 ⊕ R2 juga relasi dari A ke B.

  • Artinya, kita tidak pernah "keluar" dari himpunan relasi A × B. Hasil operasi selalu
    berupa himpunan bagian dari A × B.

Mengapa ini otomatis benar? Karena setiap operasi hanya menyaring atau

menggabungkan pasangan terurut yang sudah ada di A × B. Irisan mengambil
pasangan yang ada di keduanya (pasti anggota A × B), gabungan menggabungkan

anggota dua himpunan bagian (tetap himpunan bagian), dan seterusnya.

Kaitan dengan Relasi Invers

Ada hubungan menarik antara operasi himpunan dan invers relasi. Sebagai pengingat
dari contoh di materi: jika

R = {(2, 2), (2, 4), (4, 4), (2, 8), (4, 8), (3, 9), (3, 15)}

maka inversnya, dengan aturan (q, p) ∈ R−1 jika (p, q) ∈ R, adalah:
                    R−1 = {(2, 2), (4, 2), (4, 4), (8, 2), (8, 4), (9, 3), (15, 3)}

Sifat pentingnya: invers bersifat kompatibel dengan operasi himpunan, yaitu

(R1 ∪ R2)−1 = R1−1 ∪ R2−1,      (R1 ∩ R2)−1 = R1−1 ∩ R2−1

Selain itu, jika M adalah matriks yang merepresentasikan relasi R, maka matriks
relasi invers, sebut saja N , diperoleh cukup dengan mentranspose matriks M . Jadi
N = M T — baris menjadi kolom, kolom menjadi baris.

                            35
Latihan Soal dan Cara Berpikirnya

Mari kita latih dengan pola soal yang biasanya muncul, sekaligus langkah
penyelesaiannya.

Soal 1. Diketahui A = {1, 2, 3} dan R1 = {(1, 1), (2, 2), (3, 3), (1, 2)}, R2 =
{(1, 1), (2, 2), (3, 3), (2, 3)}. Tentukan R1 ∩ R2 dan R1 ⊕ R2.
Langkah: Untuk irisan, ambil pasangan yang sama di keduanya → R1 ∩ R2 =
{(1, 1), (2, 2), (3, 3)}. Untuk beda setangkup, ambil pasangan yang hanya ada di salah
satu → {(1, 2), (2, 3)}. Perhatikan pasangan identitas tidak muncul karena ada di

keduanya.

Soal 2. Dengan R1 dan R2 pada Soal 1, tentukan R1 − R2.
Langkah: Buang dari R1 semua pasangan yang juga ada di R2. Yang tersisa hanya
{(1, 2)}. Pasangan identitas terbuang karena ada di R2.
Soal 3. Buktikan bahwa untuk relasi apa pun berlaku R1 − R2 = R1 ∩ R2c , dengan R2c
menyatakan komplemen terhadap A × B.
Ide penyelesaian: Ambil sembarang (a, b) ∈ R1 − R2. Berarti (a, b) ∈ R1 dan (a, b) ∈/
R2, yaitu (a, b) ∈ R2c . Jadi (a, b) ∈ R1 ∩ R2c . Sebaliknya, jika (a, b) ∈ R1 ∩ R2c , maka
(a, b) ∈ R1 dan (a, b) ∈/ R2, sehingga (a, b) ∈ R1 − R2. Kedua arah terbukti.
Soal 4. Sebuah relasi R pada A = {1, 2, 3} dinyatakan dengan matriks

                                                     110
                                           M= 0 1 0

                                                     001

Tentukan matriks relasi inversnya.

Langkah: Transpose matriks M , sehingga

                                                      100
                                          MT = 1 1 0

                                                      001

Matriks ini merepresentasikan R−1.

                                                                               36
Kunci Sukses Mengerjakan Soal Relasi

  • Selalu tulis relasi sebagai himpunan pasangan terurut — begitu berbentuk
    himpunan, semua operasi jadi mudah dilihat.

  • Gunakan diagram panah atau matriks untuk memvisualisasikan; matriks sangat
    membantu saat menghitung irisan dan gabungan (bandingkan entri posisi yang
    sama).

  • Ingat sifat tertutup: hasil operasi selalu relasi dari A ke B, jadi jangan heran bila

    hasilnya tetap punya bentuk yang sama.

  • Manfaatkan identitas: R1 − R2 = R1 ∩ R2c dan R1 ⊕ R2 = (R1 ∪ R2) − (R1 ∩ R2)

    sering mempermudah pembuktian atau perhitungan.
  • Untuk invers, cukup transpose matriksnya.
Dengan memahami bahwa relasi hanyalah himpunan khusus, topik ini sebenarnya
tidak lebih sulit dari operasi himpunan biasa. Selamat berlatih — semakin banyak
contoh yang kamu kerjakan, semakin cepat kamu mengenali polanya!

                                                                               37
