---
mode: detailed
pages: 22
words: 3737
---

pelajarin.ai

                                                                      1
Pendahuluan dan Motivasi Fisis-Geometris Turunan

Dari Dua Persoalan Klasik Menuju Satu Konsep: Turunan

Halo! Sebelum masuk rumus, mari kita pahami dulu mengapa turunan ada. Konsep ini
lahir dari dua persoalan yang tampak tidak berhubungan, tetapi ternyata memiliki
struktur matematis yang identik.

Masalah Garis Singgung Geometris

Pertanyaan besarnya: bagaimana menentukan gradien garis singgung tepat di satu
titik pada kurva lengkung non-linear? Kita tidak bisa langsung memakai rumus gradien
dua titik karena hanya ada satu titik.

Solusinya bertahap. Ambil dua titik pada kurva, yaitu (c, f (c)) dan (c + h, f (c + h)).

Garis yang menghubungkan keduanya disebut garis sekan (tali busur), dengan
gradien:

msekan = f (c + h) − f (c)
                     h

Sekarang, bayangkan h → 0: titik kedua bergerak mendekati titik pertama. Garis sekan

pun berkonvergensi menjadi garis singgung, sehingga:

m = lim msekan = lim f (c + h) − f (c)
h→0                   h→0           h

Masalah Kecepatan Sesaat Fisis
Bayangkan partikel bergerak sepanjang garis lurus dengan fungsi posisi s(t).
Kecepatan rata-rata pada selang [t0, t0 + Δt] adalah rasio perubahan posisi

terhadap waktu:

vrata-rata  =  Δs  =  s(t0  + Δt)   − s(t0)
               Δt               Δt

Untuk memperoleh kecepatan sesaat pada detik t0, kita ambil limit selang waktu

mendekati nol:

                      2
                              v(t0)  =     lim   s(t0  +  Δt)  −  s(t0)
                                                           Δt
                                           Δt→0

Kesetaraan Struktur Matematis

Perhatikan kedua rumus di atas — keduanya berbentuk limit dari kuosien diferensi.

Inilah inti definisi formal turunan: jika f terdefinisi pada interval buka yang memuat x,

maka

                              f ′(x) = lim f (x + h) − f (x)
                                           h→0            h

asalkan limit tersebut ada dan bernilai bilangan riil berhingga. Geometri memberi kita
"kemiringan", fisika memberi kita "laju perubahan" — matematika menyatukannya
dalam satu operator.

Sistem Notasi Turunan

Notasi          Penulisan                              Konteks Penggunaan

Lagrange        f ′(x), f ′′(x), … , f (n)(x) Umum, ringkas untuk fungsi
(aksen)

Leibniz         dy ,    d2 y  ,…  ,  dn y              Menekankan rasio perubahan; sangat
(diferensial)           dx2          dxn               berguna pada aturan rantai
                dx
                                                       Penekanan pada turunan sebagai operator
Operator Euler  Dxy, Dx2y

Titik Newton    y˙, y¨                                 Lazim dalam mekanika fisika, turunan

                                                       terhadap waktu t

Setiap notasi punya "kepribadian": Leibniz menunjukkan dari mana ke mana
perubahan diukur, sementara Newton menegaskan bahwa yang berubah adalah
fungsi terhadap waktu. Menguasai keempatnya akan sangat membantu saat
membaca literatur berbeda. Semangat belajar!

                                                 3
Definisi dan Konsep Fundamental Turunan

Definisi Formal Turunan
Turunan fungsi f di titik x didefinisikan sebagai limit kuosien diferensi:

                f ′(x) = lim f (x + h) − f (x)
                         h→0               h

Definisi ini menangkap makna turunan sebagai laju perubahan sesaat. Kuosien
diferensi di dalam limit adalah kemiringan tali busur antara dua titik pada kurva; ketika

h menuju nol, tali busur itu "menempel" pada kurva dan menjadi garis singgung. Agar

turunan ada, limit tersebut harus bernilai bilangan riil berhingga — jika limitnya tak
hingga atau tidak ada, fungsi tidak terdiferensialkan di titik itu.

Formulasi Alternatif di Satu Titik
Untuk mengevaluasi turunan tepat di satu titik absis x = c, kita bisa memakai bentuk

yang setara:

                   ′(c)  =    lim  f  (x)  −  f  (c)
                                        x  −  c
                f             x→c

Bentuk ini diperoleh dengan substitusi x = c + h, sehingga h = x − c. Kedua rumus

memberi hasil yang sama; pilih yang paling memudahkan perhitungan.

Persamaan Garis Singgung dan Garis Normal
Nilai f ′(c) adalah gradien garis singgung kurva y = f (x) di titik singgung P (c, f (c)).

Garis           Gradien                       Persamaan

Garis singgung  m = f ′(c)                    y − f (c) = f ′(c)(x − c)
Garis normal               1                                     1

                m = − f ′(c)                  y − f (c) = − f ′(c) (x − c)

                                   4
Garis normal tegak lurus terhadap garis singgung di titik yang sama. Syarat tegak

lurus  dua  garis  adalah   m1     ⋅     m2  =  −1.  Jadi  jika  f ′(c)      =  0,  gradien  normal   adalah  −  f  1      .
                                                                                                                     ′ (c)

Penurunan Rumus Turunan Fungsi Dasar

Semua rumus berikut diturunkan langsung dari definisi limit.

Fungsi konstan f (x) = k: karena f (x + h) − f (x) = k − k = 0, maka f ′(x) =

limh→0  0   =  0.
        h

Fungsi linear f (x)  =      x:  kuosiennya       (x+h)−x   =     h     =  1, sehingga  f ′(x)  =    1.
                                                      h          h

Fungsi kuadrat f (x) = x2: jabarkan (x + h)2 = x2 + 2xh + h2, kurangi x2, lalu bagi h:

                            f ′(x) = lim 2xh + h2 = lim(2x + h) = 2x
                                         h→0 h                   h→0

Fungsi resiprokal f (x)         =  1  :  samakan     penyebut          lalu  sederhanakan:
                                   x

                   f ′(x)   =      lim   1   ⋅  x − (x + h)   =        lim      −1     =         1
                                         h       x(x + h)                    x(x + h)         − x2
                                   h→0                                 h→0

Fungsi akar f (x) = x: kalikan dengan bentuk sekawan:

        f ′(x) = lim        x+h−             x⋅      x+h+              x = lim            1           =1
                                 h                   x+h+              x h→0         x+h+           x 2x
                       h→0

Kelimanya   konsisten dengan aturan pangkat:                  d        [xn]  =   nxn−1, dengan      1  =  x−1
                                                              dx                                    x

memberi −x−2 dan            x   =  x1/2      memberi  1    x−1/2    .
                                                      2

                                                           5
Turunan Sepihak dan Keterdiferensialan

Halo! Mari kita bedah bagaimana kita menentukan apakah sebuah fungsi benar-
benar "mulus" di suatu titik. Kuncinya ada pada turunan dari dua arah.

Turunan Kiri dan Turunan Kanan

Turunan kiri di titik c melihat bagaimana fungsi berperilaku saat kita mendekati c dari

sisi kiri:

                            f−′ (c)  =  lim   f (x)  −  f (c)
                                                  x  −  c
                                        x→c−

Sedangkan turunan kanan mendekat dari sisi kanan:

                            f+′ (c)  =  lim   f (x)  −  f (c)
                                                  x  −  c
                                        x→c+

Teorema Eksistensi Turunan Bilateral: Fungsi f terdiferensialkan di c jika dan hanya

jika kedua turunan sepihak ada dan bernilai sama:

         f terdiferensialkan di c ⟺ f−′ (c) = f+′ (c) = L ∈ R

Jika kedua nilai tidak sama, atau salah satunya bernilai ±∞, maka f tidak
terdiferensialkan di c.

Empat Penyebab Kegagalan Keterdiferensialan
Grafik gagal memiliki garis singgung tunggal bergradien berhingga pada kondisi
berikut:

Kondisi               Ciri                                     Contoh di x =
                                                               0

Titik sudut (corner)  Gradien kiri = gradien kanan            f (x) = ∣x∣

                                        6
Titik kuspid (cusp)           Kemiringan menuju ±∞ dengan tanda                               f (x) = x2/3
                                                                                              f (x) = x1/3
Garis singgung                berlawanan
vertikal
                              Kuosien menuju ∞ dari kedua arah secara

                              konsisten

Diskontinuitas                Kurva terputus (loncat, tak hingga, atau                        —

                              lubang)

Untuk f (x) = ∣x∣: dari kiri f−′ (0) = −1, dari kanan f+′ (0) = 1. Karena −1 = 1,

turunannya tidak ada. Untuk f (x) = x2/3: f−′ (0) → −∞ dan f+′ (0) → +∞. Untuk

f (x) = x1/3: limitnya   1    → +∞ dari kedua arah.
                        x2/3

Teorema: Terdiferensialkan ⟹ Kontinu

Jika f terdiferensialkan di c, maka f kontinu di c.

Buktinya elegan. Kita perlu menunjukkan limx→c[f (x) − f (c)] = 0. Gunakan trik

perkalian:

lim[f (x)               −  f (c)]  =  lim  [ f (x)  −  f (c)  ⋅  (x  −  c)]  =  f ′(c)  ⋅  0  =  0
                                                 x  −  c
x→c                                   x→c

Karena f ′(c) berhingga dan (x − c) → 0, hasilnya nol—persis definisi kekontinuan.

Peringatan Penting

Konvers tidak berlaku! Kontinu tidak menjamin terdiferensialkan. Ingat f (x) = ∣x∣ di
x = 0: fungsinya kontinu (tidak ada lompatan), tetapi tajam di tengah sehingga gagal

punya turunan. Jadi keterdiferensialan adalah syarat yang lebih kuat daripada
kekontinuan. Selamat belajar!

                                                    7
Aturan-Aturan Dasar Pencarian Turunan

Sampai di sini kita sudah paham bahwa keterdiferensialan lebih kuat daripada

kekontinuan: fungsi kontinu belum tentu punya turunan (contohnya f (x) = ∣x∣ di x = 0

yang bersudut tajam). Nah, sekarang kita masuk ke "perkakas" utama untuk
menghitung turunan tanpa harus selalu memakai definisi limit. Yuk, kita bedah satu per
satu!

Teorema-Teorema Aljabar Diferensiasi
Misalkan u = f (x) dan v = g(x) adalah fungsi yang terdiferensialkan, dan c konstanta

riil.
1. Aturan Pangkat Umum (Power Rule):

                                       d [xn] = n xn−1, n ∈ R
                                      dx

2. Aturan Kelipatan Konstanta:

                                         d [c ⋅ f (x)] = c ⋅ f ′(x)
                                        dx

3. Aturan Jumlahan dan Selisih:

                                  d [f (x) ± g(x)] = f ′(x) ± g′(x)
                                  dx

4. Aturan Perkalian (Product Rule):

                                          d [u ⋅ v] = u′v + uv′
                                         dx

Hati-hati: turunan perkalian bukan hasil kali turunan! Untuk membuktikannya, kita

tambahkan dan kurangkan suku perantara u(x + h)v(x) pada pembilang:

                                                                                8
              lim u(x + h)v(x + h) − u(x + h)v(x) + u(x + h)v(x) − u(x)v(x)
              h→0                                         h

Lalu dikelompokkan menjadi dua bagian; karena u terdiferensialkan maka u kontinu
sehingga limh→0 u(x + h) = u(x). Hasil akhirnya tepat u(x)v′(x) + v(x)u′(x).

5. Aturan Pembagian (Quotient Rule):

                                     d   [u]  =  u′v  −   uv′  ,  v(x) = 0
                                     dx   v           v2

Mnemonik: [Turunan Atas × Bawah] dikurang [Atas × Turunan Bawah], seluruhnya
dibagi [Bawah Kuadrat]. Mudah diingat, kan?

Turunan Tingkat Tinggi

Jika turunan suatu fungsi masih bisa diturunkan lagi, prosesnya boleh diulang:

Turunan Notasi                           Makna

Kedua             f ′′(x)   =  d2y       Laju perubahan gradien (kelengkungan/kecekungan kurva)
Ketiga                         dx2       Dalam kinematika disebut jerk (sentakan)
                                         Diferensiasi berulang
Ke-n              f ′′′(x)  =   d3y
                                dx3

                  f (n)(x) = dny
                               dxn

Dalam fisika kinematika, rantainya indah: posisi s(t) → kecepatan v(t) = s′(t) →
percepatan a(t) = s′′(t) → jerk = s′′′(t). Jadi turunan kedua mengukur bagaimana

kecepatan berubah, sekaligus menggambarkan kecekungan kurva.

Turunan Fungsi Trigonometri

Sebagai bonus, berikut enam formula pokok:

1.  d   [sin  x]  =  cos  x
    dx

2.  d   [cos  x]  =  −  sin  x
    dx

                                                      9
3.  d   [tan  x]  =  sec2  x
    dx

4.  d   [cot  x]  =  −  csc2  x
    dx

5.  d   [sec  x]  =  sec  x  tan  x
    dx

6.  d   [csc  x]  =  −  csc  x  cot  x
    dx

Kaidah tanda: setiap fungsi berawalan "co-" (kosinus, kotangen, kosekan)

menghasilkan turunan bertanda negatif. Pola ini akan sangat membantu mengingat!

Dengan aturan-aturan ini, kamu bisa menuruni fungsi yang jauh lebih rumit hanya
dengan kombinasi langkah-langkah sederhana. Selamat berlatih!

                                        10
Turunan Fungsi Trigonometri

Enam Formula Pokok Turunan Trigonometri

Halo! Mari kita pelajari turunan fungsi trigonometri. Intinya sederhana: kita punya enam
rumus dasar yang perlu dihafal, lalu aturan tanda khusus untuk fungsi berawalan "co-".
Yuk, kita bedah satu per satu.

Fungsi f (x)                     Turunan f ′(x)

sin x                            cos x

cos x                            − sin x
tan x                            sec2 x

cot x                            − csc2 x

sec x                            sec x tan x

csc x                            − csc x cot x

Kaidah Tanda untuk Fungsi Berawalan "co-"

Perhatikan pola menarik: fungsi kosinus, kotangen, dan kosekan (yang berawalan
"co-") semuanya memiliki turunan bertanda negatif. Sebaliknya, sinus, tangen, dan
sekan bertanda positif. Jadi jika kamu lupa satu tanda, ingat saja aturan ini — fungsi
"co-" selalu membawa tanda minus. Ini akan sangat menyelamatkanmu saat ujian!

Pembuktian Turunan sin x = cos x

Pembuktian ini berangkat dari definisi kuosien diferensi:

              f ′(x) = lim sin(x + h) − sin x
              h→0                       h

Langkah 1 — terapkan identitas penjumlahan sudut sin(x + h) = sin x cos h +
cos x sin h, sehingga:

                             11
                          = lim sin x cos h + cos x sin h − sin x
                          h→0                       h

Langkah 2 — kelompokkan dan gunakan dua limit trigonometri fundamental:

                          lim cos h − 1 = 0 dan lim sin h = 1
                          h→0 h                        h→0 h

Hasilnya:

                          = sin x ⋅ (0) + cos x ⋅ (1) = cos x

Terbukti! Limit fundamental inilah kunci seluruh pembuktian.

Pembuktian Turunan tan x = sec2 x

Kita  nyatakan tan x  =   sin x                 Aturan Pembagian:
                          cos x , lalu gunakan

                      d   [ sin x ]  =  (cos x)(cos x) − (sin x)(− sin x)
                      dx   cos x                        cos2 x

Perhatikan tanda negatif dari turunan kosinus. Sederhanakan pembilangnya menjadi

cos2 x + sin2 x. Dengan identitas Pythagoras cos2 x + sin2 x = 1:

                                        =    1     =  sec2  x
                                           cos2 x

Selesai! Pembuktian ini menunjukkan betapa eratnya turunan trigonometri dengan
identitas Pythagoras — sebuah koneksi yang elegan dan sering muncul di soal
lanjutan.

Semangat belajar terus, ya! Kuasai keenam rumus dan kaidah tandanya, maka
sebagian besar soal turunan trigonometri akan terasa jauh lebih mudah.

                                                12
Aturan Rantai (Chain Rules)

Memahami Aturan Rantai

Aturan rantai adalah salah satu "senjata utama" dalam kalkulus. Ia dipakai ketika kita
harus menurunkan fungsi komposisi, yaitu fungsi yang "bersarang" di dalam fungsi

lain, seperti f (g(x)). Tanpa aturan ini, menurunkan fungsi komposisi akan sangat

merepotkan. Yuk, kita bedah pelan-pelan.

Dua Notasi, Satu Makna

Aturan rantai dapat dituliskan dalam dua gaya notasi yang setara:

  • Notasi Leibniz: jika y = f (u) dan u = g(x), maka

                                                dy = dy ⋅ du
                                                dx du dx

    Di sini kita "memecah" laju perubahan menjadi dua tahap: perubahan y terhadap u,
    lalu u terhadap x.

  • Notasi Lagrange (prime):

                                      [f (g(x))]′ = f ′(g(x)) ⋅ g′(x)

    Versi ini menegaskan bahwa turunan dievaluasi pada fungsi dalam, bukan pada x.

Kedua bentuk menyatakan hal yang sama. Pilih saja yang lebih nyaman untuk soal
yang sedang kamu kerjakan.

Kaidah Kerja: Luar Dulu, Dalam Kemudian

Cara mengingatnya sederhana dan sering disebut "turunkan dari luar ke dalam":
  1. Turunkan fungsi luar sambil mempertahankan fungsi dalam apa adanya.
 2. Kalikan dengan turunan fungsi dalam.

Contoh: untuk y = (3x + 2)4, fungsi luar adalah pangkat empat, fungsi dalam 3x + 2.
Hasilnya y′ = 4(3x + 2)3 ⋅ 3 = 12(3x + 2)3. Perhatikan bahwa 3x + 2 tetap utuh saat

kita menurunkan bagian luar — ini kuncinya.

                                                                               13
Aturan Pangkat yang Diperumum
Untuk bentuk [u(x)]n dengan u fungsi yang dapat diturunkan, berlaku:

                                    d [u(x)]n = n [u(x)]n−1 ⋅ u′(x)
                                   dx

Rumus ini adalah kasus khusus aturan rantai yang paling sering muncul. Contoh:

turunan (x2 sin x)5 adalah 5 (x2 sin x)4 ⋅ (2x sin x + x2 cos x), di mana bagian terakhir

adalah turunan fungsi dalamnya.

Aturan Rantai Berlapis

Bagaimana jika komposisinya tiga fungsi atau lebih? Aturan rantai tetap berlaku —
cukup kalikan setiap lapisan turunannya, dari lapisan terluar hingga terdalam. Untuk

y = f (g(h(x))):

              dy = f ′(g(h(x))) ⋅ g′(h(x)) ⋅ h′(x)
              dx

Semakin banyak lapisan, semakin banyak faktor yang dikalikan. Tips praktisnya:
kerjakan satu lapisan per baris agar tidak ada yang terlewat.

Ringkasan Cepat

Konsep        Rumus                            Catatan

Leibniz       dy = dy ⋅ du                     Cocok untuk substitusi bertahap
Lagrange                                       Evaluasi pada fungsi dalam
              dx du dx

              [f (g(x))]′ = f ′(g(x)) ⋅ g′(x)

Pangkat umum  [u]n → n[u]n−1u′                 Kasus paling umum

Berlapis      f ′ ⋅ g′ ⋅ h′                    Satu faktor per lapisan

Dengan menguasai pola "luar–dalam" ini, kamu akan siap menangani berbagai fungsi
komposisi, termasuk yang tampil dalam soal garis singgung dan turunan fungsi
sepotong-sepotong. Selamat berlatih!

                                14
Contoh Soal dan Pembahasan Langkah-demi-Langkah

Menerapkan Aturan Turunan pada Soal Konkret

Halo! Yuk, kita latihan bersama. Bab ini menerapkan semua aturan turunan yang
sudah kamu pelajari ke soal nyata.

1. Garis Singgung dan Garis Normal

Untuk kurva y = f (x) di titik berabsis x = c, gradien garis singgung adalah ms = f ′(c).

Persamaan garisnya:

                         y − f (c) = f ′(c)(x − c)

                                                                                            1
Garis normal tegak lurus garis singgung, sehingga gradiennya mn = − f ′(c) (syarat
f ′(c) = 0). Langkah kerjanya: cari f (c), hitung f ′(x), substitusikan c, lalu susun

persamaan.

2. Uji Keterdiferensialan Fungsi Sepotong-sepotong

Fungsi sepotong-sepotong diferensialkan di titik sambungan x = c bila dua syarat

terpenuhi:

Uji                      Keterangan

Kekontinuan              limx→c− f (x) = limx→c+ f (x) = f (c)
Turunan kiri = kanan     limx→c− f ′(x) = limx→c+ f ′(x)

Jika salah satu gagal, fungsi tidak terdiferensialkan di c (contohnya titik sudut atau

lompatan).

3. Aturan Perkalian dan Pembagian

Misal  y  =  x sin x                                 aturan pembagian dengan  u  =
             x2 + 1 . Bentuknya rasio, jadi gunakan
x sin x dan v = x2 + 1:

                                   15
                                        (  u    ′  =  u′v −   uv′
                                                          v2
                                           v  )

Turunan pembilang memakai aturan perkalian: u′ = sin x + x cos x, sedangkan v′ =
2x. Maka:

                     y′   =  (sin x  +  x cos x)(x2 + 1)      −    (x sin x)(2x)
                                                (x2 + 1)2

4. Aturan Rantai Berlapis

Untuk y = cos3(4x2 − 1), uraikan dari luar ke dalam:

• Terluar: y  =  u3  ⇒  dy  =  3u2
                        du

• Tengah:  u  =  cos w    ⇒  du  =  − sin w
                             dw

• Terdalam: w    =   4x2  −1   ⇒  dw  =    8x
                                  dx

Kalikan bertingkat:

                        dy = 3 cos2(4x2 − 1) ⋅ ( − sin(4x2 − 1)) ⋅ 8x
                        dx

                                = −24x cos2(4x2 − 1) sin(4x2 − 1)

Kunci sukses: kenali lapisan fungsi, turunkan satu per satu, lalu kalikan. Semangat
berlatih!

                                                      16
Tabel Referensi Ringkas Formula Turunan

Halo! Bab ini adalah "lembar contekan" turunan yang bisa kamu buka kapan saja saat
latihan soal. Tujuannya sederhana: menyatukan semua formula yang sudah kita
pelajari—dari definisi paling dasar sampai gradien garis normal—dalam satu tempat
supaya mudah diingat dan dipakai. Yuk, kita rangkum bersama!

1. Fondasi: Definisi Kuosien Diferensi

Sebelum masuk ke aturan praktis, ingat dulu bahwa turunan berasal dari kuosien

diferensi (selisih bagi), yaitu limit laju perubahan rata-rata ketika perubahan x

mendekati nol:

                          f ′(x) = lim f (x + h) − f (x)
                                          h→0               h

Konsep kunci yang perlu kamu pegang dari definisi ini:

• Turunan = laju perubahan sesaat, bukan lagi rata-rata, karena h dibuat mengecil

  menuju nol.

•  Notasi  yang  umum  dipakai:  f ′(x),  dy  ,  atau  y′.  Semuanya  merujuk  pada  hal  yang
                                          dx

   sama.

• Interpretasi geometris: nilai f ′(a) adalah gradien garis singgung kurva di titik
 x = a.

• Definisi ini adalah "ibu" dari semua aturan di bawah—setiap aturan praktis
  sebenarnya bisa diturunkan dari sini, hanya saja jauh lebih lambat.

  Tips: Kalau lupa sebuah aturan, kamu selalu bisa kembali ke definisi limit ini.
Memang lebih panjang, tapi selalu benar.

2. Aturan Dasar Turunan

Tiga aturan ini adalah bekal minimum yang wajib hafal di luar kepala.

Nama Aturan      Formula                  Catatan

                                                 17
Aturan            d (c) = 0          Turunan bilangan konstan selalu nol, karena
konstanta                            garisnya horizontal (tidak berubah).
                  dx
Aturan
pangkat           d (xn) = n xn−1    Pangkat turun satu, lalu pangkat lama menjadi
                                     koefisien. Berlaku untuk pangkat bilangan real.
Kelipatan         dx
konstanta
                  d (c ⋅ f (x)) =    Konstanta boleh "keluar" dari operasi turunan.

                  dx

                  c ⋅ f ′(x)

Contoh cepat:

• y = 7 ⇒ y′ = 0

• y = x5 ⇒ y′ = 5x4

• y = 3x4 ⇒ y′ = 12x3

Aturan pangkat juga berlaku untuk pangkat negatif       dan pecahan, misalnya y   =   1  =
                                                                                      x

x−1 ⇒ y′ = −x−2, dan y =     x    =  x1/2  ⇒  y′  =  1  x−1/2  .
                                                     2

3. Aturan Perkalian dan Pembagian

Saat dua fungsi "bertemu", kita tidak bisa asal menurunkan masing-masing. Gunakan
aturan berikut.

Aturan                 Formula             Cara Mengingat

Aturan perkalian       (u ⋅ v)′ =          "Turunkan yang pertama kali yang kedua,
(product rule)         u′v + uv′           tambah yang pertama kali turunkan yang
                                           kedua."

                       (  u    ′  =

Aturan pembagian             )             Penyebut dikuadratkan; urutan pengurangan
(quotient rule)        u′vv − uv′
                                           u′v − uv′ penting—jangan dibalik!

                             v2

Contoh aturan perkalian: y = x2 ⋅ sin x

                  y′ = (2x)(sin x) + (x2)(cos x) = 2x sin x + x2 cos x

                                              18
Contoh aturan pembagian: y   =     x2
                                 x+1

                   y′  =     (2x)(x +      1) − (x2)(1)         =  x2 + 2x
                                     (x    + 1)2                   (x + 1)2

⚠  Jebakan  umum:  (u ⋅ v)′  =  u′  ⋅ v′  dan  ( u )′  =  u′  .  Selalu  pakai  aturan  yang
                                                            v′
                                                  v

benar!

4. Formula Trigonometri Lengkap

Turunan fungsi trigonometri punya pola yang rapi—perhatikan tanda dan
pasangannya.

Fungsi                                          Turunan

sin x                                           cos x

cos x                                           − sin x

tan x                                           sec2 x

cot x                                           − csc2 x

sec x                                           sec x tan x

csc x                                           − csc x cot x

Pola yang membantu mengingat:

  • Fungsi yang "diawali" dengan co (cos, cot, csc) menghasilkan turunan bertanda

    negatif.

  • sin dan cos saling bertukar; tan dan sec "berpasangan" dalam hasil turunannya.
Contoh: y = 3 sin x − 2 cos x ⇒ y′ = 3 cos x + 2 sin x.

                                                19
5. Aturan Rantai (Chain Rule)

Untuk fungsi komposisi (fungsi di dalam fungsi), kita butuh aturan rantai. Inilah aturan
yang paling sering muncul di soal-soal lanjutan.
Bentuk Leibniz:

                                              dy = dy ⋅ du
                                              dx du dx

Aturan pangkat rantai (bentuk paling praktis untuk fungsi berpangkat):

                                   d [f (x)]n = n[f (x)]n−1 ⋅ f ′(x)
                                  dx
Contoh: y = (3x2 + 1)4

                             y′ = 4(3x2 + 1)3 ⋅ (6x) = 24x(3x2 + 1)3

Contoh trigonometri komposisi: y = sin(2x)

                                     y′ = cos(2x) ⋅ 2 = 2 cos(2x)

      Cara berpikir aturan rantai: turunkan "kulit luar"-nya dulu (biarkan isi tetap), lalu
   kalikan dengan turunan "isi dalam"-nya. Bisa berlapis lebih dari satu kali bila
   komposisinya bertingkat.

6. Gradien Garis Normal

Setelah tahu gradien garis singgung, kita bisa langsung menentukan garis normal—
garis yang tegak lurus terhadap garis singgung di titik singgung yang sama.

Kunci hubungan tegak lurus: dua garis saling tegak lurus jika hasil kali gradiennya −1,
yaitu m1 ⋅ m2 = −1.

                                                                               20
Maka jika gradien garis singgung di titik x = a adalah mt = f ′(a), gradien garis

normalnya:

                                                           1
                                             mn = − f ′(a)

Langkah menentukan persamaan garis normal:

  1. Hitung f ′(a) untuk mendapat gradien garis singgung mt.
 2. Gradien garis normal: mn = − 1 .

                                          mt
 3. Gunakan bentuk titik-gradien: y − y1 = mn(x − x1), dengan (x1, y1) titik singgung.

4. Sederhanakan persamaannya.

Contoh: Kurva y = x2 di titik (2, 4). Gradien singgung = 2x = 4, sehingga gradien

normal  =  −  1  .  Persamaan  garis  normal:  y  −      4  =  −  1  (x  −  2).
              4                                                   4

⚠ Catatan penting: jika f ′(a) = 0 (garis singgung horizontal), garis normal
menjadi vertikal dengan persamaan x = a.

7. Tabel Rujukan Cepat (Semua dalam Satu Pandangan)

Kategori                                       Formula

Kuosien diferensi                              f ′(x) = limh→0 f (x + h) − f (x)
Konstanta                                                                   h
Pangkat
Kelipatan konstanta                             d (c) = 0
                                               dx
                                                d (xn) = nxn−1
                                               dx
                                               (c f )′ = c f ′

Perkalian                                      (uv)′ = u′v + uv′
Pembagian
                                               (  u    ′  =  u′v − uv′
                                                                 v2
                                                  v  )

                                                     21
sin x                 cos x
cos x                 − sin x
tan x                 sec2 x
cot x                 − csc2 x
sec x                 sec x tan x
csc x                 − csc x cot x
                      dy = dy ⋅ du
Rantai (Leibniz)      dx du dx
Pangkat rantai         d [f (x)]n = n[f (x)]n−1f ′(x)
                      dx
Gradien garis normal
                                   1
                      mn = − f ′(a)

Penutup

Selamat! Kamu sekarang punya satu lembar rujukan yang menampung seluruh
formula turunan dalam bab ini—dari definisi limit, aturan dasar, perkalian dan
pembagian, trigonometri, aturan rantai, hingga gradien garis normal. Saran belajar:
jangan cuma dihafal, tapi coba turunkan ulang beberapa formula dari definisi kuosien
diferensi supaya benar-benar paham "dari mana asalnya". Semakin sering dipakai,
tabel ini akan otomatis menempel di ingatanmu. Semangat berlatih!

                      22
