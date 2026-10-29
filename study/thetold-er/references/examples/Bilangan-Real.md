---
mode: detailed
pages: 35
words: 7358
---

pelajarin.ai

Pendahuluan dan Relevansi Bilangan Real dalam Sistem
Informasi

Pendahuluan: Mengapa Bilangan Real Menjadi Fondasi Sistem
Informasi

Halo! Selamat datang di perjalanan kita memahami salah satu fondasi terpenting

dalam matematika Sistem Informasi: sistem bilangan real. Mungkin kamu bertanya-

tanya, "Kenapa sih anak Sistem Informasi harus belajar bilangan real? Bukankah itu

cuma urusan matematika murni?" Nah, justru di sinilah letak kejutan menariknya —

hampir semua yang kamu bangun sebagai profesional SI, dari aplikasi sederhana

sampai model  canggih, berdiri di atas sistem bilangan ini. Mari kita

bongkar bersama mengapa demikian.

Capaian Pembelajaran Matematika Sistem Informasi

Sebelum menyelami lebih dalam, penting untuk memahami apa yang diharapkan
setelah mempelajari bab ini. Berikut capaian pembelajaran yang menjadi target kita
dalam perkuliahan Matematika Sistem Informasi:

• Memahami konsep dasar bilangan real dan strukturnya, sehingga kita dapat
  memandangnya bukan sekadar angka, melainkan sebuah sistem yang
  terorganisasi.

• Mengidentifikasi dan mengklasifikasikan jenis-jenis bilangan (N, Z, Q, I, R) —
  kemampuan ini krusial karena setiap tipe bilangan memiliki peran berbeda dalam
  pemrograman.

• Menggunakan sifat-sifat aljabar bilangan real dalam operasi matematika,
  termasuk ketika menterjemahkannya menjadi operasi komputasi.

• Memahami relasi urutan dan sifat-sifat pertidaksamaan, yang mendasari logika
  perbandingan dan kondisi dalam kode.

• Memahami konsep kelengkapan bilangan real melalui  dan                            —
  pondasi analisis numerik tingkat lanjut.

• Menyelesaikan pertidaksamaan linear dan majemuk dalam konteks Sistem

Informasi, misalnya sebagai batasan (     ) pada optimasi sistem.

                                       1
Semua capaian ini bukan sekadar teori — mereka adalah keterampilan berpikir yang
akan menopang pekerjaanmu di dunia nyata.

Mengapa Bilangan Real Penting dalam Sistem Informasi?

Bilangan real menyusup ke hampir setiap lapisan pekerjaan Sistem Informasi. Mari kita
lihat empat area kunci.

1. Algoritma & Pemrograman. Setiap algoritma melakukan kalkulasi numerik,

mengevaluasi logika kondisi, dan menjalankan iterasi yang berbasis bilangan real.

Ketika kamu menulis                     , kamu sedang menggunakan bilangan real

untuk mengambil keputusan.

2. Database & Pengukuran Data. Basis data sering menyimpan nilai desimal (misalnya

harga produk               ), kapasitas penyimpanan, dan hasil pengukuran presisi

tinggi. Tipe data seperti         atau     di SQL adalah perwujudan langsung dari

bilangan real.

3. Statistik & Analisis Data. Rata-rata, deviasi standar, dan korelasi — semua konsep ini
menggunakan bilangan real sebagai bahan bakar. Tanpa bilangan real, pengambilan
keputusan berbasis data menjadi tidak mungkin.

4. Machine Learning & Komputasi Numerik. Bobot pada               , model

prediktif, dan proses optimasi bekerja pada ruang bilangan real kontinu. Setiap kali

sebuah model "belajar", ia sedang menyesuaikan nilai-nilai real.

Konsep Dasar Bilangan dan Representasinya

Sebelum lebih jauh, mari kita sepakati definisi dasarnya. Bilangan adalah representasi
kuantitas dan posisi suatu nilai dalam matematika. Sedangkan sistem bilangan
adalah cara penulisan dan pengorganisasian bilangan menggunakan simbol tertentu.
Ada beberapa sistem bilangan yang wajib kamu kenal:

Sistem Bilangan            Basis        Penggunaan Utama

Desimal                    10           Kehidupan sehari-hari

Biner                      2            Sistem komputer dan pemrograman

Oktal                      8            Penyimpanan data digital

                                        2
Heksadesimal     16                     Alamat memori dan penyimpanan digital

Biner dan heksadesimal sangat penting karena komputer "berbicara" dalam bahasa
ini. Misalnya, 1 byte = 8 bit, dan alamat memori biasanya ditulis dalam heksadesimal.

Contoh Konkret Bilangan dalam Kode Pemrograman

Teori ini akan terasa lebih nyata dengan melihatnya langsung di dalam kode:

•                → merepresentasikan bilangan bulat (integer) dalam kode.

•                → merepresentasikan bilangan desimal/real, penting untuk

   perhitungan presisi tinggi.

• Biner dan heksadesimal digunakan untuk merepresentasikan data di level mesin,
  dari alamat memori hingga bit penyimpanan.

Memahami perbedaan tipe data ini menyelamatkanmu dari  halus, misalnya
kesalahan pembulatan ketika menyimpan uang sebagai
                                                       alih-alih                 .

Bilangan Asli (N) dan Penerapannya dalam SI

Mari kita mulai klasifikasi dari yang paling dasar: bilangan asli. Definisi dan
konvensinya:

• Definisi: N = {1, 2, 3, 4, … } — himpunan bilangan bulat positif yang dimulai dari 1.

• Konvensi: Beberapa sistem memasukkan 0 ke dalam N (disebut bilangan cacah),
 namun secara standar N dimulai dari 1.

• Operasi Dasar: N bersifat tertutup (       ) terhadap penjumlahan dan perkalian.

   Artinya, hasil operasinya selalu tetap bilangan asli. Contoh: 3 + 5 = 8 ∈ N dan 4 ×

   7 = 28 ∈ N .

Lalu, di mana bilangan asli dipakai dalam Sistem Informasi? Ternyata sangat banyak:

• Penomoran record dan indeks database, seperti ID: 1, 2, 3, ... yang unik untuk setiap
  baris.

• Iterasi loop dalam algoritma, misalnya               .

• Menghitung jumlah elemen dalam sebuah array.

• Pengalamatan memori dan pointer, yang menggunakan indeks bilangan bulat
  positif.

                                          3
Bayangkan sebuah tabel  di database: setiap pengguna punya ID unik berupa

bilangan asli. Inilah wujud paling nyata dari N dalam pekerjaanmu sehari-hari.

Menutup Bab: Benang Merah yang Menghubungkan Semuanya

Dari algoritma, database, statistik, hingga     , satu benang merah

menyatukan semuanya: bilangan real dan keluarganya. Bilangan asli menangani

penomoran dan iterasi, sementara bilangan real menangani pengukuran presisi,

probabilitas, dan optimasi kontinu. Memahami struktur, sifat aljabar, relasi urutan, serta

contoh konkret dalam kode akan membuatmu bukan hanya sekadar pengguna alat,

tetapi pemikir yang memahami                 sistem bekerja seperti itu.

Di bab-bab selanjutnya, kita akan menyelami masing-masing jenis bilangan (Z, Q, I, R)

secara lebih mendalam, termasuk sifat kelengkapan melalui                 dan    ,

serta bagaimana pertidaksamaan menyelesaikan masalah nyata dalam Sistem

Informasi. Sampai jumpa di bab berikutnya — dan jangan ragu untuk bereksperimen

dengan kode-kode sederhana di atas, karena cara terbaik memahami bilangan

adalah dengan menggunakannya!

                                             4
Konsep Dasar dan Klasifikasi Bilangan

Halo! Selamat datang di bab pertama yang akan membuka pintu pemahaman kita
tentang dunia bilangan. Topik ini mungkin terdengar mendasar, tetapi percayalah —
konsep klasifikasi bilangan adalah fondasi yang menopang hampir seluruh bidang
komputasi, analisis data, dan sistem informasi. Mari kita telusuri bersama, langkah
demi langkah, mulai dari yang paling sederhana hingga yang paling kompleks.

Bilangan Asli (N) dan Perannya

Bilangan asli adalah jenis bilangan paling intuitif yang kita kenal sejak kecil. Secara
definisi, bilangan asli (N) mencakup bilangan positif yang dimulai dari 1, 2, 3, dan
seterusnya. Bilangan ini digunakan untuk membilang dan mengurutkan objek —
misalnya, "ada 5 pengguna aktif" atau "ini adalah iterasi ke-3".
Dalam sistem informasi, bilangan asli memiliki penerapan yang sangat luas. Kita
menggunakannya untuk:

  • Menghitung jumlah entitas: total pengguna, jumlah transaksi, banyaknya baris
    data.

  • Memberi indeks atau urutan: nomor urut log, urutan prioritas tugas.
  • Menyatakan kuantitas diskrit: jumlah paket dalam jaringan, banyaknya iterasi

    algoritma.
Poin penting yang perlu kamu ingat: bilangan asli adalah bagian dari bilangan bulat.
Artinya, setiap bilangan asli otomatis merupakan bilangan bulat. Hubungan ini kita

tuliskan sebagai N ⊂ Z.
Bilangan Bulat (Z): Menambahkan Negatif dan Nol

Sekarang, mari kita perluas wawasan. Bilangan bulat (Z) didefinisikan sebagai:

                                 Z = {..., −3, −2, −1, 0, 1, 2, 3, ...}

Perhatikan bahwa himpunan ini mencakup bilangan negatif, nol, dan bilangan positif.
Kehadiran nol dan bilangan negatif inilah yang membedakannya dari bilangan asli.

                                                                                5
Representasi Garis Bilangan: Setiap bilangan bulat menempati posisi unik pada garis
bilangan. Semakin ke kanan, nilai bilangan semakin besar. Ini membantu kita

memvisualisasikan perbandingan, misalnya −5 < −2 < 0 < 3.

Mengapa bilangan bulat begitu penting? Karena banyak fenomena nyata tidak bisa
dijelaskan hanya dengan bilangan positif. Berikut penerapannya dalam sistem
informasi:

Penerapan                                            Contoh Konteks

Saldo rekening                                       Saldo bisa positif (kredit) atau negatif (overdraft)

Perubahan stok barang                                Stok bertambah (+10) atau berkurang (−4)

Pengukuran suhu                                      Suhu bisa di bawah nol, misalnya −5°C

Selisih dan perbandingan data                        Perbedaan dua nilai, misalnya 100 − 250 = −150

Indeks array dalam pemrograman                       Mengakses elemen, termasuk indeks 0

Bilangan Rasional (Q) dan Bentuk Pecahannya

Naik satu tingkat lagi, kita bertemu bilangan rasional (Q). Definisi formalnya: bilangan

yang  dapat   dinyatakan  dalam             bentuk   p  ,  di  mana  p  dan    q  adalah         bilangan       bulat
                                                     q

(p, q ∈ Z) dan q = 0. Syarat q = 0 sangat penting karena pembagian dengan nol tidak

terdefinisi.

Bilangan rasional mencakup tiga bentuk representasi utama:

• Pecahan langsung:       1  ,  −  3  ,  7  ,  0  .  Perhatikan   bahwa  7     =  7 dan       0  =     0, jadi bilangan
                          2        4     1     5                         1                    5

bulat pun termasuk bilangan rasional!

• Desimal berhenti (desimal yang berakhir): 0.5                      =   1  ,  0.75  =  3  ,  1.25     =  5  .
                                                                         2              4                 4

• Desimal berulang (desimal dengan pola berulang): 0.333...                                =     1  ,  0.666...  =  2  ,
                                                                                                 3                  3

0.142857...   =  1  .
                 7

Dari sini muncul hubungan himpunan yang indah: N ⊂ Z ⊂ Q. Setiap bilangan asli

adalah bilangan bulat, dan setiap bilangan bulat adalah bilangan rasional (karena

dapat ditulis sebagai p/1).

                                                               6
Dalam komputasi dan analisis data, bilangan rasional adalah fondasi yang tak
tergantikan:

• Pengukuran: panjang, berat, kapasitas penyimpanan (misalnya 1.5 GB).

• Persentase: tingkat keberhasilan, akurasi model (misalnya 87.5%).

• Rasio dalam analisis data: rasio kompresi,                    .

• Perhitungan rata-rata dan statistik deskriptif.

Bilangan Irrasional (I): Ketika Desimal Tak Berujung

Tidak semua bilangan bisa ditulis sebagai pecahan. Di sinilah bilangan irrasional (I)

berperan.   Definisi:  bilangan  yang  tidak dapat  dinyatakan  sebagai  p  dengan  p, q  ∈  Z
                                                                         q

dan q = 0.

Ciri khas bilangan irrasional adalah desimal tak berhenti dan tak berulang — tidak
ada pola pengulangan digit dalam ekspansi desimalnya. Beberapa contoh klasik:

• 2 ≈ 1.41421356...

• 3 ≈ 1.73205080...

  • π ≈ 3.14159265...

Keberadaan bilangan irrasional ini melengkapi garis bilangan real dan sangat penting
dalam komputasi numerik, misalnya saat menghitung diagonal persegi atau
memodelkan lingkaran. Karena ekspansinya tak berujung, komputer hanya bisa
menyimpannya sebagai aproksimasi dengan presisi terbatas.

Peta Hubungan Semua Himpunan Bilangan

Mari kita rangkum dalam satu tabel agar mudah diingat:

Himpunan               Notasi          Cakupan                     Contoh

Asli                   N               1, 2, 3, ...                5, 12

Bulat                  Z               Negatif, nol, positif       −7, 0, 42

Rasional               Q               p/q, q = 0                 1/2, 0.75, 0.333...

Irrasional             I               Bukan pecahan               √2, π

                                       7
Real  R  Gabungan Q dan I  Semua di atas

Hubungan inklusi: N ⊂ Z ⊂ Q ⊂ R dan I ⊂ R. Perhatikan bahwa himpunan irrasional

dan rasional saling lepas (tidak ada irisan), tetapi keduanya bersama-sama
membentuk himpunan bilangan real (R).

Contoh Klasifikasi dalam Konteks Komputasi

Untuk memperkuat pemahaman, mari klasifikasikan beberapa nilai nyata:
  • Jumlah pengguna aktif 1500 → bilangan asli dan bulat.
  • Suhu server −8 → bilangan bulat (yang juga rasional).
  • Akurasi model 0.875 → bilangan rasional.
  • Nilai desimal berulang saat membagi data, 0.333... → bilangan rasional.
  • Perhitungan diagonal layar beresolusi tertentu yang melibatkan 2 → bilangan
    irrasional.

Penutup

Hebat! Kamu sekarang sudah memahami peta lengkap klasifikasi bilangan — dari
bilangan asli yang kita gunakan sehari-hari untuk membilang, hingga bilangan
irrasional yang menuntut pendekatan aproksimasi dalam komputasi. Ingat rantai

hubungan kuncinya: N ⊂ Z ⊂ Q ⊂ R, dengan I ⊂ R. Dengan fondasi ini, kamu siap

melangkah ke bab berikutnya tentang pengolahan data dan analisis numerik dengan
lebih percaya diri.

         8
Garis Bilangan Real dan Sifat Urutan

Halo! Selamat datang di bab yang akan membantu kita "melihat" bilangan real secara
nyata. Kalau selama ini bilangan terasa cuma deretan angka di kertas, di sini kita akan
belajar memvisualisasikannya pada sebuah garis lurus. Yuk, kita mulai dari konsep
dasarnya!

Apa Itu Bilangan Real?

Bilangan Real () adalah gabungan dari bilangan Rasional (Q) dan bilangan
Irrasional (I):

                                                   =∪

Ini artinya, apa pun jenis bilangan yang bisa kita pikirkan — positif, negatif, nol,
pecahan, desimal, sampai akar yang tidak rapi — semuanya masuk ke dalam keluarga
besar bilangan real. Hubungan antar himpunan bilangan bisa digambarkan seperti ini:

                                               ⊂⊂ ⊂

                        ⊂

Tanda ⊂ berarti "himpunan bagian dari". Jadi bilangan asli adalah bagian dari

bilangan bulat, bilangan bulat bagian dari rasional, dan seterusnya.

Klasifikasi Bilangan

Sebelum masuk ke garis bilangan, ada baiknya kita kenalan dulu dengan anggota-
anggota keluarga bilangan real.

Jenis  Notasi           Contoh   Ciri Khas

Asli   = {1, 2, 3, … }  1, 2, 3  Tidak ada nol dan negatif;
                                 untuk menghitung

                        9
Bulat          =                        −5, 0, 7              Mencakup negatif, nol, dan
             {… , −2, −1, 0, 1, 2, … }                        positif

Rasional        = {p/q ∣ p, q ∈ , q =                               Desimal berhenti atau
             0}
                                        1/2, −3/4, 0,5

                                                                     berulang

Irrasional                              2, 3, π               Desimal tak berhenti dan
                                                              tak berulang

Bilangan Rasional punya pola yang jelas: bentuk desimalnya berhenti (seperti 0,75)
atau berulang (seperti 0,333 …). Karena sifatnya yang rapi inilah rasional sering

dipakai untuk persentase, rasio, dan pengukuran data.

Bilangan Irrasional justru sebaliknya — desimalnya terus berjalan tanpa pernah

berhenti dan tanpa pola pengulangan. Contohnya 2 ≈ 1,414 … dan
π ≈ 3,14159 …. Meskipun "tidak rapi", bilangan ini tetap punya tempat pasti di garis

bilangan, lho!

Garis Bilangan Real: Melihat Bilangan Secara Visual

Garis bilangan real adalah representasi visual dari seluruh bilangan real pada sebuah
garis lurus. Aturan emasnya sederhana:

Ini yang disebut sifat urutan. Mari kita tempatkan beberapa titik penting pada garis:

Perhatikan posisi masing-masing:

• Bilangan negatif (−2, −1) selalu berada di kiri nol.

• Nol menjadi titik acuan di tengah.

•  Bilangan  positif  (  1  ,  2, 2, π) berada di kanan nol.
                         2

• Bilangan irasional seperti 2 ≈ 1,414 dan π ≈ 3,14 memiliki posisi pasti pada

   garis, meskipun nilainya tidak bisa ditulis secara eksak.

Dari posisi ini kita bisa membaca urutannya:

                                        10
                                   −2    <     0  <  1  <   2<2<π
                                                     2

Simbol dan Makna Urutan

Untuk membandingkan bilangan, kita pakai simbol-simbol berikut:

   Simbol         Arti                                      Contoh

   <              Kurang dari                               2<5

   >              Lebih dari                                7>3

   ≤              Kurang dari atau sama dengan              x ≤ 4 (boleh kurang, boleh sama)

   ≥              Lebih dari atau sama dengan               x≥0

   =              Sama dengan                               0,5  =  1
                                                                    2

Tips mengingat: ujung simbol yang "membuka lebar" selalu menghadap bilangan

yang lebih besar. Jadi pada 2 < 5, sisi lebar menghadap 5.

Sifat Transitif: Rantai Urutan

Inilah sifat yang membuat urutan sangat kuat dan konsisten:

            a<b b<c                   a<c

Sederhananya, urutan itu "menular" secara berantai. Contohnya, karena −2 < 0 dan

0  <  1  ,  maka  otomatis  −2  <  1  .  Kita  bisa  menyambung  rantai  ini  sepanjang  apa  pun:
      2                            2

                                   −2    <     0  <  1  <   2<2<π
                                                     2

Dari rantai ini, kita tahu langsung bahwa −2 < π tanpa perlu menghitung apa-apa

lagi. Sifat transitif inilah fondasi dari semua pembandingan bilangan.

                                                        11
Hubungan Urutan dengan Algoritma

Mengapa semua ini penting untuk komputasi? Karena setiap algoritma pengambilan
keputusan pada akhirnya bertumpu pada perbandingan urutan. Ketika komputer:

  • Mengurutkan data (sorting), ia berulang kali bertanya "apakah nilai ini lebih kecil
    dari nilai itu?"

  • Mencari nilai maksimum/minimum, ia membandingkan satu nilai dengan nilai
    lain.

  • Menentukan kondisi (misalnya "jika suhu ≥ 100, maka didih"), ia memakai simbol ≥
    atau ≤.

Sifat transitif juga membuat algoritma pengurutan bekerja efisien: daripada
membandingkan setiap pasangan, kita cukup membangun rantai urutan yang
konsisten. Ditambah sifat-sifat aljabar bilangan real seperti tertutup, komutatif,
asosiatif, distributif, identitas, dan invers, semua operasi dalam algoritma jadi punya
perilaku yang bisa diprediksi.
Singkatnya, memahami garis bilangan dan sifat urutan bukan sekadar latihan teori —
ini adalah fondasi komputasi numerik dan analisis data. Dengan menguasainya, kita
bisa membaca hubungan antar bilangan sekilas, membangun rantai perbandingan
dengan percaya diri, dan memahami cara algoritma "berpikir" saat mengambil
keputusan.
Selamat belajar, dan semoga garis bilangan ini membuat matematika terasa lebih
nyata dan ramah!

                                                                               12
Sifat-Sifat Aljabar Bilangan Real

Halo! Selamat datang di bab yang akan menjadi fondasi penting bagi perjalananmu
dalam memahami matematika dan pemrograman. Di sini, kita akan menjelajahi sifat-
sifat dasar aljabar bilangan real. Mungkin beberapa konsep ini terdengar familiar dari
sekolah, tetapi percayalah, memahami "mengapa" di baliknya akan membuka pintu
menuju optimasi kode yang lebih cerdas dan komputasi numerik yang lebih efisien.
Mari kita mulai!
Sifat Tertutup: Dunia yang Terjaga
Sebelum menyelami sifat yang lebih kompleks, kita perlu mengenal yang paling
mendasar: sifat tertutup. Sederhananya, sifat ini menjamin bahwa ketika kita
melakukan operasi penjumlahan atau perkalian pada dua bilangan real, hasilnya akan
selalu menjadi bilangan real juga. Tidak ada "makhluk aneh" yang keluar dari sistem ini.

  • Penjumlahan: Jika a dan b adalah bilangan real, maka a + b juga bilangan real.
  • Perkalian: Jika a dan b adalah bilangan real, maka a × b juga bilangan real.

Ini mungkin terdengar sederhana, tapi inilah yang membuat sistem bilangan real
sangat kokoh dan bisa diandalkan untuk komputasi apapun.
Sifat Komutatif dan Asosiatif: Fleksibilitas dalam Berhitung
Dua sifat ini memberikan kita kebebasan untuk mengatur ulang operasi tanpa
mengubah hasilnya.
Sifat Komutatif (dari kata "commute" yang berarti berpindah) berarti urutan bilangan
dalam operasi penjumlahan atau perkalian tidak mempengaruhi hasil akhir. Kita bisa
bertukar posisi sesuka hati.

  • Penjumlahan: a + b = b + a
     ◦ Contoh: 3 + 5 = 5 + 3 = 8

  • Perkalian: a × b = b × a
     ◦ Contoh: 4 × 7 = 7 × 4 = 28

Sifat Asosiatif (dari kata "associate" yang berarti mengelompokkan) memberi kita
kebebasan untuk mengelompokkan bilangan dengan tanda kurung. Selama urutan

                                                                               13
operasinya sama, di mana kita meletakkan tanda kurung tidak akan mengubah
hasilnya.

  • Penjumlahan: (a + b) + c = a + (b + c)

   ◦ Contoh: (2 + 3) + 4 = 2 + (3 + 4) = 9
• Perkalian: (a × b) × c = a × (b × c)

◦ Contoh: (2 × 3) × 4 = 2 × (3 × 4) = 24

Bayangkan kamu sedang menjumlahkan banyak angka dalam sebuah program. Sifat
komutatif dan asosiatif memungkinkan compiler untuk mengatur ulang urutan
penjumlahan agar lebih efisien, misalnya dengan mengelompokkan angka-angka
yang bisa dihitung dengan cepat terlebih dahulu.

Sifat Distributif: Menyatukan Perkalian dan Penjumlahan
Inilah bintang utamanya! Sifat distributif menghubungkan perkalian dan
penjumlahan. Inilah kunci dari penyederhanaan ekspresi matematika dan merupakan
dasar dari banyak optimasi kode.

Rumus Dasar: a(b + c) = ab + ac

Sifat ini "mendistribusikan" perkalian a ke setiap suku di dalam kurung. Mari kita lihat

beberapa contoh:

• Contoh 1: 3(4 + 5) = 3 × 4 + 3 × 5 = 12 + 15 = 27

• Contoh 2: 2(x + 3) = 2x + 6

• Contoh 3: −4(2 + 7) = −4 × 2 + (−4) × 7 = −8 + (−28) = −36

Penerapan dalam Penyederhanaan Ekspresi: Sifat distributif memungkinkan kita untuk

memfaktorkan atau mengembangkan sebuah ekspresi. Misalnya, ekspresi 2x + 6 bisa

disederhanakan menjadi 2(x + 3). Dalam konteks pemrograman, ini sangat berguna.

Jika kita punya kode seperti                , kita bisa mengoptimalkannya menjadi

. Ini mengurangi jumlah operasi perkalian dari dua menjadi satu, yang bisa

sangat menghemat waktu eksekusi, terutama dalam loop yang besar atau komputasi

numerik yang intensif.

Hubungan dengan Algoritma & Pemrograman: Sifat distributif diterapkan dalam:

• Penyederhanaan ekspresi aritmatika: Kompiler sering menggunakan sifat ini untuk
  mengoptimalkan kode.

• Optimasi loop: Mengeluarkan operasi yang konstan dari dalam loop.

                               14
  • Distribusi operasi pada array/vektor: Dalam komputasi numerik, operasi pada
    seluruh array bisa didistribusikan untuk efisiensi.

Elemen Identitas: Angka yang Tidak Mengubah Apapun
Elemen identitas adalah sebuah bilangan yang, ketika dioperasikan dengan bilangan
lain, tidak akan mengubah nilai bilangan tersebut. Setiap operasi memiliki identitasnya
sendiri.

  • Identitas Penjumlahan: 0

     ◦ Rumus: a + 0 = a
     ◦ Contoh: 7 + 0 = 7

       ◦ Menambahkan nol tidak mengubah nilai apapun. Dalam pemrograman,
         menambahkan 0 seringkali tidak berguna, tetapi konsep ini penting untuk
         memahami struktur aljabar.

  • Identitas Perkalian: 1

     ◦ Rumus: a × 1 = a
     ◦ Contoh: 9 × 1 = 9

       ◦ Mengalikan dengan satu juga tidak mengubah nilai. Ini adalah dasar dari
         operasi "normalisasi" dalam komputasi numerik.

Sifat Invers: Kembali ke Identitas
Invers adalah "kebalikan" dari sebuah bilangan yang, ketika dioperasikan, akan
menghasilkan elemen identitas. Ini seperti tombol "undo" dalam matematika.

  • Invers Penjumlahan: Untuk setiap bilangan real a, ada bilangan −a sedemikian

    sehingga:

     ◦ Rumus: a + (−a) = 0
     ◦ Contoh: 5 + (−5) = 0

       ◦ Invers penjumlahan dari 5 adalah -5. Ini adalah dasar dari operasi
         pengurangan.

  • Invers Perkalian: Untuk setiap bilangan real a (dengan syarat a = 0), ada bilangan
    1/a sedemikian sehingga:
     ◦ Rumus: a × (1/a) = 1
     ◦ Contoh: 4 × (1/4) = 1

                                                                               15
     ◦ Invers perkalian dari 4 adalah 1/4. Ini adalah dasar dari operasi pembagian.

Syarat Penting a = 0: Perhatikan bahwa invers perkalian hanya ada jika a tidak sama
dengan nol. Mengapa? Karena kita tidak bisa membagi dengan nol. 1/0 tidak

terdefinisi. Dalam pemrograman, kesalahan "division by zero" adalah hal yang umum
dan harus selalu dihindari. Memahami konsep invers ini membantumu menulis kode
yang lebih aman dan robust.

Konsep Urutan Bilangan Real: Membandingkan Nilai
Selain sifat-sifat aljabar di atas, bilangan real juga memiliki konsep urutan. Ini
memungkinkan kita untuk membandingkan posisi relatif dua bilangan pada garis
bilangan.

Simbol dan Sifat Urutan:

  • Simbol:

◦ > (lebih besar dari)

◦ < (lebih kecil dari)

◦ ≥ (lebih besar atau sama dengan)

◦ ≤ (lebih kecil atau sama dengan)

   ◦ = (sama dengan)

• Contoh:

◦ −3 < 0 < 2 < 5

   ◦ 1/2 < 2 < 2

• Sifat Transitif:

◦ Jika a < b dan b < c, maka a < c.

     ◦ Contoh: Karena −3 < 0 dan 0 < 5, maka −3 < 5.

Hubungan dengan Garis Bilangan:

• Bilangan yang lebih kecil berada di sebelah kiri.

• Bilangan yang lebih besar berada di sebelah kanan.

Sifat urutan ini menjadi dasar logika perbandingan dalam algoritma, validasi data, dan

pengambilan keputusan dalam sistem informasi. Misalnya, dalam sebuah program,

kita sering menulis     untuk membandingkan nilai dan mengambil keputusan

berdasarkan perbandingan tersebut.

                                     16
Kaitan dengan Optimasi Kode dan Komputasi Numerik
Memahami sifat-sifat aljabar ini bukan hanya tentang teori matematika. Ini adalah
alat praktis untuk menulis kode yang lebih baik.

  • Optimasi Kompilasi: Kompiler modern menggunakan sifat komutatif, asosiatif, dan
    distributif untuk mengatur ulang ekspresi matematika agar dieksekusi lebih cepat,
    misalnya dengan mengurangi jumlah operasi.

  • Efisiensi Algoritma: Dalam komputasi numerik, operasi matriks dan vektor sering
    memanfaatkan sifat distributif untuk mendistribusikan operasi ke seluruh elemen
    array, yang bisa dioptimalkan oleh hardware.

  • Keamanan Kode: Memahami invers perkalian dan syarat a = 0 membantumu

    menghindari kesalahan pembagian dengan nol.
  • Logika Perbandingan: Sifat urutan adalah dasar dari semua logika perbandingan

    dan pengambilan keputusan dalam kode.
Dengan menguasai sifat-sifat ini, kamu tidak hanya belajar matematika, tetapi juga
membangun fondasi untuk menjadi pemrogram yang lebih efektif dan efisien. Selamat
belajar, dan semoga konsep-konsep ini membantumu dalam petualangan codingmu!

                                                                               17
Interval dan Pertidaksamaan Linear

Interval: Membagi Garis Bilangan Menjadi Potongan yang Rapi

Halo! Mari kita berkenalan dengan salah satu konsep paling mendasar tapi super
penting dalam matematika: interval. Kalau kamu pernah menggambar garis bilangan
dan menandai suatu "wilayah" di atasnya, sebenarnya kamu sudah bersentuhan
dengan interval. Yuk, kita bongkar konsepnya secara menyeluruh!

Apa Itu Interval?
Interval adalah himpunan bilangan real yang terletak di antara dua nilai batas.
Bayangkan seperti sebuah pagar dengan dua tiang: semua bilangan yang "terjepit" di
antara kedua tiang itu adalah anggota interval.

Pertanyaan kuncinya adalah: apakah tiang pagarnya (titik ujung/endpoint) sendiri
termasuk di dalamnya? Jawaban atas pertanyaan inilah yang membedakan jenis-
jenis interval. Notasinya pun berbeda:

  • Kurung biasa () → titik ujung tidak termasuk

  • Kurung siku [] → titik ujung termasuk

Empat Jenis Interval dan Notasinya

Jenis                    Notasi Arti                                 Contoh
                                                                     Bilangan

Terbuka                  (a, b)  Lebih dari a, kurang dari b; ujung  a<x<b

                                 tidak termasuk

Tertutup                 [a, b]  Dari a sampai b, ujung termasuk     a≤x≤b

Setengah terbuka (kiri   [a, b) a termasuk, b tidak                  a≤x<b
tertutup)

Setengah terbuka (kanan  (a, b]  a tidak termasuk, b termasuk        a<x≤b
tertutup)

                                      18
Perhatikan pola sederhananya: kurung siku = "ikut", kurung biasa = "tidak ikut". Kalau
salah satu ujung pakai kurung siku dan ujung lainnya kurung biasa, itulah yang disebut
setengah terbuka.

Supremum dan Infimum: Batas yang Cerdas

Sebelum masuk ke pertidaksamaan, kita perlu memahami dua konsep batas yang
sering membingungkan tapi sangat elegan.

  • Supremum (sup A): batas atas terkecil dari himpunan A. Menariknya, supremum

    belum tentu menjadi anggota himpunan.

  • Infimum (inf A): batas bawah terbesar dari himpunan A. Sama seperti supremum,

    infimum juga belum tentu anggota himpunan.

Mari lihat contoh konkret. Ambil himpunan A = {x ∣ 0 < x < 1} (interval terbuka):
  • sup A = 1 → ini batas atas terkecil, tapi bukan maksimum karena 1 ∈/ A
  • inf A = 0 → ini batas bawah terbesar, tapi bukan minimum karena 0 ∈/ A

Jadi himpunan ini tidak punya maksimum maupun minimum, tetapi tetap punya
supremum dan infimum! Inilah keunikan yang sering menjadi jebakan konseptual.

Perbedaan Kunci: Max/Min vs Sup/Inf

Konsep      Harus Anggota      Sifat
            Himpunan?

Maksimum /  Ya, wajib          Nilai ekstrem yang benar-benar ada di
Minimum                        dalam

Supremum /  Tidak harus        Batas luar himpunan
Infimum

Intinya: sup dan inf bisa ada meskipun maks dan min tidak ada. Konsep ini sangat
penting untuk dipahami sebelum melangkah lebih jauh.

                           19
Sifat Kelengkapan Bilangan Real

Bilangan real ( ) punya sifat istimewa yang membedakannya dari bilangan rasional
( ): tidak ada "lubang" pada garis bilangan. Setiap titik pada garis bilangan
merepresentasikan tepat satu bilangan real.
Sifat Kelengkapan (Completeness Property):

  • Setiap himpunan bilangan real yang tidak kosong dan terbatas atas memiliki
    supremum.

  • Setiap himpunan yang terbatas bawah memiliki infimum.
Sifat ini adalah fondasi penting dalam analisis numerik dan komputasi — karena
menjamin tidak ada "celah" yang membuat perhitungan kita gagal.

Aturan Operasi pada Pertidaksamaan

Sekarang bagian yang paling praktis! Saat menyelesaikan pertidaksamaan, kita sering
memanipulasi kedua ruas. Ada aturan main yang wajib dipatuhi:

  1. Penjumlahan/pengurangan: Menambah atau mengurangi kedua ruas dengan
    bilangan yang sama tidak mengubah tanda pertidaksamaan.

     ◦ Jika a < b, maka a + c < b + c.

 2. Perkalian/pembagian dengan bilangan positif: Tanda pertidaksamaan tetap.

     ◦ Jika a < b dan c > 0, maka ac < bc.

 3. Perkalian/pembagian dengan bilangan negatif: Tanda pertidaksamaan berbalik

    (dari < menjadi >, atau sebaliknya). Ini yang paling sering bikin salah!
     ◦ Jika a < b dan c < 0, maka ac > bc.

Langkah Menyelesaikan Pertidaksamaan Linear Satu Variabel

Berikut alur sistematis yang bisa kamu ikuti:
  1. Sederhanakan kedua ruas (hilangkan tanda kurung, gabungkan suku sejenis).
 2. Kumpulkan semua suku yang mengandung variabel di satu ruas, dan konstanta di
    ruas lainnya.
 3. Selesaikan sehingga variabel berdiri sendiri di satu ruas.

                                                                               20
 4. Hati-hati saat mengalikan/membagi dengan bilangan negatif (balik tanda).
 5. Tuliskan solusi dalam notasi interval dan gambarkan pada garis bilangan.

Contoh Penyelesaian: 3x − 5 > 7

Mari kita kerjakan langkah demi langkah:
Langkah 1 — Kumpulkan konstanta:

                                               3x − 5 > 7

Tambahkan 5 ke kedua ruas (tanda tetap):

                                                 3x > 12

Langkah 2 — Bagi dengan koefisien variabel: Bagi kedua ruas dengan 3 (positif, tanda

tetap):

                                                   x>4

Langkah 3 — Tulis dalam notasi interval: Karena x > 4 (batas tidak termasuk),

solusinya adalah:

                                                  (4, ∞)

Langkah 4 — Gambar pada garis bilangan: Buat lingkaran kosong () pada angka 4
(karena 4 tidak termasuk), lalu tarik garis tebal ke arah kanan menuju tak hingga.
Contoh lain sebagai perbandingan — jika soal berbunyi −2x ≥ 8:

  • Bagi kedua ruas dengan −2 (negatif!) → tanda berbalik menjadi x ≤ −4
  • Notasi intervalnya: (−∞, −4] dengan lingkaran penuh () pada −4

                                                                               21
Penerapan: Validasi Data

Pertidaksamaan linear bukan cuma soal latihan di buku — ia sangat berguna di dunia
nyata, khususnya untuk validasi data. Bayangkan sebuah sistem menerima input suhu

yang harus berada dalam rentang aman, misalnya antara 0 (inklusif) hingga 100

(eksklusif). Kita bisa menuliskannya sebagai:

                                   0 ≤ T < 100 ⟺ [0, 100)

Sistem cukup menguji apakah nilai T memenuhi pertidaksamaan ini. Jika tidak, data

ditolak. Pola seperti ini dipakai dalam validasi form, pengecekan sensor, sampai
pembatasan parameter program.

Rangkuman Cepat

  • Interval = himpunan bilangan real di antara dua batas.

  • Kurung siku [] → ujung termasuk; kurung biasa () → ujung tidak termasuk.

  • Setengah terbuka = satu ujung termasuk, satu tidak.
  • Supremum/Infimum bisa ada tanpa maksimum/minimum.
  • Sifat kelengkapan menjamin tidak ada "lubang".
  • Mengali/membagi dengan bilangan negatif → balik tanda pertidaksamaan.
  • Solusi pertidaksamaan ditulis sebagai interval dan digambar di garis bilangan.
Selamat belajar! Dengan memahami aturan tanda dan notasi interval, menyelesaikan
pertidaksamaan linear akan terasa jauh lebih mudah. Semangat!

                                                                               22
Pertidaksamaan Majemuk dan Penerapannya dalam
Sistem Informasi

Pertidaksamaan Majemuk: Konsep, Penyelesaian, dan
Penerapannya

Halo! Selamat datang di bab yang membahas salah satu topik paling praktis dalam
aljabar: pertidaksamaan majemuk. Mungkin terdengar agak menakutkan, tapi tenang
saja — begitu kamu memahami aturannya, topik ini justru sangat berguna, terutama
ketika kita berbicara tentang sistem informasi, kapasitas server, dan validasi data. Yuk,
kita mulai dari dasar!

1. Mengingat Kembali Bilangan Real dan Aturan Operasi
Pertidaksamaan

Sebelum masuk ke pertidaksamaan majemuk, kita perlu memastikan fondasinya kuat.
Pertidaksamaan bekerja pada bilangan real — himpunan bilangan yang mencakup
bilangan bulat, pecahan, desimal, positif, negatif, dan nol. Ada beberapa aturan
operasi yang wajib kamu hafal:

Operasi              Aturan                           Contoh

Penjumlahan/         Jika a < b, maka a + c < b + c   3<7→3+2<7+
Pengurangan                                           2→5<9✓
                     (tanda tidak berubah)

Perkalian/Pembagian  Tanda tidak berubah              2<6→2×3<6×
                                                      3 → 6 < 18 ✓
dengan c > 0

Perkalian/Pembagian  Tanda berbalik arah!             2 < 6 → 2 × (−3) > 6 ×
                                                      (−3) → −6 > −18 ✓
dengan c < 0

  Aturan emas yang harus selalu diingat: Jika kamu mengalikan atau membagi kedua
ruas pertidaksamaan dengan bilangan negatif, maka tanda pertidaksamaan harus
dibalik. Ini adalah kesalahan paling umum yang dilakukan siswa, jadi berhati-hatilah!

Prinsip yang sama berlaku untuk pembagian: jika a  <  b dan c  >  0, maka  a  <  b  (tanda
                                                                           c     c

tetap). Namun jika c < 0, tanda berbalik.

                                           23
2. Menyelesaikan Pertidaksamaan Linear Sederhana

Mari kita mulai dengan contoh dasar agar pola pikirnya terbentuk. Selesaikan 3x −
5 > 7:

• Langkah 1 — Pindahkan konstanta: 3x − 5 > 7 → 3x > 7 + 5 → 3x > 12

• Langkah 2 — Bagi kedua ruas dengan 3 (positif, tanda tidak berubah): x  >  12  →
                                                                             3

x>4

• Langkah 3 — Notasi interval: (4, ∞)

• Langkah 4 — Garis bilangan: titik 4 berupa lingkaran terbuka (○), arah panah ke

 kanan menuju ∞

Karena pembaginya adalah +3 (positif), tanda pertidaksamaan tidak berbalik. Mudah,

kan?

3. Bentuk Umum Pertidaksamaan Majemuk

Pertidaksamaan majemuk adalah pertidaksamaan yang memuat dua tanda

pertidaksamaan sekaligus, misalnya a < x < b atau a ≤ x ≤ b. Intinya, variabel x

terjepit di antara dua batas nilai.

  Aturan kunci: Pada pertidaksamaan majemuk, operasi yang sama harus diterapkan
ke semua ruas secara bersamaan — bukan hanya satu ruas. Jika dikalikan atau dibagi
dengan bilangan negatif, tanda pertidaksamaan pada kedua sisi berbalik arah.

Bentuk umumnya dapat ditulis sebagai:

     a < ekspresi ≤ b

dengan a sebagai batas bawah dan b sebagai batas atas.

4. Langkah Penyelesaian: Contoh 2 < x + 3 ≤ 7

Mari kita selesaikan contoh utama bab ini langkah demi langkah:

Bentuk awal: 2 < x + 3 ≤ 7

Langkah 1 — Kurangi semua ruas dengan 3:

     2−3<x+3−3≤7−3

                                       24
Langkah 2 — Sederhanakan hasilnya:

                                               −1 < x ≤ 4

Langkah 3 — Nyatakan dalam notasi interval:

                                               x ∈ (−1, 4]

Langkah 4 — Gambarkan pada garis bilangan:

  • Titik −1 terbuka (○) karena tanda < berarti tidak termasuk
  • Titik 4 tertutup (●) karena tanda ≤ berarti termasuk
Kesimpulan: Himpunan solusinya adalah semua bilangan real x yang lebih dari −1
dan kurang dari atau sama dengan 4.
Perhatikan betapa pentingnya membedakan tanda < dan ≤ — lingkaran terbuka

versus tertutup pada garis bilangan adalah representasi visual dari perbedaan
tersebut.

5. Penerapan dalam Sistem Informasi

Inilah bagian yang paling menarik! Pertidaksamaan majemuk bukan sekadar latihan di
atas kertas — ia hadir di hampir setiap aspek teknologi yang kamu gunakan sehari-
hari.
5.1 Manajemen Kapasitas Penyimpanan

Bayangkan sebuah server penyimpanan yang sudah terisi 325 MB dan memiliki
kapasitas maksimum 500 MB. Jika kita menambahkan data sebesar x MB, kita

memerlukan:

                                             x + 325 ≤ 500

                                                                               25
Menyelesaikannya: x ≤ 500 − 325 → x ≤ 175.

Interpretasi: Kamu hanya boleh menambahkan paling banyak 175 MB data lagi agar

tidak melampaui kapasitas. Jika kamu menambahkan 176 MB, sistem akan melebihi

batas dan berpotensi gagal.
5.2 SLA (Service Level Agreement) dan Waktu Respons
Sebuah sistem sering kali memiliki jaminan waktu respons, misalnya:

                                               t < 2 detik

Interpretasi: Waktu respons t harus kurang dari 2 detik. Jika sistem merespons dalam
1,99 detik, itu memenuhi SLA. Namun 2,00 detik sudah melanggar karena tandanya
ketat (<).

5.3 Batas Ukuran File

Ketika sebuah platform menetapkan batas unggahan sebesar 10 MB:

                                               f ≤ 10 MB

Di sini tanda ≤ bersifat inklusif — file berukuran tepat 10 MB tetap diterima, sedangkan
10,01 MB ditolak.

5.4 Validasi Nilai Input
Ini contoh paling sempurna untuk pertidaksamaan majemuk! Misalnya sistem

penilaian yang hanya menerima nilai antara 0 hingga 100:

                                            0 ≤ nilai ≤ 100

Interpretasi:

  • Nilai −5 → tidak valid (di bawah batas bawah)
  • Nilai 0 → valid (batas bawah inklusif)
  • Nilai 75 → valid (berada dalam rentang)

                                                                               26
  • Nilai 100 → valid (batas atas inklusif)
  • Nilai 105 → tidak valid (di atas batas atas)

Inilah cara kerja validasi input di backend aplikasi — logika pertidaksamaan majemuk
tertanam langsung dalam kode.

6. Ringkasan Poin Penting

  • Pertidaksamaan majemuk memuat dua tanda pertidaksamaan dan operasi harus
    diterapkan ke semua ruas sekaligus.

  • Kalikan atau bagi dengan bilangan negatif tanda berbalik. Ini berlaku untuk
    pertidaksamaan tunggal maupun majemuk.

  • Tanda < menghasilkan lingkaran terbuka dan interval (a, b), sedangkan ≤
    menghasilkan lingkaran tertutup dan interval (a, b].

  • Penerapan nyata mencakup manajemen kapasitas (x + 325 ≤ 500), SLA waktu
    respons (t < 2 detik), batas ukuran file (f ≤ 10 MB), dan validasi nilai (0 ≤ nilai ≤
    100).

Dengan menguasai konsep ini, kamu tidak hanya lulus ujian matematika — kamu juga
memahami cara kerja sistem yang kamu gunakan setiap hari. Selamat belajar, dan
teruslah berlatih!

                                                                               27
Konsep Kelengkapan Bilangan Real: Supremum dan
Infimum

Halo! Setelah kita memahami bahwa bilangan real ( ) tersusun dari gabungan

bilangan rasional ( ) dan irrasional (I), kini saatnya kita menyelami salah satu sifat

paling fundamental yang membuat istimewa: sifat kelengkapan (completeness).
Sifat inilah yang membedakan garis bilangan real dari sekadar kumpulan bilangan
biasa. Mari kita bahas dengan santai namun menyeluruh.

Mengapa Kelengkapan Itu Penting?

Bayangkan garis bilangan real sebagai jalan tol tanpa lubang. Pada bilangan rasional,
ada banyak "celah" — misalnya tidak ada bilangan rasional yang tepat sama dengan

  2. Konsep kelengkapan menjamin bahwa tidak ada celah pada garis bilangan real:

setiap himpunan yang terbatas di atas pasti memiliki batas atas terkecil, dan setiap
himpunan yang terbatas di bawah pasti memiliki batas bawah terbesar.

Definisi Supremum dan Infimum

Sebelum masuk ke definisi, ingat dulu istilah dasarnya:

  • Batas atas (upper bound) himpunan S: bilangan u sehingga x ≤ u untuk semua
    x ∈ S.

  • Batas bawah (lower bound) himpunan S: bilangan l sehingga l ≤ x untuk semua
    x ∈ S.

Definisi Supremum (batas atas terkecil): Supremum himpunan S, ditulis sup S, adalah
bilangan terkecil di antara semua batas atas S. Jadi s = sup S jika:

  1. s adalah batas atas: x ≤ s untuk semua x ∈ S.
 2. s adalah yang terkecil: untuk setiap batas atas u, berlaku s ≤ u.
Definisi Infimum (batas bawah terbesar): Infimum himpunan S, ditulis inf S, adalah
bilangan terbesar di antara semua batas bawah S. Jadi i = inf S jika:
  1. i adalah batas bawah: i ≤ x untuk semua x ∈ S.
 2. i adalah yang terbesar: untuk setiap batas bawah l, berlaku l ≤ i.

Supremum/Infimum vs Maksimum/Minimum

Ini titik yang sering membingungkan. Perhatikan perbedaannya:

                                                                               28
Konsep        Apakah harus anggota                   Catatan
              himpunan?

Maksimum Ya, harus x ∈ S                             Nilai tertinggi yang benar-benar ada di
                                                     dalam himpunan
Supremum Tidak harus
                                                     Batas atas terkecil, boleh di luar himpunan

Minimum       Ya, harus x ∈ S                        Nilai terendah yang benar-benar ada di
                                                     dalam himpunan

Infimum       Tidak harus                            Batas bawah terbesar, boleh di luar
                                                     himpunan

Kunci praktisnya: jika maksimum ada, maka maksimum = supremum. Namun
supremum bisa ada walaupun maksimum tidak ada. Begitu pula sebaliknya untuk
minimum dan infimum.

Contoh Klasik: Himpunan A = {x ∣ 0 < x < 1}

Mari analisis himpunan ini dengan teliti:

• Batas atas dari A antara lain 1, 5, 100, dst. Yang terkecil adalah 1. Maka sup A = 1.

• Batas bawah dari A antara lain 0, −3, −10, dst. Yang terbesar adalah 0. Maka
 inf A = 0.

• Apakah maksimum ada? Tidak! Karena 1 ∈/ A (intervalnya terbuka). Berapa pun x

yang    kita  pilih  mendekati  1,  selalu  ada  bilangan  lebih  besar  lagi,  misalnya  x+1  ,  yang
                                                                                            2

masih di dalam A.

• Apakah minimum ada? Tidak! 0 ∈/ A, sehingga tidak ada nilai terkecil.

Jadi untuk A: sup A = 1 dan inf A = 0, tetapi maksimum maupun minimumnya tidak

ada. Inilah ilustrasi sempurna bahwa supremum/infimum lebih umum daripada
maksimum/minimum.

Sebagai bandingan, jika himpunan B = {x ∣ 0 ≤ x ≤ 1} (interval tertutup), maka
sup B = 1 dan max B = 1; inf B = 0 dan min B = 0.

                                                 29
Sifat Kelengkapan Bilangan Real

Aksioma kelengkapan menyatakan:
                                                                Secara simetris, setiap himpunan tak kosong

yang terbatas di bawah memiliki infimum di .

Sifat ini tidak berlaku pada bilangan rasional. Ambil contoh S = {q ∈ ∣ q2 < 2}.
Himpunan ini terbatas di atas (misalnya oleh 2), tetapi tidak memiliki supremum di .
Supremumnya adalah 2, yang irrasional — sebuah "celah" pada . Karena = ∪
I, celah ini tertutup, dan garis bilangan real menjadi lengkap dan kontinu.

Implikasi Ketiadaan "Celah"

Ketiadaan celah pada punya konsekuensi besar:
  • Kontinuitas garis bilangan: tidak ada lompatan atau lubang, sehingga konsep limit
    dan kekonvergenan berjalan mulus.
  • Teorema barisan konvergen: barisan yang terbatas dan monoton selalu punya
    limit di .
  • Fondasi kalkulus: semua teorema nilai antara, teorema titik ekstrem, dan
    kekontinuan fungsi bergantung pada sifat kelengkapan.

Penerapan dalam Komputasi dan Algoritma

Sifat kelengkapan bukan sekadar teori — ia hadir di balik layar komputasi numerik:
  • Metode numerik seperti pencarian biner (binary search): setiap iterasi
    menyempitkan interval di sekitar nilai target, dan kelengkapan menjamin target
    "terkurung" dengan pasti.

  • Analisis galat (error tolerance): pertidaksamaan seperti ∣x − 3∣ < 5 menunjukkan

    pentingnya batas toleransi. Supremum galat memberi tahu seberapa jauh galat
    bisa mencapai, meski tak pernah melewati batas.

  • Constraint sistem: validasi input nilai 0 ≤ nilai ≤ 100 dapat dibaca sebagai
    himpunan dengan inf 0 dan sup 100 (dan karena tertutup, keduanya juga

    minimum dan maksimum).
  • Konvergensi algoritma iteratif: banyak algoritma optimasi berhenti ketika "galat

    cukup kecil", yang secara formal berarti mendekati infimum galat.

Rangkuman Cepat

  • Supremum = batas atas terkecil; infimum = batas bawah terbesar.

                                                                               30
  • Supremum/infimum boleh tidak menjadi anggota himpunan; maksimum/minimum
    harus anggota.

  • Untuk A = {x ∣ 0 < x < 1}: sup A = 1, inf A = 0, tanpa maksimum dan minimum.

  • Sifat kelengkapan menjamin tidak ada celah di , menjadikannya fondasi analisis
    dan komputasi numerik.

Dengan memahami supremum dan infimum, fondasi berpikir analitis Anda semakin
kokoh. Teruslah berlatih, karena konsep ini adalah pintu gerbang menuju kalkulus dan
analisis numerik yang lebih dalam!

                                                                               31
Latihan HOTS dan Rangkuman Reflektif

Mengasah Logika: Latihan HOTS dan Rangkuman Reflektif

Halo, para pejuang matematika! Sampai di sini berarti kalian sudah melewati
perjalanan panjang menjelajahi dunia bilangan. Bab ini bukan sekadar penutup,
melainkan ajang pemanasan otot berpikir tingkat tinggi alias

       (HOTS). Di sini kita akan menguji pemahaman, bukan dengan hafalan, melainkan
dengan menerapkan konsep pada situasi nyata. Siap? Mari kita mulai!

Klasifikasi Bilangan Kompleks: Menguji Ketajaman Mata

Ini adalah latihan klasik untuk memastikan kalian tidak tertukar antara jenis bilangan

yang satu dengan yang lain. Coba tentukan anggota dari himpunan bilangan yang

tepat untuk deretan berikut:     16,        5,  0,666...,  π  ,  −7,  dan  0.
                                                           2

Mari kita bedah satu per satu dengan teliti, karena di sinilah jebakan sering muncul.

• 16: Meskipun bentuknya akar, hasil perhitungannya adalah 4. Karena 4 adalah

  bilangan bulat, maka ia termasuk bilangan rasional ( ) dan juga bilangan bulat
  ( ), serta bilangan asli ( ).

• 5: Ini adalah bilangan irasional ( ) karena nilainya tidak dapat dinyatakan

   sebagai    pecahan      a  dengan  a, b  bilangan      bulat.  Desimalnya   tidak  berulang  dan
                           b

   tidak berhenti.

•  0,666...:  Angka  ini,  yang  sama   dengan      2  ,  adalah  bilangan     rasional.  Pola
                                                    3

   desimalnya berulang teratur.

•  π  :  Karena  π  adalah    bilangan  irasional,  maka         pembagiannya  dengan     2  tetap
   2

   menghasilkan bilangan irasional.

• −7: Ini jelas bilangan bulat negatif, dan karenanya juga rasional.

• 0: Ini adalah bilangan bulat (netral) dan rasional. Perlu diingat, 0 bukan bilangan

  asli, melainkan bilangan cacah.

Poin Kunci: Jangan terkecoh oleh bentuk akar. Akar yang menghasilkan bilangan bulat

(seperti 16) adalah rasional, sedangkan akar yang tidak sempurna (seperti 5)

adalah irasional.

                                                    32
Bukti Kontradiksi: Keindahan Logika Irrasionalitas 2

Untuk membuktikan bahwa 2 itu irasional, kita tidak bisa hanya mengandalkan

kalkulator. Kita perlu logika. Metode yang digunakan adalah pembuktian dengan

kontradiksi (                           ).

Langkah-langkahnya adalah sebagai berikut:

1. Asumsikan sebaliknya: Andaikan 2 adalah bilangan rasional. Maka, ia dapat

ditulis  sebagai  a  ,  di  mana  a  dan   b  adalah    bilangan  bulat,  b  =  0,  dan  pecahan
                  b

tersebut sudah dalam bentuk paling sederhana (FPB dari a dan b adalah 1).

2. Manipulasi Aljabar: Dari       2  =  a  ,  kita  kuadratkan  kedua  sisi  menjadi      2  =  a2  ,
                                        b                                                       b2

sehingga a2 = 2b2.

3. Analisis Paritas (Ganjil-Genap): Karena a2 = 2b2, maka a2 adalah bilangan genap.
  Jika a2 genap, maka a juga harus genap. Misalkan a = 2k untuk suatu bilangan
  bulat k.

4. Substitusi: Gantikan a ke persamaan awal: (2k)2 = 2b2 ⇒ 4k2 = 2b2 ⇒ 2k2 = b2.
  Ini berarti b2 juga genap, sehingga b juga genap.

5. Temukan Kontradiksi: Kita telah menyimpulkan bahwa a dan b keduanya genap. Ini

berarti FPB dari a dan b minimal adalah 2, bukan 1. Ini bertentangan dengan asumsi

awal  kita  bahwa       a  sudah  paling   sederhana.
                        b

6. Kesimpulan: Karena asumsi kita salah, maka 2 bukan bilangan rasional. Ia

   adalah bilangan irasional.

Menerapkan Pertidaksamaan dalam Konteks Nyata

Kemampuan menyelesaikan pertidaksamaan sangat berguna, misalnya dalam kasus
sistem database. Bayangkan sebuah server memiliki batas kapasitas penyimpanan.
Jika kapasitas yang tersisa harus selalu lebih dari jumlah data yang akan masuk, kita

bisa memodelkannya dalam pertidaksamaan. Misal, sisa kapasitas S dan data baru d,
maka kita perlu S − d > 0. Jika data bertambah setiap detik, kita bisa menyusun
model seperti 100 − 5t > 40, yang berarti server harus berhenti menerima data
setelah t = 12 detik. Inilah esensi HOTS: mengubah cerita menjadi model matematika,

lalu menyelesaikannya.

                                                    33
Menaklukkan Nilai Mutlak: ∣x − 3∣ < 5

Pertidaksamaan nilai mutlak sering dianggap menakutkan, padahal konsepnya sangat

visual. ∣x − 3∣ < 5 berarti "jarak antara x dan 3 adalah kurang dari 5". Ini adalah

interpretasi geometris yang sangat kuat.
Untuk menyelesaikannya secara aljabar, kita pecah menjadi pertidaksamaan ganda:

                                            −5 < x − 3 < 5

Kemudian, kita tambahkan 3 ke semua ruas:

                                          −5 + 3 < x < 5 + 3

                                               −2 < x < 8

Interpretasi: Himpunan penyelesaiannya adalah semua bilangan real x yang terletak
di antara −2 dan 8. Jika digambarkan pada garis bilangan, kita membuat bulatan
kosong di −2 dan 8, lalu menarik garis tebal di antaranya. Ini menunjukkan bahwa x

bisa berupa desimal, pecahan, atau irasional, selama nilainya berada di rentang
tersebut.

Refleksi: Mengapa Ini Semua Penting?

Mari kita berhenti sejenak dan merenung. Apa perbedaan esensial antara bilangan
rasional dan irasional? Bilangan rasional adalah bilangan yang "rapi" — dapat
dinyatakan sebagai pecahan dari dua bilangan bulat. Sebaliknya, bilangan irasional
"liar" — tidak bisa dinyatakan sebagai pecahan sederhana, desimalnya tidak pernah
berhenti dan tidak berulang.
Lalu, apa peran bilangan real ( ) dalam Sistem Informasi? Sistem informasi mengolah

data. Data yang berupa suhu ruangan server (25,4∘C), waktu respons query (0,05
detik), atau ID pengguna (1024) semuanya adalah bilangan real. Konsep bilangan real

memastikan bahwa setiap pengukuran dan perhitungan dalam sistem dapat
direpresentasikan dan dioperasikan secara konsisten, baik itu data yang presisi

                                                                               34
(rasional) maupun hasil algoritma kompleks (seringkali melibatkan irasional seperti π
atau e).

Peta Konsep: Navigasi Dunia Bilangan

Untuk merangkum semuanya, mari kita lihat peta konsep himpunan bilangan. Ini
adalah kompas yang akan memandu kalian.

• Bilangan Asli ( ): {1, 2, 3, ...}

• Bilangan Cacah: {0, 1, 2, 3, ...}

• Bilangan Bulat ( ): {..., −2, −1, 0, 1, 2, ...}

• Bilangan Rasional (  ):  Semua     bilangan  yang  dapat  ditulis  sebagai  a  dengan
                                                                              b

a, b ∈ dan b = 0.

• Bilangan Irasional ( ): Bilangan yang tidak dapat ditulis sebagai pecahan, seperti

    2, π, e.

• Bilangan Real ( ): Gabungan dari semua bilangan rasional dan irasional.

Hubungan hierarkisnya adalah:

                                     ⊂⊂ ⊂

dan himpunan irasional juga merupakan bagian dari real:

                                     ⊂

Artinya, setiap bilangan asli adalah bilangan bulat, setiap bilangan bulat adalah
rasional, dan setiap bilangan rasional maupun irasional adalah bilangan real. Namun,
tidak semua bilangan real adalah rasional, dan tidak semua bilangan rasional adalah
bulat.

Selamat! Kalian telah menyelesaikan bab ini. Teruslah berlatih, karena kemampuan
berpikir tingkat tinggi adalah otot yang perlu terus dilatih. Sampai jumpa di
petualangan matematika berikutnya!

                                     35
