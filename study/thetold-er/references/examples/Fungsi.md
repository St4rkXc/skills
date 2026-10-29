---
mode: detailed
pages: 37
words: 7904
---

pelajarin.ai

Konsep Dasar Fungsi

Halo! Selamat datang di bab pertama tentang fungsi. Topik ini mungkin terlihat
sederhana, tetapi sebenarnya menjadi fondasi penting untuk hampir semua materi
matematika yang akan kamu pelajari selanjutnya, terutama di dunia sistem informasi.
Yuk, kita pelajari bersama dengan santai tapi menyeluruh!

Apa Itu Fungsi?

Bayangkan fungsi seperti sebuah "mesin ajaib". Kamu memasukkan sebuah angka ke
dalamnya, dan mesin itu akan memprosesnya lalu mengeluarkan tepat satu angka
hasil. Konsep inilah yang mendasari definisi fungsi secara formal.

Sebuah fungsi dari (bilangan real) ke adalah suatu aturan yang mengaitkan atau

memadankan setiap x ∈ dengan tepat satu y ∈ .

Kata kunci di sini adalah "tepat satu". Ini berarti satu input hanya boleh menghasilkan
satu output. Jika satu input bisa menghasilkan dua atau lebih output, maka aturan
tersebut bukanlah fungsi. Inilah syarat mutlak yang harus dipenuhi.

Notasi Fungsi

Secara matematis, fungsi dituliskan dengan notasi berikut:

              f : x → y = f (x)

Mari kita bedah notasi ini satu per satu agar lebih mudah dipahami:

  • f adalah nama fungsi (kamu bisa memberi nama apa pun, misalnya g atau h).
  • x → y menunjukkan bahwa x dipetakan ke y.
  • f (x) adalah nilai fungsi ketika dimasukkan input x. Notasi ini bisa dibaca "f dari x".

Peubah Bebas dan Peubah Tak Bebas

Dalam sebuah fungsi, terdapat dua jenis peubah yang bekerja sama:

Jenis Peubah  Simbol Peran

                            1
Peubah bebas  x               Nilai yang kita masukkan (input); kita bebas memilih
                              nilainya
Peubah tak
                              Nilai hasil yang keluar (output); nilainya bergantung pada
                           y
                              x
bebas

Disebut "bebas" karena kita bisa memilih nilai x sesuka hati. Disebut "tak bebas" karena
nilai y sepenuhnya bergantung pada pilihan x tadi. Jadi, jika kita mengubah x, maka
nilai y juga ikut berubah.

Contoh-Contoh Fungsi Sederhana

Mari kita lihat beberapa contoh fungsi beserta karakteristiknya masing-masing.

Contoh 1: Fungsi Polinomial

                              f (x) = x2 + 2x + 4

Ini adalah fungsi kuadrat. Untuk setiap nilai x yang kita masukkan, kita menghitung
nilai y-nya. Misalnya, jika x = 1, maka:

                              f (1) = 12 + 2(1) + 4 = 1 + 2 + 4 = 7

Fungsi ini terdefinisi untuk semua bilangan real, sehingga domainnya adalah seluruh
himpunan .
Contoh 2: Fungsi Akar

                                             f (x) = x + 1

Fungsi ini sedikit lebih rumit karena melibatkan akar kuadrat. Di bilangan real, kita tidak
bisa mengambil akar kuadrat dari bilangan negatif. Jadi, isi di dalam akar harus
memenuhi:

                              2
                                       x + 1 ≥ 0 ⟹ x ≥ −1

Dengan demikian, domain fungsi ini adalah Df = {x ∣ x ≥ −1}. Inilah contoh

bagaimana bentuk fungsi membatasi daerah asalnya.
Contoh 3: Fungsi dengan Batasan Domain

                                      f (x) = x2, −2 ≤ x ≤ 3

Ini adalah fungsi kuadrat yang sama seperti sebelumnya, tetapi kali ini domainnya

sengaja dibatasi hanya pada interval −2 ≤ x ≤ 3. Kenapa dibatasi? Karena kadang

dalam suatu permasalahan nyata, kita hanya peduli pada rentang nilai tertentu saja.
Batasan ini akan berpengaruh besar pada range fungsinya.

Domain (Daerah Asal)
Domain atau daerah asal dari fungsi f (x), dinotasikan Df , adalah himpunan semua
nilai x yang membuat fungsi tersebut terdefinisi. Secara formal:

                                  Df = {x ∈ ∣ f (x) terdefinisi}

Beberapa hal penting yang perlu kamu perhatikan ketika menentukan domain:

  • Fungsi polinomial (seperti x2 + 2x + 4) memiliki domain semua bilangan real.

  • Fungsi akar harus memastikan isi di dalam akar tidak negatif (untuk akar berindeks
    genap).

  • Fungsi pecahan harus memastikan penyebutnya tidak bernilai nol.

  • Batasan eksplisit seperti −2 ≤ x ≤ 3 juga mempersempit domain.
Range (Daerah Nilai)
Range atau daerah nilai dari fungsi f (x), dinotasikan Rf , adalah himpunan semua
nilai y yang mungkin dihasilkan oleh fungsi ketika x berada di domainnya. Secara

formal:

                                                                                3
                        Rf = {f (x) ∣ x ∈ Df }

Perhatikan bahwa range sangat bergantung pada domain. Mari bandingkan dua
kasus:

  • Untuk f (x) = x2 dengan domain seluruh , range-nya adalah Rf = {y ∣ y ≥ 0}.
  • Untuk f (x) = x2 dengan domain −2 ≤ x ≤ 3, range-nya menjadi {y ∣ 0 ≤ y ≤ 9},

    karena nilai x dibatasi.

Ini menunjukkan bahwa domain menentukan range. Jika kamu mengubah domain,
kamu juga mengubah range-nya.

Merangkum Hubungan Domain dan Range

Agar lebih jelas, mari kita ringkas hubungan antara input dan output dalam sebuah
tabel:

Fungsi                  Domain (Df )     Cara Menentukan Range

f (x) = x2 + 2x + 4     Semua            Substitusi seluruh x, cari nilai minimum

f (x) = x + 1           x ≥ −1           Akar selalu ≥ 0, jadi y ≥ 0

f (x) = x2, −2 ≤ x ≤ 3  −2 ≤ x ≤ 3       Hitung x2 pada batas interval

Kesimpulan
Fungsi adalah aturan yang memadankan setiap input x (peubah bebas) dengan
tepat satu output y (peubah tak bebas). Pemahaman tentang domain dan range

sangatlah krusial, karena keduanya menentukan di mana fungsi "hidup" dan nilai apa
yang bisa dihasilkannya. Kunci sukses mempelajari fungsi adalah berlatih menentukan
domain dan range dari berbagai bentuk fungsi, terutama yang melibatkan akar,
pecahan, atau batasan eksplisit.

Semangat belajar, ya! Konsep dasar ini akan sangat membantumu di bab-bab
selanjutnya, seperti komposisi fungsi dan fungsi invers.

                                      4
Menentukan Domain dan Range Fungsi

Halo! Selamat datang di bab yang akan membahas salah satu fondasi terpenting
dalam mempelajari fungsi, yaitu domain (daerah asal) dan range (daerah nilai atau
daerah hasil). Memahami kedua konsep ini ibarat memahami "batas wilayah" dari
sebuah fungsi — tanpa itu, kita bisa salah menafsirkan nilai mana saja yang
sebenarnya boleh masuk dan nilai apa saja yang bisa keluar dari fungsi tersebut.
Tenang saja, kita akan bahas langkah demi langkah dengan contoh perhitungan yang
konkret. Yuk, kita mulai!

Apa Itu Domain dan Range?
Sebelum masuk ke perhitungan, mari kita samakan dulu pemahamannya.

  • Domain (daerah asal), ditulis Df , adalah himpunan semua nilai x yang boleh

    dimasukkan ke dalam fungsi sehingga fungsi tersebut terdefinisi (menghasilkan
    nilai yang nyata).

  • Range (daerah nilai), ditulis Rf , adalah himpunan semua nilai y = f (x) yang
    benar-benar bisa dihasilkan ketika x menjelajahi seluruh domainnya.

Jadi, domain berbicara tentang "input yang sah", sedangkan range berbicara tentang
"output yang mungkin". Keduanya biasanya dituliskan dalam notasi interval.

Menuliskan Jawaban dengan Notasi Interval
Sebelum terlalu jauh, penting untuk menyegarkan cara menulis interval, karena seluruh
jawaban kita akan memakai format ini.

Notasi Interval  Arti

[a, b]           Semua bilangan dari a sampai b, termasuk a dan b

(a, b)           Semua bilangan antara a dan b, tidak termasuk a dan b

[a, ∞)           Semua bilangan ≥ a

(−∞, b]          Semua bilangan ≤ b

(−∞, ∞)          Seluruh bilangan real

                       5
Perhatikan bahwa kurung siku [ ] berarti titik ujungnya ikut, sedangkan kurung biasa ( )
berarti titik ujungnya tidak ikut. Simbol ∞ dan −∞ selalu memakai kurung biasa

karena bukan bilangan yang bisa dicapai.

Domain Fungsi Polinom: Seluruh Bilangan Real
Sekarang kita masuk ke pola pertama. Fungsi polinom adalah fungsi yang berbentuk

suku-suku dengan pangkat bulat tak negatif, misalnya f (x) = x2 + 2x + 4.

Pertanyaan kuncinya: apakah ada nilai x yang membuat fungsi ini "rusak"? Untuk

polinom, jawabannya tidak ada. Operasi yang ada hanyalah penjumlahan,
pengurangan, dan perkalian — semuanya aman untuk setiap bilangan real. Tidak ada
pembagian dengan nol, tidak ada akar dari bilangan negatif.

                                                                                        x

Oleh karena itu, domainnya adalah:

Df = {x ∣ x ∈ } = (−∞, ∞)

Inilah mengapa pada contoh pertama, langkah pertama yang dilakukan adalah

langsung menyimpulkan Df = (−∞, ∞) — karena fungsinya polinom, tidak ada

syarat khusus yang perlu diperiksa.

Menentukan Range Fungsi Kuadrat dengan Melengkapkan Kuadrat Sempurna
Domain polinom memang mudah, tetapi range-nya tidak selalu seluruh bilangan real.
Ambil contoh fungsi kuadrat:

f (x) = x2 + 2x + 4

Fungsi kuadrat x2 selalu bernilai ≥ 0, jadi hasilnya tidak mungkin mencapai semua

bilangan real. Bagaimana cara mengetahui range-nya secara tepat? Di sinilah teknik

melengkapkan kuadrat sempurna (                    ) berperan.

Langkah 1 — Kelompokkan dan siapkan bentuk kuadrat. Kita punya x2 + 2x + 4. Ambil
koefisien x, yaitu 2, lalu bagi dua sehingga menjadi 1. Kuadratkan hasilnya: 12 = 1.

Langkah 2 — Tambahkan dan kurangi nilai tersebut.

                                    6
                                     f (x) = x2 + 2x + 1 + 4 − 1

Langkah 3 — Bentuk kuadrat sempurna dan sederhanakan. Tiga suku pertama

membentuk (x + 1)2, sehingga:

                                          f (x) = (x + 1)2 + 3

Sekarang bentuknya jauh lebih mudah dibaca! Perhatikan bahwa (x + 1)2 selalu ≥ 0
untuk setiap nilai x. Nilai terkecilnya adalah 0, yang terjadi saat x = −1. Maka nilai
terkecil dari f (x) adalah:

                                         f (x)min = 0 + 3 = 3

Karena bentuk kuadratnya tidak pernah negatif, f (x) tidak akan pernah kurang dari 3.
Sebaliknya, ketika x menjauh ke arah positif atau negatif, (x + 1)2 tumbuh tanpa
batas, sehingga f (x) bisa mencapai nilai berapa pun yang lebih besar atau sama
dengan 3.

                   Rf = [3, ∞)
Perhatikan penulisan kurung siku di angka 3 — ini menandakan bahwa nilai 3 benar-
benar tercapai (saat x = −1), jadi ia termasuk dalam range. Ini poin penting yang

sering terlewat!

Domain Fungsi Akar: Syarat di Bawah Akar ≥ 0

Beralih ke pola kedua, yaitu fungsi akar. Contohnya:

                                             f (x) = x + 1

Fungsi akar memiliki aturan mutlak yang harus selalu diingat: bilangan di bawah
tanda akar (radikan) tidak boleh negatif, karena akar kuadrat dari bilangan negatif
bukan bilangan real. Jadi syaratnya:

                                                                                7
                            radikan ≥ 0

Untuk fungsi kita, radikannya adalah x + 1, sehingga:

                     x+1≥0 ⟹ x≥0

Maka domainnya:

                     Df = {x ∣ x ≥ 0} = [0, ∞)

Inilah langkah pertama yang dilakukan pada contoh kedua — yaitu menetapkan

bahwa x harus ≥ 0 agar fungsi terdefinisi.

Menentukan Range Fungsi Akar

Setelah domain diketahui, kita cari range-nya. Kita tahu bahwa untuk x ≥ 0, berlaku
juga x ≥ 0. Nilai terkecil dari x adalah 0, yang terjadi saat x = 0. Maka:

                     f (x) = x + 1 ≥ 0 + 1 = 1

Nilai terkecil fungsi adalah 1. Seiring x bertambah besar, nilai akarnya juga bertambah
besar tanpa batas, sehingga f (x) bisa mencapai nilai berapa pun yang ≥ 1.

        Rf = [1, ∞)

Sekali lagi, tanda kurung siku pada angka 1 menunjukkan bahwa nilai tersebut
tercapai (saat x = 0), jadi termasuk dalam range.

Rangkuman Kedua Contoh
Mari kita rangkum semuanya dalam satu tabel agar mudah diingat.

Fungsi               Jenis                             Df  Rf

                            8
f (x) = x2 + 2x + 4  Polinom (kuadrat)  (−∞, ∞)  [3, ∞)
f (x) = x + 1        Akar               [0, ∞)   [1, ∞)

Poin Kunci yang Perlu Diingat

  • Fungsi polinom selalu memiliki domain (−∞, ∞) karena terdefinisi untuk setiap

    bilangan real.

  • Range fungsi kuadrat ditemukan dengan melengkapkan kuadrat sempurna,

    mengubah bentuk menjadi (x + p)2 + q. Nilai q menjadi batas bawah range, yaitu
    [q, ∞).

  • Fungsi akar mensyaratkan radikan ≥ 0 untuk menentukan domainnya.

  • Range fungsi akar diperoleh dengan mencari nilai terkecil output saat radikan

    minimum (biasanya 0), lalu menambahkan konstanta di luarnya.

  • Selalu perhatikan kurung siku vs kurung biasa saat menuliskan interval, karena titik

    ujung yang tercapai harus ditulis dengan [ ].

Dengan memahami dua pola ini — polinom dan akar — kamu sudah punya bekal kuat
untuk menentukan domain dan range dari banyak fungsi lain. Latihan rutin dengan
variasi koefisien akan membuat teknik melengkapkan kuadrat dan analisis syarat akar
menjadi refleks bagimu. Semangat berlatih, ya!

                     9
Jenis-Jenis Fungsi: Polinom dan Rasional

Selamat datang di pembahasan salah satu topik paling fundamental dalam kalkulus:
jenis-jenis fungsi! Di bab ini kita akan fokus pada dua keluarga fungsi yang paling
sering muncul, yaitu fungsi polinom (suku banyak) dan fungsi rasional. Memahami
keduanya penting banget, karena hampir semua fungsi yang kamu temui nanti bisa
dipandang sebagai gabungan atau perbandingan dari keduanya. Yuk, kita bedah satu
per satu dengan santai tapi tetap teliti!

Fungsi Polinom (Suku Banyak)

Mari kita mulai dari yang paling ramah: fungsi polinom. Fungsi ini disebut juga suku
banyak, dan bentuk umumnya adalah:

                               f (x) = a0 + a1x + a2x2 + ⋯ + anxn

Beberapa hal yang perlu kamu perhatikan dari bentuk di atas:

  • Simbol a0, a1, a2, … , an adalah koefisien, yaitu bilangan-bilangan konstan yang

    nilainya sudah tertentu.

  • Pangkat tertinggi dari variabel x disebut derajat dari polinom tersebut, yaitu n.
  • Masing-masing bagian seperti a1x atau a2x2 disebut suku. Jadi polinom pada

    dasarnya adalah jumlah dari beberapa suku.
Sifat paling penting: fungsi polinom terdefinisi di seluruh bilangan real. Artinya, untuk

setiap nilai x yang kamu pilih — entah itu bilangan negatif, nol, pecahan, atau bilangan
besar sekali — kamu selalu bisa menghitung nilai f (x)-nya. Tidak ada nilai x yang

membuat polinom "rusak" atau tidak bisa dihitung.
Contoh sederhana:

  • f (x) = 3 (polinom derajat 0, biasa disebut fungsi konstan)
  • f (x) = 2x + 5 (polinom derajat 1, fungsi linear)
  • f (x) = x2 − 4x + 1 (polinom derajat 2, fungsi kuadrat)
Semuanya bisa dihitung untuk x berapa pun. Domainnya selalu seluruh bilangan real.

                                                                               10
Fungsi Rasional

Sekarang kita naik level ke fungsi rasional. Sesuai namanya (rasional = perbandingan),
fungsi ini berbentuk pembagian dua fungsi polinom:

                                                         p(x)
                                              f (x) = q(x)

dengan p(x) dan q(x) merupakan fungsi polinom, dan syarat krusialnya adalah:

                                                 q(x) = 0

Kenapa syarat ini begitu penting? Karena dalam matematika, pembagian dengan nol
tidak terdefinisi. Jadi, fungsi rasional sebenarnya terdefinisi di mana-mana, kecuali di

nilai-nilai x yang membuat penyebutnya sama dengan nol.

Menentukan Domain Fungsi Rasional
Langkah untuk menentukan domain (daerah asal) fungsi rasional sangatlah
sistematis:

  1. Ambil penyebutnya, yaitu q(x).
 2. Cari pembuat nol dari penyebut tersebut, yaitu selesaikan persamaan q(x) = 0.

 3. Keluarkan nilai-nilai itu dari himpunan seluruh bilangan real. Sisa nilainya adalah
    domain fungsi.

Dengan kata lain, nilai x yang membuat q(x) = 0 adalah "titik terlarang" yang harus

kita hindari.

Contoh Lengkap: Membedah Sebuah Fungsi Rasional

Mari kita kerjakan contoh yang sangat klasik:

                                                       x2 + 1
                                             f (x) = x2 − 4

                                                                                11
Perhatikan bahwa pembilangnya adalah p(x) = x2 + 1 dan penyebutnya adalah
q(x) = x2 − 4. Keduanya jelas merupakan polinom, jadi ini memang fungsi rasional.

Langkah 1: Cari pembuat nol penyebut.
Kita set penyebut sama dengan nol:

                                               x2 − 4 = 0

Langkah 2: Faktorkan dan selesaikan.

Bentuk x2 − 4 adalah selisih dua kuadrat, sehingga bisa difaktorkan menjadi:

                                          (x − 2)(x + 2) = 0

Dari sini diperoleh dua solusi:

                                        x = 2 atau x = −2

Langkah 3: Tentukan domain.

Karena fungsi ini menjadi tidak terdefinisi (penyebutnya nol) tepat di x = 2 dan x =
−2, maka kedua nilai itu harus dikeluarkan. Dengan demikian:

                                Df = {x ∣ x ∈ , x = −2, x = 2}

atau bisa ditulis lebih singkat sebagai ∖ {−2, 2}.
Insight penting: Perhatikan bahwa pembilang x2 + 1 tidak pernah nol untuk bilangan
real apa pun (karena x2 selalu tak negatif, ditambah 1 pasti positif). Jadi seluruh

"masalah" pada fungsi ini murni berasal dari penyebutnya. Inilah kunci utama dalam
menganalisis fungsi rasional: selalu curigai penyebutnya lebih dulu!

Rangkuman Perbandingan

Agar lebih mudah mengingat perbedaan keduanya, perhatikan tabel berikut:

                                                                               12
Aspek          Fungsi Polinom              Fungsi Rasional

Bentuk         f (x) = a0 + a1x + ⋯ +                p(x)
umum           anxn                        f (x) = q(x)

Komponen       Jumlah suku berpangkat      Perbandingan dua polinom
                                           Seluruh real kecuali pembuat nol
Domain         Seluruh bilangan real       penyebut

Syarat         Tidak ada                   q(x) = 0
khusus                                               x2 + 1
               f (x) = x2 − 4x + 1
Contoh                                     f (x) = x2 − 4

Poin-Poin Kunci untuk Diingat
  • Fungsi polinom selalu "aman" — bisa dihitung untuk semua nilai x tanpa

    pengecualian. Domain-nya adalah seluruh bilangan real.

• Fungsi rasional adalah pembagian dua polinom, dan "titik lemahnya" selalu ada di
  penyebut.

• Kunci menentukan domain fungsi rasional: cari pembuat nol penyebut, lalu
  keluarkan nilai-nilai tersebut.

• Pada contoh f (x)  =  x2  +1                                                     =
                        x2  − 4 , domain-nya adalah semua bilangan real kecuali x

2 dan x = −2.

Dengan memahami dua jenis fungsi ini, kamu sudah punya fondasi kuat untuk
menjelajahi topik-topik kalkulus berikutnya. Jangan ragu untuk berlatih dengan
berbagai bentuk penyebut — semakin sering kamu memfaktorkan dan mencari
pembuat nol, semakin cepat dan percaya diri kamu dalam menentukan domain.
Semangat belajar, ya!

                                       13
Jenis-Jenis Fungsi: Genap, Ganjil, dan Periodik

Memahami Fungsi Genap dan Fungsi Ganjil

Halo! Selamat datang di bab yang sangat menarik ini. Kita akan belajar tentang tiga
"kepribadian" khusus sebuah fungsi: fungsi ganjil, fungsi genap, dan fungsi periodik.
Mungkin terdengar seperti istilah yang rumit, tetapi sebenarnya konsepnya sangat
intuitif. Kuncinya ada pada satu pertanyaan sederhana:

Mari kita bedah satu per satu dengan santai namun teliti.

Fungsi Ganjil
Sebuah fungsi f disebut fungsi ganjil jika memenuhi persamaan berikut untuk setiap x

di daerah asalnya:

                                            f (−x) = −f (x)

Apa artinya? Artinya, jika kita memasukkan nilai negatif dari sebuah bilangan, hasilnya
sama persis dengan nilai negatif dari hasil bilangan positif itu. Dengan kata lain, tanda
negatif pada input "keluar" menjadi tanda negatif pada output.
Sifat simetri grafiknya sangat penting untuk diingat: grafik fungsi ganjil simetri

terhadap titik asal (titik (0, 0)). Bayangkan grafik yang diputar 180∘ mengelilingi titik
asal — bentuknya akan tetap sama persis. Inilah yang disebut simetri rotasi 180∘.

Contoh: f (x) = x3

Mari kita buktikan bahwa f (x) = x3 adalah fungsi ganjil.
Kita hitung f (−x):

                            f (−x) = (−x)3 = −x3 = −(x3) = −f (x)

Karena f (−x) = −f (x), terbukti bahwa f (x) = x3 merupakan fungsi ganjil. Jika kamu

menggambar grafiknya, kamu akan melihat kurva yang naik dari kiri bawah melewati

titik asal lalu menuju kanan atas — persis simetris terhadap titik (0, 0).

                                                                               14
Fungsi Genap
Sebuah fungsi f disebut fungsi genap jika memenuhi persamaan:

                           f (−x) = f (x)

Bedanya dengan fungsi ganjil sangat jelas: di sini, memasukkan bilangan negatif tidak

mengubah hasilnya sama sekali. f (−2) akan bernilai sama dengan f (2), dan

seterusnya.

Sifat simetri grafiknya: grafik fungsi genap simetri terhadap sumbu y. Jika kamu

melipat grafik di sepanjang sumbu vertikal (sumbu y), sisi kiri akan menutup sisi kanan
dengan sempurna. Ini disebut juga simetri cermin terhadap sumbu y.

Contoh: f (x) = x2

Mari kita verifikasi bahwa f (x) = x2 adalah fungsi genap.

Kita hitung f (−x):

                         f (−x) = (−x)2 = x2 = f (x)

Karena f (−x) = f (x), terbukti f (x) = x2 adalah fungsi genap. Perhatikan bahwa

mengkuadratkan bilangan negatif menghasilkan bilangan positif — inilah sebabnya
hasilnya sama. Bentuk grafiknya adalah parabola yang membuka ke atas, dengan
puncaknya di titik asal dan sisi kiri-kanan yang identik.

Ringkasan Perbandingan

Agar lebih mudah diingat, mari kita bandingkan keduanya dalam tabel berikut.

Aspek     Fungsi Ganjil                    Fungsi Genap

Definisi  f (−x) = −f (x)                  f (−x) = f (x)

Simetri   Terhadap titik asal (0, 0)       Terhadap sumbu y
grafik

                                           Tanda input negatif "hilang"

                                      15
Perilaku   Tanda input negatif "pindah" ke      f (x) = x2
tanda      output
Contoh
           f (x) = x3
Uji cepat
           Substitusi −x hasilnya negatif dari  Substitusi −x hasilnya sama

           aslinya                              dengan aslinya

Satu catatan penting: tidak semua fungsi harus ganjil atau genap. Banyak fungsi

biasa seperti f (x) = x2 + x bukan keduanya, karena tidak memenuhi salah satu

definisi di atas. Jadi, ketika kita menguji, kita perlu benar-benar memeriksa apakah
hasilnya cocok dengan definisi — jangan berasumsi.

Fungsi Periodik
Sekarang kita masuk ke konsep ketiga. Sebuah fungsi f disebut fungsi periodik jika
terdapat suatu bilangan positif p sehingga:

           f (x + p) = f (x)

untuk setiap x di daerah asalnya. Bilangan p ini disebut perioda fungsi. Artinya, nilai
fungsi akan berulang secara teratur setiap kali x bertambah sebesar p. Pola grafiknya

akan terlihat seperti gelombang yang tak berujung, mengulang bentuk yang sama
berulang-ulang.

Contoh: f (x) = sin x

Contoh klasik dan paling penting adalah fungsi sinus. Fungsi f (x) = sin x memiliki
perioda 2π, sehingga:

                                          sin(x + 2π) = sin x

Artinya, jika kita menggeser sudut sebesar satu putaran penuh (2π radian atau 360∘),

nilai sinusnya kembali sama. Grafiknya berupa gelombang mulus yang naik dan turun
secara berulang tanpa henti.

           16
Membaca Ketiga Konsep Ini Bersama

Tiga jenis fungsi ini sering muncul bersamaan dalam soal dan aplikasi:
  • Fungsi ganjil dan genap membantu kita mengenali simetri — mempermudah
    menggambar grafik dan menyederhanakan perhitungan integral.
  • Fungsi periodik muncul secara alami di dunia nyata, seperti pada gelombang
    suara, arus listrik bolak-balik, dan gerak bandul.
  • Mengetahui jenis sebuah fungsi bisa menjadi "jalan pintas" untuk memprediksi
    bentuk grafiknya tanpa harus menghitung banyak titik.

Poin-Poin Kunci yang Wajib Diingat
  • Fungsi ganjil: f (−x) = −f (x), grafiknya simetri terhadap titik asal, contohnya
    f (x) = x3.
  • Fungsi genap: f (−x) = f (x), grafiknya simetri terhadap sumbu y, contohnya
    f (x) = x2.
  • Fungsi periodik: f (x + p) = f (x) dengan perioda p, contohnya f (x) = sin x
    dengan perioda 2π.
  • Selalu uji dengan substitusi — masukkan −x ke dalam rumus dan bandingkan
    hasilnya dengan f (x) asli.

  • Tidak semua fungsi termasuk ganjil atau genap; sebagian di antaranya adalah
    "biasa saja".

  • Simetri adalah kata kuncinya: ganjil berarti simetri titik asal, genap berarti simetri

    sumbu y.

Dengan memahami ketiga konsep ini, kamu sudah memiliki alat penting untuk
menganalisis perilaku fungsi, terutama saat berhadapan dengan trigonometri dan
kalkulus. Latihan terbaik adalah dengan mencoba menguji beberapa fungsi sendiri —
semangat belajar, kamu pasti bisa!

                                                                               17
Grafik Fungsi: Fungsi Linear

Grafik Fungsi Linear: Menggambar Garis Lurus dengan Tepat

Halo! Selamat datang di bab tentang grafik fungsi, khususnya fungsi linear. Kalau
kamu pernah melihat garis lurus yang digambar pada bidang koordinat, itulah yang
akan kita pelajari di sini. Kabar baiknya: menggambar grafik fungsi linear itu salah satu
keterampilan paling mudah dan paling memuaskan dalam matematika. Dengan
hanya dua titik, kamu sudah bisa menggambar seluruh garisnya. Mari kita bahas
langkah demi langkah dengan santai tapi teliti.

Apa Itu Grafik Fungsi?

Sebelum melangkah ke fungsi linear, kita perlu memahami dulu apa yang dimaksud

dengan grafik fungsi. Misalkan diberikan suatu fungsi y = f (x). Himpunan titik-titik

berbentuk:

                                      {(x, y) ∣ x ∈ Df , y ∈ Rf }

disebut grafik fungsi f .

Mari kita bedah notasi ini agar tidak terasa menakutkan:

  • x ∈ Df berarti x adalah anggota domain (daerah asal) fungsi, yaitu semua nilai

    input yang boleh dimasukkan.

  • y ∈ Rf berarti y adalah anggota range (daerah hasil) fungsi, yaitu semua nilai

    output yang dihasilkan.

  • Pasangan (x, y) menunjukkan bahwa untuk setiap nilai x yang kita pilih, kita
    memperoleh tepat satu nilai y = f (x).

Jadi, grafik fungsi pada dasarnya adalah kumpulan pasangan input-output yang
digambar sebagai titik pada bidang koordinat Cartesius. Setiap titik pada grafik

adalah "bukti" bahwa ketika kita memasukkan nilai x tertentu, fungsinya menghasilkan
nilai y tertentu. Dengan kata lain, grafik adalah wajah visual dari sebuah fungsi — kita

bisa "melihat" perilaku fungsi tersebut tanpa harus menghitung satu per satu.

Mengenal Fungsi Linear

Sekarang kita masuk ke inti bab ini. Fungsi linear adalah fungsi yang bentuk umumnya:

                                                                               18
                                          f (x) = ax + b

dengan a dan b adalah konstanta bilangan real, dan a = 0.

Beberapa hal penting yang perlu kamu ingat:

  • a disebut koefisien (kemiringan/gradien). Nilai ini menentukan seberapa miring

    garisnya dan ke arah mana garis tersebut menanjak atau menurun.

  • b disebut konstanta (titik potong sumbu-y). Nilai ini menunjukkan di mana garis

    memotong sumbu-y.

  • Variabel x berpangkat satu (linear), sehingga tidak ada lengkungan, patahan, atau

    gelombang pada grafiknya.

Ciri khas paling mencolok dari fungsi linear adalah: grafiknya selalu berupa garis
lurus. Inilah sebabnya fungsi ini disebut "linear" — dari kata yang berarti garis. Tidak

peduli berapa pun nilai a dan b yang kamu pilih (asal a = 0), hasilnya tetap garis lurus.

Sifat inilah yang membuat fungsi linear sangat istimewa dan mudah digambar.

Strategi Menggambar Grafik: Dua Titik Potong

Karena grafik fungsi linear berupa garis lurus, kita hanya perlu dua titik untuk
menggambarnya. Dua titik ini cukup untuk menentukan satu garis lurus secara unik.
Cara paling praktis dan rapi adalah dengan menentukan titik potong terhadap
sumbu-x dan titik potong terhadap sumbu-y. Mari kita bahas keduanya.

1. Menentukan Titik Potong Sumbu-x

Titik potong sumbu-x adalah titik di mana grafik menyentuh atau memotong sumbu-

x. Pada sumbu-x, nilai y selalu sama dengan nol. Karena itu, untuk mencarinya kita
substitusikan y = 0 ke dalam persamaan fungsi, lalu selesaikan untuk x.

Langkah-langkahnya:

1. Tulis persamaan fungsi: y = ax + b.

2. Substitusikan y = 0, sehingga menjadi 0 = ax + b.

3.  Selesaikan:  ax  =  −b,  sehingga  x  =    b  .
                                             −a

4. Titik potong sumbu-x adalah           b
                                       −a, 0 .

                                                  19
2. Menentukan Titik Potong Sumbu-y
Titik potong sumbu-y adalah titik di mana grafik memotong sumbu-y. Pada sumbu-y,

nilai x selalu sama dengan nol. Karena itu, kita substitusikan x = 0 ke dalam

persamaan fungsi.
Langkah-langkahnya:

  1. Tulis persamaan fungsi: y = ax + b.
 2. Substitusikan x = 0, sehingga menjadi y = a(0) + b = b.
 3. Titik potong sumbu-y adalah (0, b).
Perhatikan bahwa nilai b pada bentuk umum f (x) = ax + b langsung menunjukkan

titik potong sumbu-y. Ini adalah "jalan pintas" yang sangat berguna!

Contoh Lengkap: Menggambar Grafik y = x + 1

Sekarang mari kita terapkan semua langkah di atas pada contoh konkret. Misalkan kita
ingin menggambar grafik fungsi:

                                                y = x+1

Di sini, a = 1 dan b = 1.
Langkah 1 — Menentukan titik potong sumbu-x (substitusi y = 0):

                                                0=x+1

                                                  x = −1

Jadi, titik potong sumbu-x adalah (−1, 0).
Langkah 2 — Menentukan titik potong sumbu-y (substitusi x = 0):

                                             y = 0+1 = 1

                                                                               20
Jadi, titik potong sumbu-y adalah (0, 1).

Langkah 3 — Menggambar kedua titik pada bidang koordinat, lalu
menghubungkannya dengan garis lurus.

Kedua titik ini, yaitu (−1, 0) dan (0, 1), kita gambarkan pada bidang Cartesius. Titik
(−1, 0) berada di sumbu-x sebelah kiri titik asal, sedangkan titik (0, 1) berada di

sumbu-y tepat satu satuan di atas titik asal. Setelah kedua titik ini ditandai, tarik garis

lurus yang melewati keduanya, dan perpanjang di kedua arah. Itulah grafik fungsi y =
x + 1.

Verifikasi dengan Titik Ketiga
Sebagai pengecekan, kita bisa memilih nilai x lain dan memastikan titiknya terletak
pada garis yang sama. Misalnya, ambil x = 1:

              y = 1+1 = 2

Titik (1, 2) seharusnya juga terletak pada garis tersebut. Jika kita menggambarnya, titik
ini memang berada tepat pada garis lurus yang menghubungkan (−1, 0) dan (0, 1).

Verifikasi semacam ini sangat berguna untuk memastikan tidak ada kesalahan hitung.

Rangkuman Praktis

Berikut tabel ringkasan yang bisa kamu jadikan panduan cepat:

Langkah       Yang Dilakukan                                Hasil

Titik potong  Substitusi y = 0                                b
sumbu-x                                                     − ,0

                                                              a

Titik potong  Substitusi x = 0                              (0, b)
sumbu-y

Menggambar    Hubungkan kedua titik dengan garis lurus dan  Grafik fungsi
              perpanjang                                    linear

                                21
Hal-Hal yang Perlu Diwaspadai
  • Pastikan a = 0. Jika a = 0, fungsi menjadi f (x) = b, yang grafiknya berupa garis

    horizontal (bukan fungsi linear murni dalam konteks ini).

  • Periksa tanda positif dan negatif. Misalnya, untuk y = −2x + 4, titik potong sumbu-
    x adalah (2, 0) dan sumbu-y adalah (0, 4).

  • Perpanjang garis. Garis pada grafik fungsi linear berlanjut tanpa batas ke kedua
    arah, jadi jangan hanya menggambar segmen pendek antara dua titik saja.

  • Gunakan penggaris. Karena grafiknya garis lurus, menggambar dengan penggaris
    memastikan keakuratan visual.

Penutup

Selamat! Kamu baru saja menguasai cara menggambar grafik fungsi linear. Kuncinya

sederhana: pahami definisi grafik fungsi sebagai himpunan titik (x, y), kenali bentuk
umum f (x) = ax + b, lalu tentukan dua titik potong — sumbu-x dengan y = 0 dan
sumbu-y dengan x = 0. Dari sana, cukup hubungkan kedua titik dengan garis lurus.

Dengan latihan yang cukup, langkah-langkah ini akan terasa seperti refleks. Teruslah

berlatih dengan berbagai nilai a dan b, dan kamu akan semakin percaya diri

membaca serta menggambar grafik fungsi. Sampai jumpa di bab berikutnya!

                                                                               22
Grafik Fungsi: Fungsi Kuadrat dan Fungsi Banyak Aturan

Halo! Pada bab ini kita akan belajar menggambar grafik dua jenis fungsi yang sangat
penting: fungsi kuadrat yang membentuk kurva mulus bernama parabola, dan fungsi
banyak aturan (piecewise) yang grafiknya tersusun dari beberapa potongan berbeda.
Mari kita bahas keduanya langkah demi langkah dengan santai namun tetap teliti.

Mengingat Kembali: Fungsi Linear dan Titik Potong Sumbu

Sebelum masuk ke fungsi kuadrat, ada baiknya kita mengingat cara menentukan titik
potong sumbu pada sebuah grafik, karena metode yang sama akan kita pakai
berulang kali.
Untuk menggambar grafik sebuah fungsi, kita biasanya mencari dua titik bantu
terlebih dahulu:

  • Titik potong dengan sumbu-x, yaitu titik saat nilai y = 0, sehingga kita mencari
    nilai x yang membuat fungsi bernilai nol.

  • Titik potong dengan sumbu-y, yaitu titik saat nilai x = 0, sehingga kita cukup

    menghitung nilai fungsi di titik nol.

Sebagai contoh, perhatikan fungsi y = x + 1:
  • Saat y = 0, kita peroleh x = −1, sehingga titik potong sumbu-x adalah (−1, 0).
  • Saat x = 0, kita peroleh y = 1, sehingga titik potong sumbu-y adalah (0, 1).

Dengan menghubungkan kedua titik ini, kita sudah bisa menggambar grafik garis
lurusnya. Pola berpikir "cari titik potong, lalu hubungkan" inilah yang akan kita
kembangkan untuk fungsi kuadrat.

Fungsi Kuadrat dan Bentuk Parabolanya

Fungsi kuadrat adalah fungsi yang memiliki bentuk umum:

                                         f (x) = ax2 + bx + c

dengan a = 0. Ciri khas fungsi kuadrat adalah variabel x berpangkat paling tinggi dua.

Berbeda dengan fungsi linear yang grafiknya berupa garis lurus, grafik fungsi kuadrat
berupa parabola — sebuah kurva mulus yang simetris dan melengkung.

                                                                               23
Bentuk parabola ini tidak tetap; ia bergantung pada dua hal utama:

  1. Nilai a (koefisien dari x2), yang menentukan arah keterbukaan parabola.
 2. Nilai Diskriminan D, yang menentukan bagaimana parabola memotong sumbu-x.

Mari kita bahas satu per satu.

Pengaruh Nilai a terhadap Bentuk Parabola

Nilai a adalah "kompas" yang menentukan ke arah mana parabola membuka.

Nilai  Arah Parabola                        Titik Puncak   Sifat

a

a > 0 Terbuka ke atas (seperti senyum)      Titik minimum  Mempunyai nilai
                                                           terkecil

a<0    Terbuka ke bawah (seperti            Titik          Mempunyai nilai
       cemberut)                            maksimum       terbesar

  • Ketika a positif, parabola membuka ke atas, artinya ada titik terendah (minimum)

    pada grafik. Nilai fungsi akan mengecil lalu membesar kembali.

  • Ketika a negatif, parabola membuka ke bawah, artinya ada titik tertinggi

    (maksimum). Nilai fungsi akan membesar lalu mengecil kembali.

Selain arahnya, besar kecilnya nilai a juga memengaruhi "kegemukan" parabola:
semakin besar ∣a∣, semakin sempit dan runcing parabolanya; semakin kecil ∣a∣,

semakin lebar dan landai bentuknya. Titik balik (puncak) inilah yang menjadi pusat
simetri parabola.

Diskriminan D = b2 − 4ac dan Pengaruhnya pada Grafik

Langkah penting kedua adalah menghitung diskriminan, yaitu:

                                  D = b2 − 4ac

Diskriminan memberi tahu kita berapa banyak titik potong grafik dengan sumbu-x. Ini
sangat membantu saat menggambar, karena kita langsung tahu apakah parabola
menyentuh, memotong, atau sama sekali tidak menyentuh sumbu-x.

                                        24
Nilai        Banyak Titik Potong           Posisi Grafik
Diskriminan  Sumbu-x

D>0          Dua titik potong berbeda      Parabola memotong sumbu-x di dua
D=0                                        tempat
D<0
             Satu titik potong (titik      Parabola menyinggung sumbu-x tepat di
             singgung)                     puncaknya

             Tidak ada titik potong        Parabola sama sekali tidak menyentuh
                                           sumbu-x

Dengan menggabungkan informasi dari a dan D, kita sudah bisa membayangkan

bentuk parabola sebelum menggambarnya secara detail:

  • Jika a > 0 dan D < 0, parabola terbuka ke atas dan "melayang" di atas sumbu-x

    (selalu bernilai positif).

  • Jika a < 0 dan D > 0, parabola terbuka ke bawah dan memotong sumbu-x di dua

    titik.

  • Jika D = 0, puncak parabola tepat menyentuh sumbu-x, apa pun arah

    keterbukaannya.
Langkah praktis menggambar fungsi kuadrat:

  1. Tentukan arah keterbukaan dari tanda a.
 2. Hitung diskriminan D = b2 − 4ac untuk mengetahui titik potong sumbu-x.
 3. Cari titik potong sumbu-y dengan menghitung f (0) = c.

 4. Tentukan titik puncak (titik balik) sebagai pusat simetri.

 5. Hubungkan titik-titik tersebut menjadi kurva parabola yang mulus.

Fungsi Banyak Aturan (Piecewise)

Sekarang kita beralih ke jenis fungsi yang sedikit berbeda: fungsi banyak aturan.
Dinamakan demikian karena fungsi ini didefinisikan oleh beberapa rumus sekaligus,
masing-masing berlaku pada selang (interval) tertentu dari domainnya.

Bentuk umumnya dapat dituliskan sebagai berikut:

                                       25
f (x) =  g1(x),  syarat 1
         g2(x),  syarat 2

         ⋮       syarat n
         gn(x),

Setiap baris berisi aturan (rumus gi(x)) beserta syarat kapan aturan itu berlaku. Saat

menggambar grafiknya, kunci utamanya adalah menggambar setiap potongan
secara terpisah sesuai selangnya, lalu menggabungkannya dalam satu bidang
koordinat.

Perhatikan hal penting berikut saat menggambar fungsi banyak aturan:

  • Perhatikan tanda pertidaksamaan. Simbol ≤ atau ≥ berarti titik ujung termasuk
    (digambar dengan titik penuh/bulat). Simbol < atau > berarti titik ujung tidak

    termasuk (digambar dengan titik kosong/lingkaran).

  • Gambar potongan demi potongan pada selang yang diminta saja, bukan seluruh
    domain.

  • Periksa kesinambungan di titik pertemuan antar selang; grafik bisa tersambung
    mulus, bisa juga "melompat".

Contoh Grafik Fungsi Banyak Aturan

Mari kita gambarkan fungsi berikut:

f (x) =  x2,     x≤0
         x,      0<x<1
         x + 2,  x≥1

Fungsi ini terdiri dari tiga potongan yang masing-masing menempati selang berbeda.

Potongan 1: f (x) = x2 untuk x ≤ 0
Ini adalah bagian dari parabola y = x2 yang hanya berlaku di sebelah kiri sumbu-y
(termasuk titik x = 0). Karena x ≤ 0, titik (0, 0) ikut termasuk dan digambar dengan
titik penuh. Contoh titik: (−1, 1), (−2, 4), dan (0, 0).

Potongan 2: f (x) = x untuk 0 < x < 1

         26
Ini adalah segmen garis lurus y = x yang berlaku di antara x = 0 dan x = 1. Karena
tanda pertidaksamaannya tegas (tanpa "sama dengan"), maka titik ujung x = 0 dan
x = 1 tidak termasuk — digambar dengan titik kosong. Contoh titik: (0,5; 0,5),
sedangkan (0, 0) dan (1, 1) hanya sebagai batas.
Potongan 3: f (x) = x + 2 untuk x ≥ 1

Ini adalah garis lurus dengan kemiringan 1 yang digeser ke atas dua satuan, dan

berlaku mulai dari x = 1 ke kanan. Titik (1, 3) ikut termasuk (titik penuh). Contoh titik:
(1, 3), (2, 4), (3, 5).

Cara menggabungkannya: Gambar ketiga potongan pada satu bidang koordinat.

Pada x → 0, potongan pertama berakhir di titik penuh (0, 0), sementara potongan
kedua mulai tepat setelahnya dengan titik kosong. Pada x = 1, potongan kedua
berakhir di titik kosong (1, 1), sedangkan potongan ketiga mulai di titik penuh (1, 3).
Perhatikan bahwa di x = 1 grafik melompat dari ketinggian 1 ke ketinggian 3 — inilah

salah satu ciri menarik fungsi banyak aturan.

Rangkuman Cepat
  • Fungsi kuadrat f (x) = ax2 + bx + c bergrafik parabola.
  • Tanda a menentukan arah: a > 0 terbuka ke atas (titik minimum), a < 0 terbuka ke

    bawah (titik maksimum).

  • Diskriminan D = b2 − 4ac menentukan banyak titik potong sumbu-x: D > 0 dua
    titik, D = 0 satu titik, D < 0 tidak ada.

  • Fungsi banyak aturan didefinisikan oleh beberapa rumus pada selang berbeda;
    gambarlah tiap potongan sesuai syaratnya.

  • Perhatikan simbol ≤, ≥ (titik penuh) dan <, > (titik kosong) di setiap batas selang.
Dengan memahami hubungan antara nilai a, diskriminan, dan syarat tiap potongan,

kamu sudah punya bekal lengkap untuk menggambar kedua jenis grafik fungsi ini
dengan percaya diri. Selamat berlatih!

                                                                               27
Operasi Aljabar pada Fungsi

Pengantar: Saat Dua Fungsi "Bekerja Sama"

Halo! Selamat datang di bab yang membahas Operasi Aljabar pada Fungsi. Kalau
sebelumnya kita sudah mengenal apa itu fungsi dan bagaimana menentukan daerah
asalnya, sekarang saatnya kita melangkah lebih jauh. Kita akan belajar bagaimana
menggabungkan dua fungsi — layaknya menambahkan dua resep, mengurangi,
mengalikan, bahkan membaginya — untuk menghasilkan fungsi baru.

Kabar baiknya: konsep di bab ini sebenarnya cukup intuitif. Jika kamu sudah nyaman
dengan operasi aljabar biasa (penjumlahan, pengurangan, perkalian, pembagian)
pada bilangan, maka kamu sudah setengah jalan memahami bab ini. Yang perlu kita
tambahkan hanyalah satu perhatian khusus, yaitu soal daerah asal (domain) dari
fungsi hasil operasi tersebut.

Mari kita bedah satu per satu, secara santai tapi menyeluruh.

Konsep Dasar: Dua Fungsi, Dua Domain

Sebelum masuk ke operasi, mari kita sepakati dulu dasarnya. Misalkan kita punya dua

fungsi, yaitu f (x) dan g(x). Masing-masing mempunyai daerah asal (daerah asal

sering disebut  ):

• f (x) memiliki daerah asal Df
• g(x) memiliki daerah asal Dg

Daerah asal ini penting sekali. Ingat, sebuah fungsi hanya "hidup" atau terdefinisi pada

nilai-nilai x yang termasuk dalam daerah asalnya. Jadi ketika kita menggabungkan
dua fungsi, hasil gabungannya pun hanya bisa hidup pada nilai x yang diterima oleh

keduanya sekaligus.

Konsep kunci inilah yang menjadi benang merah seluruh bab ini: irisan daerah asal.

Simbolnya ∩, yang artinya "irisan" atau "yang dimiliki bersama".

Operasi Penjumlahan dan Pengurangan Fungsi

Ini operasi yang paling mudah. Kita cukup menjumlahkan atau mengurangkan nilai
kedua fungsi pada titik yang sama.

Rumusnya:

                                 28
                                      (f + g)(x) = f (x) + g(x)

                                      (f − g)(x) = f (x) − g(x)

Aturan daerah asalnya:

                              Df+g = Df ∩ Dg Df−g = Df ∩ Dg

Artinya, fungsi hasil penjumlahan (atau pengurangan) hanya terdefinisi pada nilai x
yang ada di Df sekaligus ada di Dg.
Contoh konkret: Misalkan f (x) = x + 2 dengan Df = (semua bilangan real) dan
g(x) = x dengan Dg = {x ∣ x ≥ 0}.

Maka:

  • (f + g)(x) = (x + 2) + x = x + 2 + x
  • (f − g)(x) = (x + 2) − x = x + 2 − x
Daerah asalnya adalah Df ∩ Dg = ∩ {x ≥ 0} = {x ∣ x ≥ 0}.
Perhatikan: meskipun f (x) sendiri terdefinisi di semua bilangan real, fungsi
gabungannya "tertahan" oleh batas dari g(x). Inilah kekuatan aturan irisan tersebut —

ia menjaga agar hasil gabungan tidak "berbohong" dengan mengklaim terdefinisi di
tempat yang sebenarnya tidak.

Operasi Perkalian Fungsi

Prinsipnya sama, hanya operatornya berubah menjadi perkalian.
Rumusnya:

                                       (f ⋅ g)(x) = f (x) ⋅ g(x)

Aturan daerah asalnya:

                                                                               29
                                            Df⋅g = Df ∩ Dg

Perhatikan bahwa aturan domain untuk perkalian sama persis dengan penjumlahan
dan pengurangan: tetap irisan dari kedua daerah asal. Tidak ada syarat tambahan
khusus seperti "hasil tidak boleh negatif" dan sejenisnya. Jadi jangan tertipu — baik
penjumlahan, pengurangan, maupun perkalian, ketiganya memakai aturan domain
yang identik.

Contoh konkret: Misalkan f (x) = x − 1 dengan Df = dan g(x) = x + 3 dengan
Dg = {x ∣ x ≥ −3}.

Maka:

                        (f ⋅ g)(x) = (x − 1) x + 3

Daerah asalnya:

                        Df⋅g = ∩ {x ≥ −3} = {x ∣ x ≥ −3}

Sederhana, bukan? Selama kedua fungsi bisa "dihidupkan" pada suatu titik x, maka

hasil perkaliannya juga hidup di titik itu.

Operasi Pembagian Fungsi (Perhatikan Syaratnya!)

Nah, bagian ini yang paling menarik sekaligus paling sering menjebak. Saat kita
membagi dua fungsi, muncul satu syarat tambahan yang tidak boleh kita lupakan.
Rumusnya:

                 f      f (x)
                        (x) = , dengan syarat g(x) = 0
                 g      g(x)

Aturan daerah asalnya:

                               30
Df/g = Df ∩ Dg − {x ∣ g(x) = 0}

Mari kita baca aturan ini dengan teliti, karena ada dua langkah:

  1. Ambil irisan dulu: Df ∩ Dg — sama seperti operasi lainnya.

 2. Buang titik-titik pembuat nol: kemudian kita keluarkan semua nilai x di mana
    g(x) = 0.

Kenapa harus dibuang? Karena pembagian dengan nol tidak terdefinisi dalam

matematika. Jika ada nilai x yang membuat penyebut g(x) menjadi nol, maka di titik

itu hasil bagi tidak punya arti. Maka kita harus mengeluarkannya dari daerah asal.

Contoh konkret: Misalkan f (x) = x + 1 dengan Df = dan g(x) = x − 2 dengan
Dg = .

Langkah 1 — Bentuk fungsi hasil bagi:

                                   f  (x)  =  x+1
                                   g          x−2

Langkah 2 — Tentukan irisan domain:

                                        Df ∩ Dg = ∩ =
Langkah 3 — Cari nilai yang membuat g(x) = 0:

x−2=0⇒x=2

Langkah 4 — Buang nilai tersebut:

Df/g = − {2} = {x ∣ x = 2}

                                      31
Jadi, meskipun kedua fungsi asalnya terdefinisi di seluruh bilangan real, hasil baginya

tidak terdefinisi di x = 2. Inilah mengapa langkah pembuangan nilai nol begitu krusial

— dan inilah beda utama pembagian dibanding tiga operasi lainnya.

Tabel Ringkasan Operasi dan Domain

Agar semua mudah diingat, mari kita rangkum dalam satu tabel.

Operasi      Rumus                 Aturan Domain   Catatan Khusus

Penjumlahan  (f + g)(x) =          Df ∩ Dg         Tidak ada syarat
             f (x) + g(x)                          tambahan

                     (f − g)(x) =  Df ∩ Dg         Tidak ada syarat
Pengurangan f (x) − g(x)                           tambahan

Perkalian    (f ⋅ g)(x) = f (x) ⋅  Df ∩ Dg         Tidak ada syarat
             g(x)                                  tambahan

Pembagian    f  (x)  =  f (x)      Df ∩ Dg − {x ∣  Wajib membuang nilai
             g          g(x)       g(x) = 0}
                                                   g(x) = 0

Pola yang bisa kamu pegang: tiga operasi pertama seragam, sementara pembagian
punya "bonus" pengurangan himpunan.

Kesalahan yang Sering Terjadi (dan Cara Menghindarinya)

Mari kita bahas beberapa jebakan umum, supaya kamu lebih waspada.

  • Lupa menghitung irisan domain. Banyak siswa hanya menuliskan rumus fungsinya
    lalu selesai, padahal domain hasil operasi harus ditentukan secara eksplisit.

  • Menganggap domain selalu . Tidak selalu! Fungsi seperti akar atau pecahan
    punya batasan, dan batasan itu akan "menular" ke hasil operasi.

  • Lupa membuang nilai nol pada pembagian. Ini jebakan paling klasik. Selalu periksa
    kapan penyebut bernilai nol.

  • Mengira perkalian punya aturan domain khusus. Tidak. Perkalian sama seperti
    penjumlahan dan pengurangan — hanya irisan.

                                   32
Rangkuman Akhir

Kita sudah menjelajahi seluruh operasi aljabar pada fungsi. Mari kita tarik benang
merahnya:

• Penjumlahan dan pengurangan: (f ± g)(x) = f (x) ± g(x), dengan domain Df ∩
 Dg .

• Perkalian: (f ⋅ g)(x) = f (x) ⋅ g(x), dengan domain Df ∩ Dg.

• Pembagian:  f  (x)  =  f (x)  dengan  g(x)  =  0,  dan  domain  Df  ∩  Dg  −  {x  ∣  g(x)  =
              g          g(x)

0}.

Inti dari seluruh bab ini ada dua hal: bentuk fungsinya (bagaimana menggabungkan
rumus) dan daerah asalnya (di mana fungsi gabungan itu sah hidup). Untuk tiga
operasi pertama, cukup ambil irisan domain. Untuk pembagian, tambahkan satu
langkah ekstra: buang titik yang membuat penyebut nol.

Kalau kamu sudah memahami kedua aspek ini, kamu siap melangkah ke materi
berikutnya, termasuk konsep fungsi komposisi dan fungsi invers. Selamat belajar, dan
jangan ragu untuk berlatih dengan contoh-contohmu sendiri — semakin banyak kamu
mencoba, semakin otomatis konsep ini terasa!

                                        33
Ringkasan dan Penerapan Konsep Fungsi

Halo! Selamat datang di bab rangkuman kita tentang fungsi. Bab ini akan membantu
kamu mengikat semua konsep yang sudah kita pelajari tentang fungsi, mulai dari
definisi dasar, domain, range, berbagai jenis fungsi, grafik, hingga operasi aljabar. Ini
adalah bekal penting sebelum kita masuk ke materi lanjutan seperti komposisi dan
fungsi invers, sekaligus pondasi untuk penerapan fungsi dalam sistem informasi.

Definisi Fungsi, Domain, dan Range

Secara sederhana, fungsi dari bilangan real ke bilangan real adalah suatu aturan yang

memadankan setiap nilai x dengan tepat satu nilai y. Notasinya f : x → y atau y =
f (x).

• x disebut peubah bebas (variabel independen).

• y disebut peubah tak bebas (variabel dependen), karena nilainya bergantung
 pada x.

Perhatikan kata "tepat satu" — inilah yang membedakan fungsi dari relasi biasa.

Contoh fungsi: f (x) = 2x2 + 4x + 4, f (x) =  x  +  1,  dan  f (x)  =  x  untuk  x  pada
                                                                       2

rentang tertentu.

Ada dua istilah kunci yang harus selalu kamu ingat:

  • Domain (daerah asal), dinotasikan Df , adalah himpunan semua nilai x yang
    membuat f (x) terdefinisi: Df = {x ∣ f (x) terdefinisi}.

  • Range (daerah nilai), dinotasikan Rf , adalah himpunan semua nilai y yang
    dihasilkan: Rf = {f (x) ∣ x ∈ Df }.

Contoh 1. Tentukan domain dan range dari f (x) = x2 + 2x + 4. Karena fungsi ini selalu
terdefinisi untuk setiap x, maka Df = (−∞, ∞). Dengan melengkapkan kuadrat,
f (x) = (x + 1)2 + 3, sehingga nilai terkecilnya adalah 3 dan Rf = [3, ∞).

Contoh 2. Untuk f (x) = x + 1, kita butuh x ≥ 0 agar akar terdefinisi, jadi Df =
[0, ∞). Karena x ≥ 0, maka f (x) ≥ 1, sehingga Rf = [1, ∞).

Jenis-Jenis Fungsi

Memahami jenis fungsi membantumu memprediksi bentuk grafik dan perilakunya.

1. Fungsi Polinom (Suku Banyak). Berbentuk f (x) = a0 + a1x + a2x2 + ⋯ + anxn.
Fungsi ini terdefinisi di seluruh bilangan real, jadi domainnya selalu (−∞, ∞).

                   34
2. Fungsi Rasional. Berbentuk f (x)  =  p(x)  dengan p(x) dan q(x) polinom serta q(x)  =
                                        q(x)

0. Fungsi ini terdefinisi di mana-mana kecuali di titik pembuat nol q(x).

Jenis     Contoh                                          Domain

Polinom   f (x) = x3 − 2x                                 (−∞, ∞)

Rasional  f (x)  =                   x2 +1                ∖ {−2, 2}
                                     x2 −4

Pada contoh rasional di atas, penyebut x2 − 4 = 0 saat x = 2 atau x = −2, sehingga

kedua titik itu dikeluarkan dari domain.

3. Fungsi Genap dan Ganjil. Keduanya dinilai dari simetri grafiknya:

  • Fungsi ganjil: f (−x) = −f (x). Grafiknya simetri terhadap titik asal. Contoh:
    f (x) = x3, karena f (−x) = (−x)3 = −x3 = −f (x).

  • Fungsi genap: f (−x) = f (x). Grafiknya simetri terhadap sumbu-y. Contoh:
    f (x) = x2, karena f (−x) = (−x)2 = x2 = f (x).

4. Fungsi Periodik. Fungsi f (x) disebut periodik dengan perioda p jika f (x + p) = f (x).
Contoh klasiknya adalah f (x) = sin x, yang periodik dengan perioda 2π.

Menggambar Grafik Fungsi
Grafik fungsi f adalah himpunan titik {(x, y) ∣ x ∈ Df , y ∈ Rf }.

a. Fungsi Linear. Berbentuk f (x) = ax + b, grafiknya garis lurus. Cara mudah
menggambarnya: cari titik potong sumbu-x (saat y = 0) dan sumbu-y (saat x = 0).

          y = x+1                                      x  y=0
                y x=0                             (0, 1)
(−1, 0)

b. Fungsi Kuadrat. Berbentuk f (x) = ax2 + bx + c, grafiknya parabola. Bentuk
parabola bergantung pada nilai a (terbuka ke atas jika a > 0, ke bawah jika a < 0)
dan diskriminan D = b2 − 4ac yang menentukan jumlah titik potong dengan sumbu-
x.

c. Fungsi Banyak Aturan (Piecewise). Fungsi yang didefinisikan berbeda pada interval

berbeda: f (x) = g1(x) untuk suatu selang, g2(x) untuk selang lain, dan seterusnya.

                                              35
                       x2, x ≤ 0
           f (x) = x, 0 < x < 1

                       2, x ≥ 1

Operasi Aljabar pada Fungsi
Jika f (x) dan g(x) punya domain Df dan Dg, maka:

Operasi    Rumus                                   Domain

Penjumlahan/pengurangan (f ± g)(x) = f (x) ± g(x) Df ∩ Dg

Perkalian  (f ⋅ g)(x) = f (x) ⋅ g(x)               Df ∩ Dg
Pembagian                                          Df ∩ Dg kecuali g(x) = 0
           f  (x)  =  f (x)
           g          g(x)

Poin penting: domain hasil operasi adalah irisan domain kedua fungsi, ditambah

syarat tambahan g(x) = 0 untuk pembagian. Jadi selalu periksa kedua syarat ini!

Penerapan dalam Sistem Informasi

Konsep fungsi sangat relevan di dunia sistem informasi. Misalnya, domain dan range
membantu memastikan sebuah sistem hanya menerima input yang valid — persis
seperti fungsi yang hanya terdefinisi pada domainnya. Fungsi rasional mengingatkan
kita untuk menangani pembagian nol sebagai kasus error. Fungsi periodik dan
piecewise dapat memodelkan pola yang berulang atau aturan yang berbeda pada
kondisi berbeda, seperti tarif atau hak akses pengguna. Operasi aljabar pada fungsi
juga menjadi dasar ketika kita menggabungkan beberapa modul perhitungan menjadi
satu sistem yang lebih besar.

Persiapan ke Materi Lanjutan

Rangkuman ini adalah pijakan penting. Pemahaman tentang domain dan range akan

sangat kamu butuhkan saat mempelajari komposisi fungsi (f ∘ g)(x) = f (g(x)), di
mana range g harus beririsan dengan domain f . Begitu pula, konsep fungsi satu-satu

dan operasi aljabar menjadi kunci dalam memahami fungsi invers, karena invers
hanya ada bila fungsi tersebut berkorespondensi satu-satu. Kuasai semua dasar di

                      36
bab ini dengan baik, dan materi berikutnya akan terasa jauh lebih mudah. Semangat
belajar!

                                                                               37
