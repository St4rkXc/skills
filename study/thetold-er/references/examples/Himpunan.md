---
mode: detailed
pages: 18
words: 3283
---

pelajarin.ai

Definisi dan Penyajian Himpunan

Definisi Himpunan

Himpunan (set) adalah kumpulan objek-objek yang berbeda. Setiap objek di dalam
himpunan disebut elemen, unsur, atau anggota.

Sebagai contoh, HMSI merupakan sebuah himpunan yang berisi anggota berupa
mahasiswa SI. Contoh lain: himpunan bilangan genap, himpunan warna pelangi, atau
himpunan huruf vokal.

Himpunan vs Multiset

Poin penting yang membedakan keduanya:

Aspek          Himpunan                  Multiset

Urutan elemen  Tidak diperhatikan        Diperhatikan

Pengulangan    Tidak boleh ada duplikat  Elemen boleh muncul lebih dari sekali

Karena urutan dan pengulangan tidak berpengaruh pada himpunan, maka {1, 2, 3}
sama dengan {3, 1, 2}, dan {a, a, b} cukup ditulis {a, b}. Multiset seperti {a, a, b} tetap

membedakan jumlah kemunculan tiap elemen.

Cara Penyajian Himpunan

1. Metode Enumerasi (Roster Method)
Semua elemen didaftarkan satu per satu, dipisahkan koma, dan diapit kurung kurawal.

  • A = {1, 2, 3, 4, 5}
  • B = {merah, kuning, hijau}

2. Simbol Baku dan Notasi Pembentuk Himpunan
Beberapa himpunan memiliki simbol baku, misalnya:

  • = himpunan bilangan asli
  • = himpunan bilangan bulat

                                   1
  • = himpunan bilangan real
Notasi pembentuk himpunan mendefinisikan himpunan melalui syarat keanggotaan:

                               A = {x ∣ x bilangan genap, x < 10}

3. Diagram Venn
Diagram Venn menyajikan himpunan secara visual: himpunan semesta digambar
sebagai persegi panjang, sedangkan setiap himpunan sebagai lingkaran/ellips di
dalamnya, dengan elemen dituliskan sebagai titik.

Notasi Keanggotaan
Notasi ∈ berarti "anggota dari", sedangkan ∈/ berarti "bukan anggota dari".

  • Jika A = {1, 2, 3}, maka 2 ∈ A (dibaca: 2 anggota himpunan A).
  • Sebaliknya, 5 ∈/ A (dibaca: 5 bukan anggota himpunan A).
Rangkuman Cepat

  • Himpunan = kumpulan objek berbeda; objeknya disebut elemen.
  • Urutan dan pengulangan tidak relevan dalam himpunan.
  • Tiga cara penyajian: enumerasi, notasi pembentuk himpunan/simbol baku, dan

    diagram Venn.

  • ∈ dan ∈/ menyatakan status keanggotaan suatu elemen.

Materi ini menjadi fondasi untuk topik berikutnya seperti kardinalitas dan operasi
himpunan. Selamat belajar!

                                                                                2
Kardinalitas Himpunan

Memahami Kardinalitas Himpunan

Halo! Setelah kita belajar menyajikan himpunan dengan enumerasi, simbol baku,

notasi pembentuk himpunan, dan diagram Venn, pertanyaan penting berikutnya

adalah: berapa banyak sih elemen di dalam himpunan itu? Jawabannya ada pada

konsep                .

Apa Itu Kardinalitas?

Kardinalitas himpunan adalah banyaknya elemen berbeda (distinct) yang dimiliki

oleh suatu himpunan. Notasi yang umum dipakai adalah n(A) atau ∣A∣, dan dibaca
"jumlah elemen himpunan A".

Ada satu hal kunci yang perlu kamu ingat: karena himpunan tidak mengenal

perulangan elemen, elemen yang sama dihitung satu kali saja. Contohnya,

{1, 2, 2, 3, 4, 4, 4, 5, 6} = {1, 2, 3, 4, 5, 6}, sehingga kardinalitasnya tetap 6, bukan 9.

Perulangan seperti itu baru relevan jika dibahas sebagai  .

Menghitung Kardinalitas Himpunan Berhingga

Untuk himpunan berhingga, kita cukup mendaftar elemennya lalu menghitung berapa
banyak yang berbeda.

Himpunan                         Elemen                                   n(A)

A = {1, 2, 3, 4}                 1, 2, 3, 4                               4

B = {2, 4, 6, 8, 10}             lima bilangan genap positif pertama      5

C = {kucing, a, Amir, 10, paku}  lima elemen berbeda                      5

R = {a, b, {a, b, c}, {a, c}}    4 elemen (dua di antaranya himpunan)     4

K = {{}}                         satu elemen, yaitu himpunan kosong       1

Menarik, bukan? Himpunan K = {{}} punya kardinalitas 1 karena ia berisi satu elemen:
{}. Perhatikan pula bahwa elemen bisa berupa himpunan lain, seperti pada R.

                                 3
Latihan Menghitung Kardinalitas

Coba tentukan kardinalitas dari himpunan-himpunan berikut, ya!

  • Himpunan bilangan asli pertama sampai 100: {1, 2, … , 100}. Karena berurutan
    lengkap, n = 100.

  • {x ∣ x2 = 1, x ∈ }: selesaikan x2 = 1, diperoleh x = −1 dan x = 1. Jadi n = 2.
  • {x ∣ x bilangan bulat positif < 12}: anggotanya 1 sampai 11, sehingga n = 11.
  • {x ∣ x kuadrat bilangan bulat dan x < 100}: kuadratnya

    0, 1, 4, 9, 16, 25, 36, 49, 64, 81 (karena 100 tidak termasuk). Maka n = 10.
Poin Penting untuk Diingat

  • Urutan elemen tidak memengaruhi kardinalitas: {a, b, c} = {c, a, b}.

  • Elemen yang berulang dihitung satu kali dalam himpunan biasa.
  • Elemen himpunan boleh tidak saling berkaitan, yang penting berbeda satu sama

    lain, seperti {56, Rp3000, Amir, cacing}.
  • Untuk himpunan tak berhingga seperti bilangan bulat {… , −2, −1, 0, 1, 2, … },

    kardinalitasnya khusus dan dibahas terpisah.
Dengan memahami kardinalitas, kamu sudah punya bekal kuat untuk menjelajahi
operasi himpunan selanjutnya, seperti gabungan dan irisan. Semangat berlatih!

                                                                                4
Jenis-Jenis Himpunan

Himpunan Kosong (Null Set)

Himpunan kosong adalah himpunan yang tidak memiliki anggota sama sekali.

Kardinalitasnya nol, dan ia dinotasikan dengan ∅ atau {}.
Contohnya, jika E = {x ∣ x bilangan prima genap selain 2}, maka E = ∅ karena tidak

ada bilangan prima genap selain 2.
Hati-hati dengan perbedaan halus ini:

  • {∅} bukan himpunan kosong — ia memuat satu elemen, yaitu himpunan kosong itu

    sendiri.

  • {{}} sama dengan {∅}.
  • {{}, {{}}} sama dengan {∅, {∅}}.
Jadi, membungkus ∅ dengan kurung kurawal menambah satu tingkat "keanggotaan".

Himpunan Bagian (Subset) dan Superset
Himpunan A disebut himpunan bagian dari B jika dan hanya jika setiap elemen A
juga merupakan elemen B. Notasinya A ⊆ B. Dalam kondisi ini, B disebut superset
dari A.

Perhatikan contoh berikut:

A          B                A ⊆ B?

{3, 9}     {5, 9, 1, 3}     Ya

{1, 2, 3}  {2, 3, 4}        Tidak (1 tidak ada di B)

Satu teorema penting: untuk sembarang himpunan A, berlaku A ⊆ A (setiap

himpunan adalah himpunan bagian dari dirinya sendiri).

Himpunan Bagian Sebenarnya (Proper Subset)
A disebut himpunan bagian sebenarnya dari B jika A ⊆ B tetapi A = B — artinya B
memiliki setidaknya satu elemen yang tidak dimiliki A. Dengan kata lain, himpunan

bagian "murni" tidak termasuk himpunan itu sendiri.

                         5
Himpunan yang Sama
Dua himpunan A dan B dikatakan sama (A = B) jika dan hanya jika A ⊆ B dan
B ⊆ A. Inilah aksioma kesamaan: dua himpunan sama bila keduanya saling memuat.
Urutan dan pengulangan penulisan tidak mengubah kesamaan, karena A =
{3, 3, 3, 9} sebenarnya sama dengan {3, 9}.
Himpunan yang Ekivalen

Dua himpunan disebut ekivalen jika keduanya memiliki kardinalitas yang sama, yaitu

∣A∣ = ∣B∣. Perlu dicatat: ekivalen tidak berarti sama. Contohnya A = {1, 2, 3} dan
B = {a, b, c} ekivalen karena ∣A∣ = ∣B∣ = 3, meski anggotanya berbeda.
Himpunan Saling Lepas (Disjoint)
Dua himpunan A dan B disebut saling lepas jika keduanya tidak memiliki anggota
bersama, yaitu A ∩ B = ∅. Contoh: A = {1, 2} dan B = {3, 4} saling lepas.
Himpunan Kuasa (Power Set)
Himpunan kuasa dari A, ditulis P (A), adalah himpunan yang berisi semua himpunan
bagian dari A (termasuk ∅ dan A sendiri). Jumlah anggotanya dirumuskan:

                                              ∣P (A)∣ = 2m

dengan m = ∣A∣. Misalnya, jika A = {a, b}, maka P (A) = {∅, {a}, {b}, {a, b}} dan
∣P (A)∣ = 22 = 4.

Selamat belajar! Pahami perbedaan "bagian" dan "bagian sebenarnya", serta "sama"
dan "ekivalen", karena ketiganya sering menjadi jebakan soal.

                                                                                6
Operasi Dasar pada Himpunan

Memahami Operasi Dasar pada Himpunan

Halo, teman-teman! Setelah mengenal apa itu himpunan, sekarang saatnya kita
bermain dengan operasi-operasinya. Anggap saja himpunan itu seperti kumpulan
benda, dan kita bisa menggabung, memotong, atau membandingkannya. Yuk, kita
bahas satu per satu!

Irisan (Intersection): A B

Irisan dari dua himpunan A dan B adalah himpunan yang berisi elemen-elemen yang

dimiliki bersama oleh A dan B. Notasinya A ∩ B.
  • Jika A = {1, 2, 3} dan B = {3, 4, 5}, maka A ∩ B = {3} karena hanya angka 3 yang

    ada di keduanya.
  • Jika dua himpunan tidak punya elemen sama, keduanya disebut saling lepas

    (disjoint) dengan notasi A//B, sehingga A ∩ B = ∅.

Gabungan (Union): A B

Gabungan dari A dan B adalah himpunan yang memuat semua elemen dari A atau B
(elemen yang muncul di keduanya cukup ditulis sekali).

  • Dengan A = {1, 2, 3} dan B = {3, 4, 5}, maka A ∪ B = {1, 2, 3, 4, 5}.

Komplemen (Complement): A' atau A^c

Komplemen himpunan A adalah semua elemen di dalam semesta pembicaraan (U)
yang bukan anggota A.

  • Jika U = {1, 2, 3, 4, 5} dan A = {1, 2, 3}, maka Ac = {4, 5}.

Selisih (Difference): A − B

Selisih A terhadap B adalah elemen yang ada di A tetapi tidak ada di B.

  • A = {1, 2, 3}, B = {3, 4, 5} A − B = {1, 2} dan B − A = {4, 5}. Perhatikan bahwa

    selisih tidak bersifat komutatif!

                                                                                7
Beda Setangkup (Symmetric Difference): A B

Beda setangkup adalah elemen yang ada di A atau di B, tetapi tidak di keduanya.

Dengan kata lain, A ⊕ B = (A − B) ∪ (B − A).

  • A = {1, 2, 3}, B = {3, 4, 5} A ⊕ B = {1, 2, 4, 5}.

Ringkasan Operasi

Operasi            Notasi     Arti Singkat

Irisan             A∩B        Elemen milik bersama

Gabungan           A∪B        Semua elemen A dan B

Komplemen          Ac         Elemen U di luar A

Selisih            A−B        Milik A, bukan milik B

Beda setangkup     A⊕B        Milik salah satu, bukan keduanya

Penerapan di Kehidupan Nyata

  • Media sosial: A = pengguna yang menyukai sepak bola, B = pengguna yang

    menyukai basket. Irisan A ∩ B adalah pengguna yang menyukai keduanya —

    berguna untuk rekomendasi konten.

  • Daftar belanja: Gabungan membantu menggabungkan daftar belanja dua orang
    menjadi satu tanpa duplikat.

  • Seleksi karyawan: Selisih dapat mencari pelamar yang lolos tes tulis tetapi belum
    mengikuti wawancara.

Dengan menguasai operasi-operasi ini, kamu punya perangkat dasar yang kuat untuk
menyelesaikan banyak masalah himpunan. Jangan ragu berlatih dengan contoh kecil
di sekitarmu, ya. Semangat!

                           8
Perkalian Kartesian

Perkalian Kartesian: Menyusun Pasangan dari Dua Himpunan

Halo! Setelah kita membahas irisan, gabungan, komplemen, selisih, dan beda

setangkup, kini kita berkenalan dengan operasi yang agak berbeda: perkalian

kartesian. Kalau operasi sebelumnya menghasilkan elemen dari himpunan yang

sama, perkalian kartesian justru membentuk         baru. Yuk kita pelajari

bersama!

Definisi Perkalian Kartesian

Perkalian kartesian dari himpunan A dan himpunan B adalah himpunan yang berisi
semua pasangan terurut (a, b), dengan a diambil dari A dan b diambil dari B.

Notasinya:

          A × B = {(a, b) ∣ a ∈ A dan b ∈ B}

Kata "terurut" penting di sini: urutan sangat menentukan, sehingga (a, b) dan (b, a)
dianggap berbeda kecuali a = b.

Kardinalitas Hasil

Jika kita mengetahui banyaknya elemen masing-masing himpunan, kita bisa
langsung menghitung besar hasil perkaliannya:

                       ∣A × B∣ = ∣A∣ ⋅ ∣B∣

Contoh: jika ∣A∣ = 3 dan ∣B∣ = 4, maka ∣A × B∣ = 3 ⋅ 4 = 12 pasangan. Aturan ini

bekerja karena setiap elemen A dipasangkan dengan  elemen B.

Sifat Tidak Komutatif

Perhatikan bahwa:

                       A × B = B × A

                       9
Mengapa? Karena pasangan (a, b) pada A × B memiliki urutan terbalik dibanding
(b, a) pada B × A. Kedua himpunan ini berisi pasangan yang berbeda secara urutan,
jadi hasilnya tidak sama (kecuali dalam kondisi khusus seperti A = B atau salah

satunya himpunan kosong).

Kasus Khusus: Himpunan Kosong

Jika salah satu himpunan kosong, maka tidak ada pasangan yang bisa dibentuk:

           A × = dan × B =

Akibatnya, ∣A × ∣ = 0, sesuai rumus kardinalitas karena ∣A∣ ⋅ 0 = 0.

Contoh Lengkap
Misalkan A = {1, 2} dan B = {x, y}. Maka:

Perkalian  Hasil                             Banyak Elemen

A×B        {(1, x), (1, y), (2, x), (2, y)}  4

B×A        {(x, 1), (x, 2), (y, 1), (y, 2)}  4

Perhatikan bahwa A × B dan B × A sama-sama berisi 4 elemen, tetapi

pasangannya berbeda. Inilah bukti nyata bahwa perkalian kartesian tidak komutatif.

Latihan Mandiri

Coba kerjakan soal berikut untuk mengasah pemahamanmu:

  1. Jika A = {a, b, c} dan B = {1, 2}, tentukan A × B dan hitung ∣A × B∣.
 2. Jika C = {p} dan D = , berapakah C × D?
 3. Diketahui ∣P ∣ = 5 dan ∣Q∣ = 3. Berapakah ∣P × Q∣ dan ∣Q × P ∣? Apakah hasilnya

    sama?
Semangat berlatih! Dengan memahami perkalian kartesian, kamu siap melangkah ke
topik relasi, yang konsepnya dibangun langsung dari operasi ini.

                  10
Perampatan Operasi Himpunan

Halo! Sampai di sini kita sudah lancar mengerjakan irisan dan gabungan untuk dua
himpunan. Pertanyaan menariknya: bagaimana kalau ada tiga, empat, atau bahkan
ratusan himpunan? Tenang, konsepnya sebenarnya hanya perluasan dari yang sudah
kita pelajari. Yuk kita bahas bersama!

Dari Dua Himpunan ke Banyak Himpunan
Operasi seperti irisan dan gabungan bisa kita rampatkan (generalisasi) untuk
sejumlah himpunan, bukan hanya dua. Idenya sederhana: kita kerjakan operasi yang
sama berulang-ulang untuk semua himpunan yang ada.

Misalnya kita punya himpunan A1, A2, A3, … , An. Maka:

  • Irisan merampat: himpunan semua elemen yang menjadi anggota setiap
    himpunan yang terlibat.

  • Gabungan merampat: himpunan semua elemen yang menjadi anggota paling
    sedikit satu himpunan yang terlibat.

Perhatikan kata kuncinya. Irisan menuntut elemen harus ada di semuanya, sedangkan
gabungan cukup muncul di salah satu saja.

Notasi Perampatan
Agar penulisan lebih ringkas, kita gunakan notasi berikut:

Operasi            Notasi            Cara Membaca

Irisan merampat    A1 ∩ A2 ∩ ⋯ ∩ An  irisan dari n himpunan
Gabungan merampat  A1 ∪ A2 ∪ ⋯ ∪ An  gabungan dari n himpunan

Sifat-sifat operasi himpunan — seperti hukum komutatif, asosiatif, dan distributif —
tetap berlaku pada perampatan ini. Itu sebabnya kita bisa mengelompokkan
himpunan dengan bebas tanpa mengubah hasilnya.

Contoh Sederhana
Misalkan:

  • A1 = {1, 2, 3}
  • A2 = {2, 3, 4}

                           11
  • A3 = {3, 4, 5}

Irisan merampat:

                                         A1 ∩ A2 ∩ A3 = {3}

Hanya angka 3 yang muncul di ketiga himpunan sekaligus.

Gabungan merampat:

                                    A1 ∪ A2 ∪ A3 = {1, 2, 3, 4, 5}

Semua elemen yang pernah muncul kita kumpulkan jadi satu.
Kegunaannya di Dunia Nyata
Bayangkan situasi pada himpunan mahasiswa tadi. Kita bisa memakai lebih dari dua
kriteria. Contohnya, misalkan:

  • P = mahasiswa dengan nilai UTS di atas 80
  • Q = mahasiswa dengan nilai UAS di atas 80
  • R = mahasiswa yang aktif di organisasi

Dengan perampatan, kita bisa langsung mencari mahasiswa yang memenuhi ketiga

syarat (P ∩ Q ∩ R) atau mahasiswa yang memenuhi minimal salah satu syarat (P ∪
Q ∪ R). Jauh lebih praktis, bukan?

Inti yang Perlu Diingat
  • Perampatan berarti memperluas operasi himpunan agar berlaku untuk banyak
    himpunan sekaligus.
  • Irisan merampat = elemen yang ada di semua himpunan.
  • Gabungan merampat = elemen yang ada di setidaknya satu himpunan.
  • Hukum-hukum aljabar himpunan tetap berlaku, sehingga kita leluasa menyusun
    ulang operasinya.

                                                                               12
Kuncinya adalah memahami pola: irisan makin "sempit", gabungan makin "luas". Kalau
pola ini sudah kamu pegang, berapa pun jumlah himpunannya tidak akan jadi
masalah. Selamat belajar, kamu pasti bisa!

                                                                               13
Hukum-Hukum Aljabar Himpunan

Halo! Siap belajar hukum-hukum himpunan? Tenang, materi ini sebenarnya rapi dan
berpola — begitu kamu paham beberapa aturan dasarnya, sisanya akan terasa
mudah.

Hukum Identitas dan Hukum Null
Hukum identitas menunjukkan bahwa ada elemen "netral" yang tidak mengubah hasil
operasi.

  • A ∩ U = A — irisan dengan semesta tidak mengubah A.
  • A ∪ ∅ = A — gabungan dengan himpunan kosong juga tidak mengubah A.

Kebalikannya, hukum null (dominasi) menunjukkan elemen yang "menelan" hasil
operasi:

  •A∪U =U
  •A∩∅=∅

Hukum Komutatif dan Asosiatif
Komutatif berarti urutan tidak berpengaruh:

  •A∪B =B∪A
  •A∩B =B∩A

Asosiatif berarti pengelompokan tidak berpengaruh:

  • (A ∪ B) ∪ C = A ∪ (B ∪ C)
  • (A ∩ B) ∩ C = A ∩ (B ∩ C)

Hukum Distributif

Operasi gabungan dan irisan saling mendistribusi, mirip sifat a(b + c) = ab + ac pada

aritmetika:

  • A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C)
  • A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)

                                                                               14
Hukum Idempoten dan Hukum Komplemen
Idempoten — mengulang operasi pada himpunan yang sama tidak menambah apa
pun:

  •A∪A=A
  •A∩A=A
Komplemen melibatkan semesta U :
  • (Ac)c = A
  • A ∪ Ac = U
  • A ∩ Ac = ∅
  • U c = ∅ dan ∅c = U

Hukum De Morgan
Hukum ini sangat berguna saat menyederhanakan komplemen dari gabungan atau
irisan:

  • (A ∪ B)c = Ac ∩ Bc
  • (A ∩ B)c = Ac ∪ Bc

Singkatnya: komplemen "membalik" operasinya.

Hukum Penyerapan dan Hukum Lainnya
Penyerapan (absorpsi):

  • A ∪ (A ∩ B) = A
  • A ∩ (A ∪ B) = A

Hukum selisih:

  • A − B = A ∩ Bc

Prinsip Dualitas — Kunci Semua Hukum Ini
Inilah ide yang membuat tabel di atas terasa ringkas. Prinsip dualitas menyatakan:
dua konsep berbeda dapat dipertukarkan namun tetap menghasilkan jawaban benar.

Jika S adalah kesamaan himpunan, dual S∗ diperoleh dengan menukar:

Tukar  Menjadi

       15
∪  ∩

∩  ∪

∅  U

U  ∅

Komplemen dibiarkan seperti semula. Contoh: A ∩ U = A berdual A ∪ ∅ = A.

Analogi sederhananya: seperti kemudi mobil di Amerika Serikat (kanan) versus Inggris
(kiri) — konsep kiri dan kanan dapat dipertukarkan selagi aturannya konsisten.

Latihan Singkat: Kardinalitas dan Keanggotaan

Kardinalitas n(A) adalah banyaknya elemen dalam A:
  • n({a}) = 1 dan n({{a}}) = 1 (satu elemen, yaitu himpunan {a}).
  • n({a, {a}}) = 2.

Untuk pernyataan keanggotaan, bedakan ∈ (elemen) dan ⊆ (himpunan bagian):
  • 0 ∈ ∅ salah, karena ∅ tidak punya elemen.
  • ∅ ∈ {0} salah; {0} hanya memuat elemen 0.
  • ∅ ⊂ {0} benar; himpunan kosong adalah himpunan bagian dari setiap

    himpunan.
Semangat berlatih! Kuasai dualitasnya, dan separuh tabel hukum ini otomatis kamu
hafal.

   16
Prinsip Dualitas

Memahami Prinsip Dualitas

Halo! Setelah kita mempelajari hukum-hukum aljabar himpunan, sekarang saatnya
berkenalan dengan salah satu ide paling elegan dalam teori himpunan: prinsip
dualitas. Kabar baiknya, konsep ini sebenarnya cukup intuitif—kita hanya perlu
menukar beberapa simbol, dan ternyata hasilnya tetap benar!

Apa Itu Prinsip Dualitas?
Secara sederhana, prinsip dualitas menyatakan bahwa dua konsep yang berbeda
dapat dipertukarkan, namun tetap memberikan jawaban yang benar. Prinsip ini terlihat
jelas pada tabel kesamaan himpunan: setiap baris pertama dari suatu hukum
identitas memiliki dual pada baris kedua.

Contohnya, hukum identitas A ∩ U = A memiliki dual A ∪ ∅ = A. Keduanya sama-

sama benar!

Cara Memperoleh Dual Suatu Kesamaan

Misalkan S adalah suatu kesamaan (      ) yang melibatkan himpunan dan operasi

seperti ∪, ∩, serta komplemen. Dual dari S, yang kita sebut S∗, diperoleh dengan

aturan pertukaran berikut:

Simbol Asal                             Ditukar Menjadi

∪ (gabungan)                            ∩ (irisan)

∩ (irisan)                              ∪ (gabungan)

∅ (himpunan kosong)                     U (semesta)

U (semesta)                             ∅ (himpunan kosong)

Catatan penting: operasi komplemen dibiarkan seperti semula, tidak ikut ditukar. Jika

S∗ diperoleh dengan cara ini, maka S∗ juga merupakan kesamaan yang benar dan
disebut dual dari S.

Contoh Penerapan pada Hukum-Hukum Himpunan
Mari kita lihat bagaimana dualitas bekerja pada beberapa hukum himpunan:

                                    17
Hukum        Kesamaan Asli      Dualnya

Identitas    A∩U =A             A∪∅=A

Idempoten A ∩ A = A             A∪A=A

Komutatif    A∩B =B∩A           A∪B =B∪A

Distributif  A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C) A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C)

Perhatikan pola yang konsisten: cukup tukar ∪ dengan ∩, dan ∅ dengan U . Selesai!

Kesamaan baru yang terbentuk otomatis juga valid.

Ilustrasi dalam Kehidupan Sehari-Hari
Prinsip dualitas ternyata hadir di sekitar kita. Bayangkan peraturan lalu lintas di dua
negara:

  • Amerika Serikat: mobil berjalan di kanan jalan, lajur kiri untuk mendahului, dan
    saat lampu merah menyala, mobil boleh belok kanan langsung.

  • Inggris (atau Indonesia): mobil berjalan di kiri jalan, lajur kanan untuk mendahului,
    dan saat lampu merah, mobil boleh belok kiri langsung.

Konsep kiri dan kanan dipertukarkan, namun peraturan tetap konsisten dan berlaku
dengan benar di masing-masing negara. Inilah esensi dualitas: menukar pasangan
konsep yang berlawanan tanpa merusak kebenaran sistem.

Dengan memahami prinsip ini, kamu bisa menghemat usaha—cukup kuasai satu
hukum himpunan, dan dualnya langsung kamu dapatkan secara gratis. Selamat
belajar, dan jangan ragu bereksperimen dengan pertukaran simbol!

                            18
