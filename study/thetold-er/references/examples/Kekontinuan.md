---
mode: detailed
pages: 16
words: 3012
---

pelajarin.ai

Pendahuluan dan Peta Konsep Kekontinuan

Hubungan Fundamental Limit dan Kekontinuan

Halo! Sebelum masuk ke definisi formal, mari kita pahami dulu mengapa limit dan
kekontinuan selalu dibahas berpasangan. Keduanya ibarat dua sisi koin yang sama.

Secara konseptual, limit menelaah perilaku nilai fungsi di sekitar suatu titik, tanpa
memedulikan nilai fungsi tepat di titik itu. Sementara itu, kekontinuan justru
menjembatani keduanya: ia menghubungkan nilai pendekatan limit dengan nilai
fungsi aktual di titik tersebut. Dengan kata lain, fungsi kontinu adalah fungsi yang
"setia" — nilai yang didekati sama dengan nilai yang benar-benar dimiliki.

Makna Geometris: Kurva Tanpa Putusan

Secara visual, grafik fungsi disebut kontinu pada suatu selang jika kurvanya dapat
digambarkan mulus — tanpa putusan, lompatan, atau "pengangkatan pena" dari
bidang gambar. Bayangkan menggambar satu tarikan garis tanpa mengangkat
pensil: itulah intuisi kekontinuan.

Landasan Analitis versus Persepsi Visual

Meski intuisi gambar membantu, kalkulus modern menuntut landasan analitis yang
ketat. Kita tidak boleh bergantung pada persepsi visual semata, karena grafik bisa
menipu di skala tertentu. Karena itu, kekontinuan dirumuskan lewat syarat-syarat
formal berbasis limit.

Tiga Pilar Peta Konsep Kekontinuan

Pilar                   Cakupan Materi

1. Kekontinuan di Satu  Tiga syarat formal kekontinuan dan klasifikasi jenis-jenis
Titik                   diskontinuitas

2. Kekontinuan          Definisi kontinu kiri dan kontinu kanan, kekontinuan pada selang
Sepihak dan pada        tertutup, serta Teorema Nilai Antara (Intermediate Value
Interval                Theorem)

                                        1
3. Aplikasi dan    Penentuan nilai parameter konstanta pada fungsi sepotong-
Pemecahan Masalah  sepotong (piecewise) dan redefinisi fungsi kontinu perluasan
                   (extended continuous function)

Dengan peta ini, perjalanan kita akan bergerak dari titik, melebar ke interval, lalu
berujung pada penerapan nyata. Siap? Mari kita mulai!

                   2
Konsep Kekontinuan Fungsi di Satu Titik

Tiga Syarat Formal Kekontinuan di Titik
Misalkan f adalah fungsi yang terdefinisi pada interval buka yang memuat titik x = c.
Fungsi f dikatakan kontinu di titik x = c jika dan hanya jika ketiga syarat analitis

berikut terpenuhi secara simultan:

  1. Syarat 1 — Nilai Fungsi Terdefinisi: f (c) terdefinisi, yaitu c ∈ Df . Titik c harus berada

    di dalam domain alami fungsi, sehingga perhitungan fungsi menghasilkan
    bilangan riil berhingga.

 2. Syarat 2 — Limit Fungsi Ada: limx→c f (x) ada dan berhingga. Artinya, limit kiri dan
    limit kanan di titik c keduanya ada, berhingga, dan bernilai sama: limx→c− f (x) =
    limx→c+ f (x) = L ∈ R.

 3. Syarat 3 — Kesesuaian Nilai: limx→c f (x) = f (c). Nilai kecenderungan pendekatan
    limit di sekitar c harus berimpit sempurna dengan nilai fungsi sebenarnya tepat di
    titik c.

Jika salah satu atau lebih syarat di atas gagal, fungsi f dikatakan diskontinu di titik
x = c.

Taksonomi Diskontinuitas

Kegagalan memenuhi syarat kekontinuan dipetakan ke dalam empat jenis:

Jenis      Kondisi Matematis          Ciri Visual           Sifat

Removable  Limit di c ada (= L),      Grafik mulus dengan   Dapat dihapus dengan
           tetapi f (c) tidak         satu "lubang" (hole)  mendefinisikan ulang
           terdefinisi atau f (c) =
                                      di absis c            nilai fungsi tepat di c
           L

Jump       limx→c− f (x) =           Patahan vertikal      Tidak dapat diperbaiki
           limx→c+ f (x), keduanya    mendadak antar        hanya dengan
                                      tingkat               mengubah nilai di satu
           berhingga                                        titik

                                      3
Infinite  Salah satu atau kedua     Kurva menuju       Tidak dapat dihapus
Osilasi   limit sepihak bernilai    asimtot vertikal   Tidak dapat dihapus

          ±∞

          Limit tidak menuju nilai  Grafik berosilasi
          tunggal karena fungsi     tanpa menetap
          berayun

Diskontinuitas yang Dapat Dihapus (Removable)

Limit fungsi di titik c ada, tetapi f (c) tidak terdefinisi atau berbeda dengan nilai
limitnya. Disebut removable karena kita dapat membuat fungsi baru F (x) yang
kontinu di c cukup dengan mendefinisikan ulang nilai tepat di titik tersebut agar
F (c) = L. Contohnya adalah fungsi dengan grafik mulus yang hanya memiliki satu
"lubang" pada x = c.

Diskontinuitas Loncat (Jump)
Kedua limit sepihak ada dan bernilai riil berhingga, namun nilainya tidak sama. Kurva
mengalami patahan vertikal mendadak dari satu tingkat ke tingkat lain. Jenis ini sering

dijumpai pada fungsi nilai mutlak rasional seperti f (x) = ∣x∣ atau fungsi tangga ⌊x⌋,

                                                                                                         x

dan tidak dapat diperbaiki hanya dengan mengubah nilai pada satu titik tunggal.

Diskontinuitas Tak Hingga
Salah satu atau kedua limit sepihak bernilai tak hingga positif atau negatif. Grafik
umumnya menuju asimtot vertikal, sehingga diskontinuitas ini tidak dapat dihapus.

Diskontinuitas Osilasi

Limit tidak menuju nilai tunggal karena fungsi berayun di sekitar titik c, sehingga nilai

limitnya tidak menetap — jenis ini pun tidak dapat dihapus.

Intinya: mengenali jenis diskontinuitas membantu kita tahu apakah fungsi masih bisa
"diperbaiki" di titik tersebut atau tidak. Semangat belajar, dan terus latih ketiga syarat
formalnya!

                                    4
Sifat Aljabar dan Keluarga Fungsi Kontinu

Halo! Siap melanjutkan petualangan kita di dunia kekontinuan? Kali ini kita akan
membedah aturan-aturan aljabar yang menjaga sifat kontinu tetap utuh, lalu
mengenali keluarga fungsi yang sudah "otomatis" kontinu. Yuk, kita mulai!

Operasi Aljabar yang Mempertahankan Kekontinuan
Bayangkan Anda punya dua fungsi kontinu, f dan g, yang keduanya kontinu di titik
x = c. Misalkan pula k adalah sembarang konstanta skalar riil. Maka ada teorema
penting: hasil kombinasi keduanya juga kontinu di c. Operasi apa saja yang dijamin

aman?

Operasi           Bentuk    Catatan/Syarat

Penjumlahan       f +g      Selalu kontinu

Pengurangan       f −g      Selalu kontinu

Kelipatan skalar  k⋅f       Selalu kontinu

Perkalian         f ⋅g      Selalu kontinu

Pembagian         f         Wajib g(c) = 0
Perpangkatan      g         Untuk n ∈ Z+

                  [f (x)]n

Akar              n f (x)   Syarat f (c) > 0; jika n genap, butuh f (x) ≥ 0

Intinya sederhana: selama tidak ada pembagian dengan nol dan tidak melanggar
syarat akar, kekontinuan otomatis terwarisi. Inilah sebabnya kita jarang repot
menghitung limit satu per satu — cukup kenali "bahan dasarnya".

Keluarga Fungsi Standar yang Kontinu

Sekarang bagian yang paling melegakan: beberapa keluarga fungsi sudah kontinu by
default.

  • Fungsi polinomial, P (x) = anxn + ⋯ + a0, kontinu di seluruh garis bilangan riil
    (−∞, ∞). Tidak ada pengecualian!

                            5
• Fungsi rasional, R(x)  =  P (x)  ,  kontinu  di  seluruh  domain  aslinya,  yaitu  setiap  titik
                            Q(x)

dengan Q(x) = 0. Titik di mana penyebut nol justru menjadi asimtot tegak — ingat

diskontinuitas tak hingga dengan bentuk khas seperti f (x)          =     1    .
                                                                       (x−c)2

• Fungsi trigonometri sin x dan cos x kontinu pada seluruh R. Sementara tan x, cot x,
 sec x, dan csc x kontinu di setiap titik dalam domainnya masing-masing.

Rangkuman Cepat

Kombinasi ketiga fakta ini sangat powerful: karena polinomial kontinu dan sin x, cos x

kontinu, maka hampir semua fungsi "cantik" yang Anda temui di kalkulus tersusun dari
operasi aljabar yang menjaga kekontinuan. Anda cukup memeriksa penyebut tak nol
dan syarat akar untuk menentukan titik diskontinuitas. Semangat, Anda sudah
selangkah lebih dekat memahami kekontinuan secara utuh!

                                                   6
Kontinu Sepihak: Kiri dan Kanan

Kekontinuan pada Interval Tertutup
Ketika kita bicara kekontinuan pada interval tertutup [a, b], ada nuansa penting di
kedua ujung interval. Fungsi f dikatakan kontinu pada interval tertutup [a, b] jika

memenuhi tiga kriteria:

  1. f kontinu pada interval terbuka (a, b).
 2. f kontinu kanan di titik ujung kiri a: limx→a+ f (x) = f (a).
 3. f kontinu kiri di titik ujung kanan b: limx→b− f (x) = f (b).

Perhatikan pola: di ujung kiri kita hanya bisa mendekat dari kanan (karena domain

tidak mencakup x < a), jadi yang relevan adalah limit kanan. Sebaliknya di ujung

kanan, yang relevan adalah limit kiri.

Definisi Kontinu Kiri dan Kanan
  • Kontinu kiri di c: f kontinu kiri di titik c jika limx→c− f (x) = f (c).
  • Kontinu kanan di c: f kontinu kanan di titik c jika limx→c+ f (x) = f (c).

Keduanya menuntut nilai fungsi terdefinisi di c dan limit sepihak yang sesuai sama

dengan nilai itu.

Teorema Relasi Bilateral

Hubungan keduanya dirangkum dalam teorema berikut:

Kondisi                                   Kesimpulan

f kontinu kiri dan kontinu kanan di c     f kontinu (bilateral) di c

f kontinu di c                            f kontinu kiri dan kanan di c

Jadi kekontinuan biasa setara dengan kekontinuan kedua arah sekaligus.

                                       7
Penerapan pada Titik Sambung Piecewise

Pada fungsi sepontong-sepotong, titik sambung adalah kandidat utama

diskontinuitas. Contoh: f (x)  =    x2 −4  untuk x  =  2, dan f (2)  =  5. Mari uji di x  =  2 melalui
                                    x−2

tiga syarat:

1. Nilai fungsi: f (2) = 5 terdefinisi. ✓

2. Nilai limit: limx→2  (x−2)(x+2)  =  limx→2(x + 2)    =  4. ✓
                             x−2

3. Kesesuaian: 4 = 5, sehingga limit tidak sama dengan nilai fungsi.

Karena syarat ketiga gagal, f tidak kontinu di x = 2 — ini diskontinuitas yang dapat

dihapus (removable).

Kaitan dengan Teorema Nilai Antara

Kekontinuan sepihak ini menjadi fondasi Teorema Nilai Antara (IVT): jika f kontinu
pada [a, b] dan N terletak di antara f (a) dan f (b), maka ada c ∈ (a, b) dengan
f (c) = N . Syarat mutlaknya: f harus kontinu tanpa putus pada seluruh [a, b] —

termasuk kontinu sepihak di kedua ujungnya. Jika ada satu titik diskontinuitas saja,

kesimpulan gagal. Korolarinya adalah Teorema Lokasi Akar (Bolzano): bila f (a) ⋅
f (b) < 0, persamaan f (x) = 0 punya setidaknya satu akar riil di (a, b).

                                           8
Kekontinuan pada Interval

Kekontinuan pada Interval Terbuka (a, b)

Sebuah fungsi f dikatakan kontinu pada interval terbuka (a, b) apabila f kontinu di
setiap titik c di dalam interval tersebut. Dengan kata lain, untuk setiap c ∈ (a, b), harus

berlaku tiga syarat kekontinuan di titik, yaitu:

1. limx→c f (x) ada,
2. f (c) terdefinisi, dan

3. limx→c f (x) = f (c).

Fungsi polinomial dan fungsi linear adalah contoh yang paling aman — keduanya

kontinu  di  seluruh  garis  bilangan  riil.  Pada  Contoh  Soal  2,  potongan  g(x)  =  ax  −  3
                                                                                                2

untuk x < 2 (polinomial kuadratik) kontinu di (−∞, 2), sedangkan g(x) = 2x + a untuk

x ≥ 2 (linear) kontinu di (2, ∞). Jadi satu-satunya titik yang perlu diperiksa hanyalah

titik sambung x = 2.

Kekontinuan pada Interval Tertutup [a, b]

Untuk interval tertutup, aturannya sedikit berbeda dan menarik. Fungsi f dikatakan
kontinu pada [a, b] jika:

  • f kontinu pada interval terbuka (a, b), dan

  • f kontinu kanan di titik ujung kiri a, dan

  • f kontinu kiri di titik ujung kanan b.

Apa maksudnya? Di titik ujung, kita tidak bisa mengambil limit dua arah karena fungsi
tidak terdefinisi di luar interval. Karena itu, kita cukup memperhatikan arah dari dalam
interval.

Syarat Kontinu Kanan di Titik Ujung Kiri a

Fungsi kontinu kanan di a jika:

                                            lim f (x) = f (a)

                                                              x→a+

Artinya, nilai limit saat x mendekati a dari arah kanan (dari dalam interval) harus
sama dengan nilai fungsi di a.

                                                    9
Syarat Kontinu Kiri di Titik Ujung Kanan b

Fungsi kontinu kiri di b jika:

                                        lim f (x) = f (b)

                                        x→b−

Artinya, nilai limit saat x mendekati b dari arah kiri harus sama dengan nilai fungsi di b.

     Tips mengingat: "kanan" mengacu pada arah datangnya x menuju titik ujung. Di
   ujung kiri a, kita hanya bisa datang dari kanan; di ujung kanan b, kita hanya bisa

   datang dari kiri.

Menerapkan Syarat pada Titik Sambung

Saat fungsi didefinisikan secara sepotong-sepotong (piecewise), titik sambung adalah
tempat paling rawan terjadi ketidakkontinuan. Strategi umumnya:

Langkah  Yang dilakukan

1        Hitung nilai fungsi di titik sambung, f (c)

2        Hitung limit kiri limx→c− f (x)

3        Hitung limit kanan limx→c+ f (x)

4        Terapkan syarat: limit kiri = limit kanan = f (c)

Contoh satu parameter (Contoh Soal 2): Agar g kontinu di x = 2, kita samakan limit kiri

dan kanan:

         4a − 3 = 4 + a                 ⇒   3a = 7              ⇒  a=  7
                                                                       3

Jadi  g  kontinu di seluruh R jika dan  hanya jika  a  =  7  .
                                                          3

Contoh dua parameter (Contoh Soal 3): Fungsi h memiliki dua titik sambung, x = 1
dan x = 3. Di x = 1:

                                        10
                                     a + b = 2 (Persamaan 1)
Di x = 3, kita juga menyamakan limit kiri dan limit kanan untuk memperoleh

persamaan kedua. Dengan dua titik sambung, kita butuh dua persamaan untuk

menyelesaikan dua variabel a dan b — inilah sebabnya soal dua parameter muncul.
Jenis Ketidakkontinuan yang Perlu Diketahui

Ketika syarat ketiga gagal (limit ada tetapi tidak sama dengan nilai fungsi), kita
menyebutnya Diskontinuitas yang Dapat Dihapus (Removable Discontinuity). Ciri
khasnya: nilai limit ada, tetapi tidak sama dengan nilai fungsi. Fungsi seperti ini bisa
"diperbaiki" menjadi kontinu cukup dengan mendefinisikan ulang nilai fungsi di titik
tersebut agar sama dengan limitnya.
Itulah gambaran lengkap kekontinuan pada interval terbuka dan tertutup. Kuasai tiga
syarat di titik, lalu perluas ke ujung interval dengan konsep kontinu satu arah — dan
kamu siap menaklukkan soal fungsi sepotong-sepotong!

                                                                                11
Kekontinuan Fungsi Komposisi

Teorema Limit Komposisi
Bayangkan kita punya dua fungsi, f dan g, lalu kita gabungkan menjadi (f ∘ g)(x) =
f (g(x)). Pertanyaan pentingnya: bagaimana perilaku limit fungsi komposisi ini? Di

sinilah Teorema Limit Komposisi berperan.

Teorema ini menyatakan bahwa jika limx→c g(x) = L dan fungsi luar f kontinu di titik
L, maka:

lim f (g(x)) = f (lim g(x)) = f (L)
x→c  x→c

Inti idenya: kita boleh "memindahkan" limit ke dalam fungsi luar hanya jika fungsi luar

kontinu di nilai limit tersebut. Syarat f kontinu di L ini mutlak — tanpa itu, kesimpulan

teorema bisa gagal total.

Contoh penerapan: Misalkan g(x) = x2 + 1 sehingga limx→3 g(x) = 10, dan f (u) =
  u yang kontinu di u = 10. Maka:

lim x2 + 1 = lim(x2 + 1) = 10
x→3  x→3

Teorema Kekontinuan Komposisi

Sekarang kita beralih dari limit ke kekontinuan. Teorema ini menjawab: kapan fungsi

komposisi (f ∘ g) kontinu?

Teorema: Jika g kontinu di titik c, dan f kontinu di g(c), maka fungsi komposisi (f ∘ g)
kontinu di c.

Dengan kata lain, komposisi dua fungsi kontinu tetap kontinu, selama syarat
bersarangnya terpenuhi. Secara formal:

     lim f (g(x)) = f (g(c))

     x→c

     12
Mengapa Dua Syarat Itu Penting?

Syarat          Peran                       Jika Dilanggar

g kontinu di c  Menjamin limx→c g(x) =      Nilai g(x) tidak mendekati g(c), komposisi
                g(c)
                                            bisa terputus
f kontinu di    Menjamin limit bisa
g(c)                                        f bisa meloncat/lubang tepat di titik
                "masuk" ke f
                                            tujuan

Perhatikan: kekontinuan f diperlukan di g(c), bukan di c. Ini sering menjadi jebakan —
titik yang tepat adalah hasil pemetaan g(c).

Menghubungkan Kedua Teorema

Kedua teorema sebenarnya satu keluarga. Teorema limit komposisi memberi izin

memindahkan limit ke dalam f ketika f kontinu di nilai limit L. Teorema kekontinuan
komposisi adalah versi "lebih kuat": ketika L = g(c) dan g sendiri kontinu, hasilnya
bukan sekadar limit, melainkan kekontinuan penuh di c.

Alur logika ringkas:

  • g kontinu di c ⇒ limx→c g(x) = g(c).
  • f kontinu di g(c) ⇒ limit boleh masuk ke f .

  • Gabungan keduanya ⇒ limx→c f (g(x)) = f (g(c)), yaitu (f ∘ g) kontinu di c.

Kesalahan Umum yang Perlu Diwaspadai
  • Menganggap semua komposisi otomatis kontinu. Jika g tidak kontinu di c,

    komposisi bisa tetap kontinu — tetapi teorema ini tidak menjaminnya; perlu analisis
    terpisah.

  • Mengecek kekontinuan f di titik yang salah. Selalu evaluasi f di g(c), bukan di c.

  • Mengabaikan domain. Pastikan g(c) berada dalam domain f agar f (g(c))

    terdefinisi.

Dengan memahami kedua teorema ini, kamu punya alat ampuh: untuk fungsi
komposisi yang tersusun dari fungsi-fungsi kontinu (polinomial, akar di domainnya,
dan sebagainya), kekontinuannya bisa dipastikan tanpa harus menghitung limit dari
nol setiap kali. Selamat belajar — kamu sudah selangkah lebih dekat menguasai
analisis kekontinuan!

                                        13
Teorema Nilai Antara (Intermediate Value Theorem)

Teorema Nilai Antara (IVT)
Pernyataan formal: Jika f kontinu pada selang tertutup [a, b] dan f (a) ⋅ f (b) < 0,
maka terdapat c ∈ (a, b) sehingga f (c) = 0.
Syarat mutlak: Kekontinuan pada seluruh [a, b], termasuk di titik ujung (kontinu kanan
di a, kontinu kiri di b).

Dampak diskontinuitas: Satu titik diskontinuitas saja merusak kesimpulan teorema —

grafik bisa "melompat" tanpa memotong sumbu-x.

Korolari Lokasi Akar (Bolzano)

Aspek         Penjelasan

Syarat tanda  f (a) dan f (b) berlawanan tanda

Jaminan       Ada solusi riil c ∈ (a, b) dengan f (c) = 0

Catatan penting: Diskontinuitas tak terhingga (asimtot tegak di x = c) juga

menggugurkan jaminan akar. Jadi, periksa kekontinuan lebih dulu sebelum
menyimpulkan!

              14
Pembahasan Soal dan Tabel Ringkasan Diagnostik

Menerapkan Konsep Kekontinuan: Soal dan Tabel Diagnostik

Halo! Mari kita tutup pembahasan kekontinuan dengan berlatih soal dan menyusun
tabel diagnostik yang bisa kamu pakai saat ujian.

Pola Soal Fungsi Sepotong-sepotong

Saat menguji kekontinuan fungsi sepotong-sepotong di titik sambung, selalu ikuti tiga

langkah: hitung f (c), hitung limit kiri dan kanan, lalu bandingkan. Contoh: f (x)  =  x2 −4
                                                                                       x−2

untuk x = 2 dan f (2) = 5. Limitnya limx→2(x + 2) = 4, tetapi f (2) = 5. Karena limit

ada namun tidak sama dengan nilai fungsi, ini diskontinuitas yang dapat dihapus

(removable) — perbaiki dengan redefinisi f (2) = 4.

Menentukan Parameter Konstanta

Satu parameter: Untuk g(x) = ax2 − 3 (x < 2) dan 2x + a (x ≥ 2), samakan limit kiri

4a −  3 dengan limit kanan 4 +  a,  sehingga 3a  =  7  ⇒  a  =  7  .
                                                                3

Dua parameter: Untuk fungsi dengan titik sambung x = 1 dan x = 3, hasilkan dua
persamaan dari tiap titik: a + b = 2 dan 3a + b = 26. Eliminasi menghasilkan 2a =
24 ⇒ a = 12, lalu b = −10.

Teorema Nilai Antara (IVT)
Untuk membuktikan x3 + 2x − 5 = 0 punya akar di [1, 2]: fungsi polinomial kontinu
pada [1, 2], lalu f (1) = −2 < 0 dan f (2) = 7 > 0. Karena tanda berlawanan, ada c ∈
(1, 2) dengan f (c) = 0 (Teorema Lokasi Akar/Bolzano).

Tabel Ringkasan Diagnostik

Kasus      Evaluasi                              Status               Tindakan

Kontinu    limx→c f (x) = f (c)                  Kontinu              Grafik mulus
Penuh

Removable  Limit ada, f (c) = L atau tak        Diskontinu           Redefinisi f (c) = L

           terdefinisi

                                           15
Jump          L1 = L2, keduanya                Diskontinu      Tak bisa diperbaiki
                                                Loncat          satu titik
              berhingga
                                                Diskontinu Tak  Asimtot tegak x = c
Infinite      lim = ±∞                          Hingga
                                                                Ujung kanan [a, b]
Kontinu Kiri  limx→c− f (x) = f (c)             Kontinu Kiri
              limx→c+ f (x) = f (c)
Kontinu       f kontinu, f (a) ⋅ f (b) < 0      Kontinu Kanan   Ujung kiri [a, b]
Kanan
                                                Ada akar        f (c) = 0
IVT

Semangat berlatih — kuasai tabel ini dan soal sepotong-sepotong jadi mudah!

                                            16
