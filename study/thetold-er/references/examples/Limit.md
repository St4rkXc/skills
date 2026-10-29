---
mode: medium
pages: 14
words: 2823
---

pelajarin.ai

Pendahuluan dan Peta Konsep Limit

Selamat Datang di Dunia Limit!

Halo! Sebelum kita menyelami kalkulus lebih jauh, mari berkenalan dengan konsep
yang menjadi fondasi seluruh bangunan ini: limit. Anggap limit sebagai "jembatan"
yang menghubungkan aljabar biasa dengan kalkulus — tanpa jembatan ini, kita tidak
bisa melangkah ke turunan dan integral.

Mengapa Limit Begitu Penting?

Limit adalah landasan aksiomatis kalkulus diferensial dan integral. Coba bayangkan
dua definisi inti berikut:

  • Turunan didefinisikan sebagai laju perubahan sesaat (instantaneous rate of
    change) — yang secara matematis adalah limit.

  • Integral tentu didefinisikan sebagai limit jumlahan Riemann — juga limit!
Tanpa pemahaman limit yang presisi, kedua definisi ini tidak dapat dikonstruksi
secara matematis. Itulah sebabnya limit selalu diajarkan pertama.

Peta Konsep: Empat Pilar Utama

Materi limit terbagi menjadi empat pilar yang saling menopang:

Pilar                    Fokus Pembelajaran

1. Konsep Fundamental &  Memahami perilaku lokal fungsi di sekitar titik uji; teknik
Sifat Aljabar            eliminasi bentuk tak tentu aljabar

2. Limit Sepihak         Analisis arah pendekatan dari kiri dan kanan; kriteria eksistensi
                         limit bilateral

3. Limit Fungsi          Pemanfaatan Teorema Apit (Squeeze Theorem) dan identitas
Trigonometri             analitis untuk bentuk tak tentu rasio trigonometris

4. Perilaku Asimtotik    Fenomena ketakhinggaan: limit tak hingga (asimtot tegak)
                         dan limit di tak hingga (asimtot datar)

                         1
Intuisi Awal: Melihat Limit Beraksi

Mari lihat contoh sederhana. Tinjau fungsi rasional:

          f (x)   =     x2 − 1
                        x−1

Domainnya adalah seluruh bilangan riil kecuali x = 1, sebab substitusi langsung

menghasilkan bentuk tak tentu:

f (1)  =  1−1  =  0     (tidak terdefinisi)
          1−1     0

Meski f (1) tidak terdefinisi, kita tetap bisa mengamati perilaku f (x) saat x mendekati
1 tanpa pernah menyentuhnya:

  • Dari kiri (x < 1): f (0,9) = 1,9; f (0,99) = 1,99; f (0,999) = 1,999 → menuju 2

  • Dari kanan (x > 1): f (1,1) = 2,1; f (1,01) = 2,01 → juga menuju 2

Kedua arah mengarah ke nilai yang sama! Inilah inti gagasan limit: kita peduli pada
perilaku fungsi di sekitar titik, bukan pada nilai fungsi tepat di titik itu. Fenomena
inilah yang akan kita bedah secara mendalam di bab-bab berikutnya. Siap? Mari kita
mulai!

                     2
Konsep Fundamental Limit Fungsi

Intuisi Limit: Mendekat Tanpa Harus Menyentuh

Bayangkan kita mengamati bagaimana nilai f (x) berubah ketika x mendekati suatu
titik. Dari pola numerik, misalnya saat x = 1,01 memberi f (x) = 2,01 dan x = 1,001
memberi f (x) = 2,001, terlihat bahwa f (x) semakin dekat ke bilangan tetap 2. Inilah

inti konsep limit: limit berfokus pada kecenderungan nilai fungsi di sekitar titik uji,
bukan pada nilai fungsi tepat di titik tersebut. Grafik pun memperkuat ini: kurva
mengarah ke satu ketinggian tertentu walau titik itu sendiri "berlubang".

Definisi Intuitif dan Formal
Secara intuitif, lim f (x) = L berarti nilai f (x) dapat dibuat sedekat mungkin ke L

                          x→c

asalkan jarak antara x dan c dibuat cukup kecil, dengan syarat x = c.

Untuk ketelitian analitis, Cauchy dan Weierstrass merumuskan definisi presisi epsilon-

delta: lim f (x) = L jika dan hanya jika untuk setiap ϵ > 0 (berapapun kecilnya)

           x→c

terdapat δ > 0 sehingga jika 0 < ∣x − c∣ < δ maka berlaku ∣f (x) − L∣ < ϵ.

Makna geometrisnya:

  • ϵ adalah pita toleransi vertikal (L − ϵ, L + ϵ).

  • δ adalah pita horizontal (c − δ, c + δ), tanpa melibatkan titik c.

  • Jaminannya: seluruh bayangan f (x) di dalam interval horizontal jatuh ke dalam

    pita toleransi vertikal.

Sifat-Sifat Aljabar Limit

Jika lim f (x) = L dan lim g(x) = M keduanya ada dan berhingga, serta k skalar,
x→c               x→c

maka:

Sifat                      Rumus

Konstanta                  lim k = k
Identitas
Kelipatan skalar           x→c

                           lim x = c

                           x→c

                           lim[k ⋅ f (x)] = k ⋅ L

                           x→c

                                  3
Penjumlahan/pengurangan                         lim[f (x) ± g(x)] = L ± M
Perkalian
Pembagian                                       x→c
Perpangkatan
Akar                                            lim[f (x) ⋅ g(x)] = L ⋅ M

                                                x→c

                                                lim    f (x)  =  L , syarat M  =  0
                                                       g(x)
                                                x→c              M

                                                lim[f (x)]n = Ln

                                                x→c

                                                lim n f (x) = n L; untuk n genap disyaratkan L > 0

                                                x→c

Bentuk Tentu vs Tak Tentu

Bentuk  tentu  langsung          memberi        hasil  pasti,    misalnya  2   atau   5  +  7.  Bentuk  tak tentu
                                                                           3

muncul  saat   substitusi        menghasilkan          ekspresi  seperti   0   —   hasilnya     belum  jelas  dan
                                                                           0

perlu diolah lebih lanjut.

Tiga metode dasar menyelesaikannya:

1. Substitusi langsung — coba dulu; jika hasilnya tentu, selesai.

2.  Faktorisasi  —     untuk     0  pada  polinomial,         faktorkan  lalu  coret     faktor  penyebab     nol.
                                 0
                       x2 −1          (x−1)(x+1)
    Contoh: lim        x−1    =  lim       x−1    =    2.

                  x→1            x→1

3. Rasionalisasi — untuk bentuk akar, kalikan dengan sekawan. Contoh: lim                               x+1−1 ⋅
                                                                                                 x→0
                                                                                                          x

    x+1+1  =   lim     x(      x      =   1  .
    x+1+1                     x+1+1)      2
               x→0

Kunci suksesnya: kenali bentuknya dulu, baru pilih metode yang tepat.

                                                              4
Limit Sepihak (Limit Kiri dan Kanan)

Konsep Limit Kiri dan Limit Kanan
Halo! Mari kita bedah limit sepihak. Idenya sederhana: alih-alih mendekati titik c dari

dua arah sekaligus, kita mendekat hanya dari satu sisi.

  • Limit kiri limx→c− f (x): nilai f (x) saat x mendekati c dari nilai yang lebih kecil (x <
    c).

  • Limit kanan limx→c+ f (x): nilai f (x) saat x mendekati c dari nilai yang lebih besar
    (x > c).

Limit sepihak sangat berguna ketika fungsi "bertingkah" berbeda di kedua sisi titik,
misalnya pada fungsi sepotong-sepotong.

Teorema Fundamental Keberadaan Limit Bilateral
Ini inti bab ini. Limit bilateral limx→c f (x) ada jika dan hanya jika kedua limit sepihak

ada dan nilainya sama:

                lim f (x) = L ⟺ lim f (x) = lim f (x) = L
                x→c            x→c−                  x→c+

Jika kedua limit sepihak berbeda, limit bilateral tidak ada.

Tiga Penyebab Limit Tidak Ada

Penyebab        Ciri                                 Ilustrasi

Diskontinuitas  Limit kiri = limit kanan, keduanya  Fungsi sepotong dengan
loncat
                berhingga                            "lompatan" nilai di c

Perilaku tak    Fungsi membesar/mengecil             limx→0   1   = +∞
terhingga                                                     x2
                tanpa batas di sekitar c

Osilasi         Nilai terus berayun tanpa            Fungsi yang bergetak tak
                menetap
                                                     beraturan mendekati c

                               5
Analisis pada Berbagai Jenis Fungsi
Fungsi sepotong-sepotong: hitung limit kiri memakai cabang untuk x < c, dan limit
kanan memakai cabang untuk x > c, lalu bandingkan. Inilah tempat limit sepihak

paling sering diuji.

Fungsi nilai mutlak: titik "patahan" di x = 0 wajib diperiksa dari dua arah. Untuk
f (x) = ∣x∣, limit kiri bernilai −x dan limit kanan bernilai +x — keduanya bertemu di 0,

jadi limitnya ada.

Fungsi tangga (floor): di bilangan bulat n, ⌊x⌋ meloncat. Limit kiri bernilai n − 1
sementara limit kanan bernilai n, sehingga limit bilateral tidak ada di setiap titik

bilangan bulat.

Contoh: Nilai Mutlak dan Penentuan Parameter

Contoh nilai mutlak:  evaluasi limx→0      ∣x∣   .  Untuk  x   <  0,  ∣x∣  =  −1; untuk x  >  0,  ∣x∣  =  +1.
                                           x                          x                           x

Karena −1 = +1, limit tidak ada (diskontinuitas loncat).

Contoh parameter piecewise: misalkan

                                  f  (x)  =      {xax2  +  1,  x<2
                                                        +  b,  x≥2

Agar limit di x = 2 ada, syaratnya limit kiri = limit kanan: 2a + 1 = 4 + b. Dari satu
persamaan ini kita bisa menentukan hubungan parameter (misalnya b = 2a − 3);
nilai a dan b tunggal butuh syarat tambahan seperti kesinambungan nilai fungsi.

Catatan Penyelesaian Aljabar

Saat menghitung limit sepihak, tetap evaluasi lewat substitusi langsung lebih dulu.

Jika  muncul  bentuk  tak  tentu  seperti  0  ,  gunakan       faktorisasi    (batalkan  faktor   (x   −  c))
                                           0

atau rasionalisasi (kalikan konjugat memakai (a − b)(a + b) = a2 − b2) sebelum

menyimpulkan. Setelah penyederhanaan, substitusi ulang memberi nilai definitif tiap

arah — baru bandingkan keduanya.

Semangat berlatih! Kuncinya selalu: periksa dua arah, bandingkan, simpulkan.

                                                    6
Limit Fungsi Trigonometri

Teorema Apit (Squeeze Theorem) dan Penerapannya

Teorema Apit menyatakan bahwa jika sebuah fungsi "terjepit" di antara dua fungsi lain
yang menuju nilai limit yang sama, maka fungsi yang terjepit tersebut juga menuju

nilai yang sama. Secara formal: jika g(x) ≤ f (x) ≤ h(x) di sekitar titik c dan
limx→c g(x) = limx→c h(x) = L, maka limx→c f (x) = L.

Teorema ini menjadi kunci untuk menangani fungsi yang berosilasi, seperti f (x) =

sin 1 saat x → 0. Ketika x → 0, argumen 1 → ±∞, sehingga nilai sinus terus berayun
   x                                                         x

antara −1 dan 1 tanpa memusat ke satu nilai. Inilah perilaku berosilasi tanpa henti —

salah satu dari tiga penyebab kegagalan eksistensi limit (selain diskontinuitas loncat

dan perilaku menuju tak terhingga).

Pembuktian Geometris limx→0                                  sin x  =  1
                                                               x

Bayangkan lingkaran satuan dengan sudut pusat x (dalam radian). Bandingkan tiga

luas:

•  Segitiga      kecil:  1  sin x
                         2

•  Sektor  lingkaran:          1  x
                               2

•  Segitiga      besar:     1  tan x
                            2

Karena segitiga kecil ≤ sektor ≤ segitiga besar, maka sin x ≤ x ≤ tan x. Membagi

dengan sin x memberi 1               ≤    x    ≤    1  x  .  Dengan    Teorema   Apit  dan  fakta  cos  x  →  1,
                                        sin x     cos

terbukti  sin x  →  1.
            x

Teorema Dasar dan Perluasan Koefisien

Bentuk dasar                                                        Nilai limit

limx→0 sin x                                                        1

           x

limx→0 tan x                                                        1
           x

limx→0      x    x                                                  1
          sin

                                                                7
Perluasan koefisien: jika argumen sinus berbentuk ax, maka limx→0                              sin ax  =  1,
                                                                                                 ax

sehingga limx→0       sin ax  =  a.
                        x

Catatan    kritis  mengenai limit        kosinus:  berbeda       dengan        sinus,  limx→0     cos x  tidak ada  —
                                                                                                    x

pembilangnya menuju 1 sementara penyebut menuju 0. Yang benar adalah

limx→0  1−cos x    =  0, karena bentuk ini dapat dimanipulasi memakai                       identitas sudut
            x

rangkap.

Identitas Trigonometri Esensial

• Sudut rangkap: sin 2x = 2 sin x cos x dan cos 2x = 1 − 2 sin2 x

•  Selisih  kosinus:  cos A      −   cos  B  =  −2    sin(  A+B  )   sin(      A−B  )
                                                              2                  2

•  Selisih  sinus:    sin A   −  sin  B   =  2  cos(  A+B  )  sin(   A−B    )
                                                        2              2

Contoh Penggunaan Identitas

Contoh  1  (sudut     rangkap):      Hitung  limx→0   1−cos   2x  .  Gunakan        cos 2x  =  1  −    2 sin2  x,
                                                          x2
sehingga 1 − cos 2x = 2 sin2 x. Maka limitnya = 2 ( sin x )2 = 2.
                                                                            x

Contoh  2  (selisih kosinus):        Hitung  limx→0   cos   4x−cos   2x  .  Dengan     identitas  selisih  kosinus,
                                                              x2

cos 4x − cos 2x = −2 sin 3x sin x. Limitnya = −2 ⋅ 3 ⋅ 1 = −6.

Semangat berlatih! Kunci sukses bab ini adalah mengenali kapan memakai Teorema
Apit dan kapan memanipulasi identitas agar muncul bentuk sin x .

                                                                                                               x

                                                      8
Limit Tak Hingga dan Limit di Tak Hingga

Memahami Dua Wajah "Tak Hingga"

Halo! Sebelum masuk ke rumus, mari kita luruskan dulu satu hal yang sering bikin
bingung: frasa "tak hingga" bisa muncul di dua posisi berbeda, dan keduanya punya
makna yang sangat berbeda. Yuk kita bedakan.

Limit tak hingga adalah ketika nilai fungsi yang membesar tanpa batas, misalnya

f (x) → ∞ saat x → c. Ini berkaitan dengan asimtot tegak di x = c. Sebaliknya, limit di
tak hingga adalah ketika variabel x yang menuju tak hingga, misalnya x → ∞. Ini

berkaitan dengan asimtot datar.

Istilah                Yang menuju tak hingga Asimtot                          Contoh

Limit tak hingga       Nilai fungsi f (x)           Tegak (vertikal)           limx→2     1    =∞
                                                                                       (x−2)2

Limit di tak hingga Variabel x                      Datar (horizontal)         limx→∞  1  =    0
                                                                                       x

Teorema Dasar Pecahan Satuan

Fondasi semua pembahasan limit di tak hingga adalah fakta sederhana ini: untuk

sembarang n > 0,

                                                  1
                                           lim = 0.
                                           x→∞ xn

Karena penyebut membesar tanpa batas sementara pembilangnya tetap, hasilnya

menyusut  menuju  nol.  Inilah  "senjata"  utama    kita:  setiap  suku  yang  mengandung         1
                                                                                                  xn

akan lenyap saat x → ∞.

Limit di Tak Hingga Fungsi Rasional

Untuk fungsi rasional  P (x)  dengan P     dan Q polinomial,  kita  bandingkan derajat
                       Q(x)

pembilang dan penyebut. Trik bakunya: bagi pembilang dan penyebut dengan x

berpangkat tertinggi.

• Derajat pembilang = derajat penyebut: limit adalah rasio koefisien pangkat

tertinggi. Contoh: limx→∞       3x2 +5  =  3  .
                                2x2 −x     2

                                                 9
• Derajat pembilang < derajat penyebut: limit bernilai 0 (asimtot datar y = 0).

   Contoh: limx→∞  x+1    =  0.
                   x3 +4

• Derajat pembilang > derajat penyebut: limit menuju ±∞ (tidak ada asimtot datar).

Menangani Bentuk Tak Tentu ∞ − ∞ pada Selisih Akar

Nah, ini bagian yang paling sering menjebak. Bentuk seperti

limx→∞ ( x2 + ax − x2 + bx) menghasilkan ∞ − ∞, yang tak tentu. Solusinya:

kalikan dengan bentuk sekawan          ⋅+  ⋅  .
                                       ⋅+  ⋅

Setelah dikalikan, pembilangnya menjadi selisih kuadrat (rasional), sehingga bentuk
tak tentu hilang dan kita bisa membandingkan derajat seperti biasa. Contoh singkat:

               lim (      x2 + 4x − x) = lim                 4x     4
                                                                 = = 2.
               x→∞                                      x→∞  x2 + 4x + x 2

Perangkap Kritis: Menuju Negatif Tak Hingga

Saat x → −∞, ada dua jebakan yang wajib diwaspadai:

  1. Tanda akar. Ingat bahwa x2 = ∣x∣, bukan x. Ketika x < 0, maka ∣x∣ = −x. Jadi
    saat memfaktorkan x keluar dari akar untuk x → −∞, kita harus menulis
       x2(⋯ ) = −x ⋯. Lupa tanda negatif ini adalah sumber kesalahan paling

    umum!

2. Faktorisasi yang konsisten. Selalu faktorkan pangkat tertinggi secara eksplisit agar
   arah tanda terjaga sampai akhir perhitungan.

Sebagai contoh, limx→−∞      x2 +1  =  limx→−∞       −x      1+1/x2 = −1, bukan +1 — karena di
                              x
                                                             x

sini x2 = −x.

Rangkuman Cepat

• Limit tak hingga → asimtot tegak; limit di tak hingga → asimtot datar.

•  1   → 0 adalah kunci semua limit di tak hingga.
   xn

• Fungsi rasional: bandingkan derajat pembilang dan penyebut.

• Selisih akar: kalikan bentuk sekawan untuk mengubah ∞ − ∞ menjadi bentuk

  rasional.

• Saat x → −∞: hati-hati, x2 = ∣x∣ = −x. Tanda negatif adalah segalanya!

                                                 10
Semangat berlatih, ya — begitu kamu terbiasa dengan trik sekawan dan sadar jebakan
tanda pada negatif tak hingga, soal-soal ini akan terasa jauh lebih ramah.

                                                                                11
Tabel Referensi Ringkas Formula Kunci

Halo! Bab ini merangkum semua formula dan teorema penting dari materi limit dalam
satu tempat, supaya kamu bisa cepat mengingatnya saat mengerjakan soal atau
ujian. Anggap ini sebagai "kartu contekan" pribadimu.

Eksistensi Limit Bilateral

Limit limx→c f (x) hanya ada jika limit kiri dan limit kanan sama-sama menuju nilai

yang sama. Jika keduanya berbeda atau salah satunya tak hingga, limit bilateral tidak
eksis. Ini penting sebagai prasyarat sebelum memakai teorema lain.

Limit Trigonometri Dasar dan Perluasan Koefisien

Bentuk  dasar limx→0       sin x  =  1  dan limx→0         tan x  =   1 diperluas menjadi rasio dengan
                             x                               x

koefisien:

            lim sin(ax) = a , lim tan(ax) = a , lim tan(ax) = a
            x→0 sin(bx) b x→0 tan(bx) b x→0 sin(bx) b

Perhatikan bahwa koefisien pembilang selalu menjadi pembilang hasil, dan koefisien
penyebut menjadi penyebut hasil.

Limit Kosinus dan Bentuk Kuadratik

Catatan kritis: teorema rasio koefisien tidak berlaku untuk kosinus, karena cos(ax) →
cos(0) = 1 = 0 saat x → 0. Tidak ada pembuat nol, jadi kita harus memakai identitas

trigonometri lebih dulu.

Identitas esensial:

•  Sudut    rangkap:  cos(2θ)      =    1  −  2  sin2  θ,  sehingga     1  −     cos(kx)  =  2  sin2  (  kx  )
                                                                                                         2

•  Selisih  kosinus:  cos  A  −   cos   B  =     −2  sin   (  A+B  )  sin  (  A−B  )
                                                                2               2

•  Selisih  sinus:  sin A  −  sin    B  =  2  cos  (   A+B    ) sin  (  A−B   )
                                                         2                2

Contoh  1:  limx→0  1−cos(4x)
                    x⋅sin(3x)

Ubah pembilang dengan identitas: 1 − cos(4x) = 2 sin2(2x).

                                                           12
             lim 2 sin2(2x) = 2 ⋅ lim sin(2x) ⋅ lim sin(2x) = 2 ⋅ 2 ⋅ 2 = 8
             x→0 x sin(3x)              x→0 x x→0 sin(3x)                       33

Contoh  2:  limx→0  cos(5x)−cos(3x)
                             x2

Gunakan selisih kosinus dengan A = 5x, B = 3x: pembilang menjadi
−2 sin(4x) sin(x).

                     lim       −2 sin(4x) sin(x)    =  −2    ⋅  4  ⋅  1  =  −8
                                        x2
                     x→0

Limit di Tak Hingga untuk Rasio Polinomial

Distingsi terminologi yang sering tertukar:

Kategori             Definisi                                               Asimtot

Limit tak hingga     x → c berhingga, f (x) → ±∞                            Asimtot tegak x = c
                                                                            Asimtot datar y = L
Limit di tak hingga  x → ±∞, f (x) → L

Teorema pecahan satuan: untuk r > 0 rasional,

                                     1                          1
                            lim = 0 dan lim = 0
                     x→∞ xr                         x→−∞ xr

(asalkan xr terdefinisi untuk x < 0).

Untuk rasio  polinomial f (x)  =     P (x)  dengan  derajat  pembilang      n dan penyebut m,
                                     Q(x)

perilaku x → ±∞ ditentukan perbandingan derajat:

•n  =   m: limit sama dengan rasio koefisien pangkat tertinggi,             an ; garis y  =  an  adalah
                                                                                             bm
                                                                            bm

asimtot datar.

• n < m: penyebut bertumbuh lebih cepat, sehingga limit = 0; sumbu-x (y = 0)

  adalah asimtot datar.

                                            13
• n > m: pembilang bertumbuh lebih cepat, sehingga limit menuju ±∞ (tidak ada

  asimtot datar).

Selisih Akar Kuadrat dan Akar pada Negatif Tak Hingga

Saat menemui bentuk a − b pada limit di tak hingga, kalikan dengan bentuk

sekawan  a+  b untuk menghilangkan bentuk tak tentu ∞ − ∞. Hati-hati ketika x →
         a+
             b

−∞: karena x negatif, x2 = ∣x∣ = −x. Kelalaian di sini adalah sumber kesalahan

paling umum—selalu periksa tanda sebelum menyederhanakan akar!

Semoga ringkasan ini memudahkan belajarmu. Latihan rutin adalah kunci!

             14
