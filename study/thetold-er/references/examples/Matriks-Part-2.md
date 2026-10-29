---
mode: medium
pages: 10
words: 1665
---

      pelajarin.ai

Tinjauan Ulang Konsep Dasar Matriks dan Relasi

Matriks dan Relasi Biner

Matriks adalah susunan bilangan dalam bentuk persegi panjang, yang tersusun atas
baris dan kolom.

Relasi biner R dari himpunan A ke himpunan B dipandang sebagai pemetaan dari
hasil kali Kartesius A × B ke himpunan {0, 1}. Nilai 1 menunjukkan pasangan
berurutan termasuk relasi, sedangkan nilai 0 menunjukkan sebaliknya.
Representasi Relasi

Relasi dapat disajikan melalui:

  • Diagram panah, dengan panah dari anggota A menuju anggota B.

  • Tabel, yang mencatat pasangan anggota dan status relasinya.

  • Matriks biner (matriks nol-satu), berisi hanya angka 0 dan 1.

  • Graf berarah, dengan titik sebagai anggota himpunan dan anak panah sebagai
    relasi.

Sifat dan Operasi Relasi

Untuk relasi pada suatu himpunan, sifatnya dapat berupa refleksif, simetris,

antisimetris, atau transitif. Relasi invers R−1 dari B ke A membalik setiap pasangan:
(b, a) ∈ R−1 jika dan hanya jika (a, b) ∈ R.
Beberapa relasi dapat digabungkan menggunakan union (∪), intersection (∩), selisih,

dan selisih setangkup, yaitu pasangan yang terdapat tepat pada salah satu relasi.

                                                                                1
Komposisi Relasi: Definisi dan Konsep Dasar

Halo! Yuk kita pelajari komposisi relasi. Konsep ini mirip dengan "menyambung" dua
perjalanan: dari titik awal ke titik tengah, lalu lanjut ke titik akhir.

Definisi Formal
Misalkan R adalah relasi dari himpunan A ke himpunan B, dan S adalah relasi dari
himpunan B ke himpunan C. Komposisi R dan S, dinotasikan S ∘ R, adalah relasi dari A
ke C yang didefinisikan oleh:

S ∘ R = {(a, c) ∣ a ∈ A, c ∈ C, dan untuk beberapa b ∈ B, (a, b) ∈ R dan (b, c) ∈ S}

Urutan Penerapan
Perhatikan urutannya dengan saksama:

  1. Terapkan R terlebih dahulu — dari A ke B, menghasilkan pasangan (a, b).
 2. Baru kemudian terapkan S — dari B ke C, menghasilkan pasangan (b, c).
 3. Hasil akhirnya adalah pasangan (a, c) dari A ke C.

Meskipun R diterapkan lebih dulu, notasinya ditulis S ∘ R (dibaca "S setelah R"). Ini
karena notasi dibaca dari kanan ke kiri, seperti fungsi komposisi.

Peran Elemen Perantara b ∈ B

Elemen b adalah "jembatan" yang menghubungkan kedua relasi. Pasangan (a, c)
hanya terbentuk jika ada elemen b ∈ B sedemikian sehingga (a, b) ∈ R dan (b, c) ∈ S.
Tanpa perantara yang cocok, (a, c) tidak termasuk dalam komposisi.

Komponen  Peran

A         Himpunan asal

B         Himpunan perantara

C         Himpunan tujuan

R         Relasi A → B

          2
S    Relasi B → C
S∘R  Relasi A → C

Semangat belajar! Dengan memahami peran elemen perantara, kamu sudah
menguasai inti komposisi relasi.

     3
Contoh Komposisi Relasi dan Representasinya

Contoh 20: Menelusuri Komposisi Relasi
Diberikan A = {1, 2, 3}, B = {2, 4, 6, 8}, dan C = {s, t, u}, dengan

                          R = {(1, 2), (1, 6), (2, 4), (3, 4), (3, 6), (3, 8)}

           S = {(2, u), (4, s), (4, t), (6, t), (8, u)}.

Pada S ∘ R, terapkan R terlebih dahulu untuk berpindah dari A ke B, lalu terapkan S
untuk berpindah dari B ke C. Pasangan awal dan akhir dicatat apabila keduanya
terhubung melalui anggota B.

Anggota A  Jalur melalui B                                Hasil di C

1          1 → 2 → u; 1 → 6 → t                           u, t

2          2 → 4 → s; 2 → 4 → t                           s, t

3          3 → 4 → s, t; 3 → 6 → t; 3 → 8 → u             s, t, u

Jadi,

           S ∘ R = {(1, u), (1, t), (2, s), (2, t), (3, s), (3, t), (3, u)}.

Diagram panah memperagakan perhitungan yang sama: gambarkan panah R dari A
ke B dan panah S dari B ke C, kemudian ikuti setiap rangkaian dua panah. Meskipun
3 mencapai t melalui 4 dan 6, pasangan (3, t) cukup ditulis sekali.

Representasi Matriks

Dengan urutan baris dan kolom sesuai urutan anggota himpunan di atas, matriks
relasinya ialah

                            4
           1010           001
MR = 0 1 0 0 ,
                    MS =  1  1  0  .
           0111           0  1  0

                          001

Seperti bentuk pada Contoh 21, MR2∘R1 = MR1 ⋅ MR2 . Kalikan matriks menurut urutan

penerapan relasi; setiap hasil positif menunjukkan adanya jalur. Dengan demikian,

             011
MS∘R = 1 1 0 .

             111

                 5
Relasi Ekuivalen: Definisi dan Sifat

Relasi ekuivalen membantu kita merelasikan objek-objek yang memiliki kemiripan
dalam suatu hal tertentu. Idenya sederhana: kita ingin mengelompokkan hal-hal yang
"setara" menurut kriteria tertentu.

Definisi

Suatu relasi pada himpunan A disebut relasi ekuivalen jika relasi tersebut memenuhi

tiga sifat sekaligus:
  1. Refleksif
 2. Simetris
 3. Transitif

Dua anggota A yang berelasi oleh relasi ekuivalen dikatakan ekivalen.

Makna Tiap Sifat

Sifat      Implikasi

Refleksif  Setiap elemen ekivalen terhadap dirinya sendiri.

Simetris   a ekivalen dengan b setiap kali b ekivalen dengan a.

Transitif  Jika a dan b ekivalen serta b dan c ekivalen, maka a dan c juga ekivalen.

Contoh

Misalkan A himpunan string atas suatu alfabet dan l(x) menyatakan panjang string x.
Definisikan relasi R pada A dengan a R b jika dan hanya jika l(a) = l(b).

  • Refleksif: l(a) = l(a), jadi a R a. ✓

  • Simetris: jika l(a) = l(b), maka l(b) = l(a). ✓

  • Transitif: jika l(a) = l(b) dan l(b) = l(c), maka l(a) = l(c). ✓

Ketiga sifat terpenuhi, sehingga R adalah relasi ekuivalen — string-string dengan

panjang sama saling ekivalen.

                      6
Contoh dan Pembuktian Relasi Ekuivalen

Misalkan A adalah himpunan semua string yang dibentuk dari suatu alfabet, dan l(x)
menyatakan panjang string x. Definisikan relasi R pada A sebagai berikut:

                                        a R b ⟺ l(a) = l(b)

Artinya, dua string berelasi jika panjangnya sama. Untuk memastikan R adalah relasi

ekuivalen, kita harus membuktikan tiga sifat: refleksif, simetris, dan transitif.

Pembuktian Ketiga Sifat
1. Refleksif. Untuk setiap string a, jelas l(a) = l(a), sehingga a R a. Sifat refleksif

terpenuhi.

2. Simetris. Jika a R b, maka l(a) = l(b). Karena kesamaan bilangan bersifat simetris,
l(b) = l(a), sehingga b R a. Sifat simetris terpenuhi.
3. Transitif. Jika a R b dan b R c, maka l(a) = l(b) dan l(b) = l(c). Karena kesamaan
bilangan bersifat transitif, l(a) = l(c), sehingga a R c. Sifat transitif terpenuhi.
Kesimpulan
Karena R memenuhi sifat refleksif, simetris, dan transitif, maka R merupakan relasi

ekuivalen. Perhatikan bahwa inti pembuktiannya bertumpu pada sifat kesamaan
bilangan yang sudah kita kenal — sebuah strategi yang sering dipakai untuk
membuktikan relasi ekuivalen.

                                                                                7
Relasi Pengurutan Parsial dan Himpunan Terurut Parsial
(Poset)

Relasi Pengurutan Parsial

Halo! Mari kita pelajari salah satu relasi paling penting dalam matematika diskrit, yaitu
relasi pengurutan parsial. Relasi ini memungkinkan kita membandingkan elemen-
elemen dalam himpunan berdasarkan "urutan" tertentu.

Definisi Pengurutan Parsial

Sebuah relasi R pada himpunan S disebut relasi pengurutan parsial jika memenuhi

tiga sifat sekaligus:

  • Refleksif: setiap elemen berelasi dengan dirinya sendiri, yaitu (a, a) ∈ R untuk
    semua a ∈ S.

  • Antisimetris: jika (a, b) ∈ R dan (b, a) ∈ R, maka haruslah a = b.
  • Transitif: jika (a, b) ∈ R dan (b, c) ∈ R, maka (a, c) ∈ R.

Himpunan Terurut Parsial (Poset)

Jika R adalah relasi pengurutan parsial pada S, maka pasangan (S, R) disebut

himpunan terurut parsial (partially ordered set), disingkat poset. Kata "parsial" dipakai
karena tidak semua pasangan elemen harus bisa dibandingkan.

Contoh-Contoh Poset

Poset      Relasi             Mengapa Poset?

(Z, ≥)     "lebih besar sama  refleksif (a ≥ a), antisimetris, transitif
           dengan"

(Z+, ∣)    "habis dibagi"     a ∣ a; jika a ∣ b dan b ∣ a maka a = b; transitif

(P (S), ⊆  "subhimpunan"      A ⊆ A; jika A ⊆ B dan B ⊆ A maka A = B;
)
                              transitif

Ketiga contoh ini menunjukkan bahwa pengurutan parsial muncul secara alami, baik
pada bilangan maupun pada himpunan.

                              8
Klosur Relasi: Konsep dan Klosur Refleksif serta Setangkup

Konsep Klosur Relasi
Sebuah relasi R pada himpunan A bisa memiliki atau tidak memiliki sifat tertentu,

misalnya refleksif, setangkup, atau menghantar. Klosur adalah cara "memaksa" relasi
agar memiliki sifat tersebut dengan penambahan seminimal mungkin.

Definisi: Jika S adalah relasi dengan sifat P yang mengandung R, dan S merupakan
himpunan bagian dari setiap relasi bersifat P yang mengandung R, maka S disebut
klosur (closure) atau tutupan dari R. Intinya, S adalah relasi terkecil bersifat P yang
memuat R.
Klosur Refleksif
Klosur refleksif dibentuk dengan menambahkan semua pasangan (a, a) yang belum

ada. Secara formal:

                                S = R ∪ Δ, Δ = {(a, a) ∣ a ∈ A}

Contoh: R = {(1, 1), (1, 3), (2, 3), (3, 2)} pada A = {1, 2, 3} belum refleksif karena
(2, 2) dan (3, 3) tidak ada. Setelah ditambahkan:

                          S = {(1, 1), (1, 3), (2, 2), (2, 3), (3, 2), (3, 3)}

Klosur Setangkup
Klosur setangkup dibentuk dengan menambahkan pasangan kebalikan (b, a) untuk
setiap (a, b) ∈ R yang belum memiliki pasangannya.
Contoh: R = {(1, 3), (1, 2), (2, 1), (3, 2), (3, 3)} pada A = {1, 2, 3} tidak setangkup
karena (1, 3) ada tetapi (3, 1) tidak. Klosur setangkupnya menambahkan (3, 1) dan
(2, 3), menghasilkan relasi yang setiap pasangannya muncul dua arah.

Perhatikan bahwa kedua klosur ini hanya menambah pasangan, tidak pernah
menghapus.

                                                                                9
Klosur Menghantar (Transitif) dan Latihan Soal

Klosur Menghantar dan Latihan Soal
Relasi R = {(1, 2), (1, 4), (2, 1), (3, 2)} pada A = {1, 2, 3, 4} tidak transitif. Pasangan
yang perlu ditambahkan agar menjadi transitif adalah (1, 1), (2, 2), (2, 4), dan (3, 1).
Latihan. Diberikan R = {(1, 2), (2, 1), (2, 3), (3, 3)} pada S = {1, 2, 3}.

  • Klosur refleksif: R ∪ Δ, dengan Δ = {(1, 1), (2, 2), (3, 3)}, menghasilkan
    {(1, 1), (1, 2), (2, 1), (2, 2), (2, 3), (3, 3)}.

  • Klosur menghantar: R∗ = {(1, 1), (1, 2), (1, 3), (2, 1), (2, 2), (2, 3), (3, 3)}.
Latihan komposisi. Untuk R = {(1, 2), (1, 3), (2, 3), (2, 4), (3, 1)} dan S =
{(2, 1), (3, 1), (3, 2), (4, 2)}, tentukan S ∘ R dan R ∘ S dengan menelusuri pasangan

berurutan.

                                                                               10
