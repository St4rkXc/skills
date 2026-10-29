---
mode: detailed
pages: 34
words: 7208
---

pelajarin.ai

Prinsip Inklusi-Eksklusi

Prinsip Inklusi-Eksklusi: Menghitung Gabungan Himpunan dengan
Cermat

Halo! Selamat datang di bab yang sangat berguna ini. Pernahkah kamu diminta
menghitung "berapa banyak bilangan yang habis dibagi 3 atau 5" dalam suatu
rentang? Kalau kamu hanya menjumlahkan banyaknya bilangan kelipatan 3 dengan
kelipatan 5, jawabanmu akan salah karena bilangan kelipatan 15 terhitung dua kali. Di
sinilah Prinsip Inklusi-Eksklusi menyelamatkan kita. Prinsip ini adalah alat fundamental
dalam teori himpunan yang memungkinkan kita menghitung kardinalitas gabungan
beberapa himpunan secara akurat, dengan memperhitungkan tumpang tindih (irisan)
di antara mereka.

Konsep Dasar
Bayangkan dua himpunan, A dan B. Kalau kita ingin tahu berapa banyak anggota
gabungannya (A ∪ B), kita tidak bisa sekadar menjumlahkan ∣A∣ + ∣B∣. Kenapa?
Karena anggota yang berada di kedua himpunan (yakni di A ∩ B) akan dihitung dua

kali. Maka, kita perlu mengurangi bagian yang tumpang tindih itu sekali agar setiap
anggota dihitung tepat satu kali.

Logika inilah yang menjadi inti prinsip inklusi-eksklusi:

  • Inklusi (memasukkan): jumlahkan kardinalitas semua himpunan.

  • Eksklusi (mengeluarkan): kurangi kardinalitas irisan agar tidak terjadi penghitungan
    ganda.

Rumus untuk Dua dan Tiga Himpunan

Dua himpunan:

                ∣A ∪ B∣ = ∣A∣ + ∣B∣ − ∣A ∩ B∣

Tiga himpunan:

                1
     ∣A ∪ B ∪ C∣ = ∣A∣ + ∣B∣ + ∣C∣ − ∣A ∩ B∣ − ∣A ∩ C∣ − ∣B ∩ C∣ + ∣A ∩ B ∩ C∣

Perhatikan polanya: kita tambah semua himpunan tunggal, kurangi semua irisan
pasangan, lalu tambah kembali irisan ketiganya. Mengapa ditambah kembali? Karena
saat mengurangkan ketiga irisan pasangan, anggota yang berada di ketiga himpunan

sekaligus (A ∩ B ∩ C) ikut terbuang tiga kali, padahal sebelumnya hanya dihitung

tiga kali. Agar kembali seimbang (dihitung tepat sekali), kita harus menambahkannya
satu kali lagi.

Bilangan yang Tidak Habis Dibagi Dua Bilangan

Ini penerapan paling populer. Misalnya kita ingin menghitung banyaknya bilangan
bulat dari 1 sampai 100 yang tidak habis dibagi 3 dan tidak habis dibagi 5.
Triknya: hitung dulu banyaknya bilangan yang habis dibagi 3 atau 5, lalu kurangkan
dari total.

  • Banyak kelipatan 3: ⌊100/3⌋ = 33
  • Banyak kelipatan 5: ⌊100/5⌋ = 20
  • Banyak kelipatan 3 dan 5 (yaitu kelipatan 15): ⌊100/15⌋ = 6
Maka bilangan yang habis dibagi 3 atau 5 adalah 33 + 20 − 6 = 47.
Bilangan yang tidak habis dibagi keduanya: 100 − 47 = 53.

Poin penting: saat mengerjakan soal "tidak habis dibagi", jangan lupa langkah terakhir
mengurangi dari total. Kesalahan paling umum adalah berhenti di angka 47.

Penerapan pada Rentang Bilangan Tertentu (101–600)

Untuk rentang yang tidak dimulai dari 1, kita gunakan prinsip yang sama tetapi hitung
kelipatan di dalam rentang itu saja. Misal kita ingin tahu berapa bilangan antara 101
sampai 600 yang habis dibagi 4 atau 7.

  • Kelipatan 4 dari 101–600: nilai terkecil ≥ 101 adalah 104, terbesar ≤ 600 adalah 600.
    Banyaknya: ⌊600/4⌋ − ⌊100/4⌋ = 150 − 25 = 125.

  • Kelipatan 7 dari 101–600: ⌊600/7⌋ − ⌊100/7⌋ = 85 − 14 = 71.
  • Kelipatan 4 dan 7 (kelipatan 28): ⌊600/28⌋ − ⌊100/28⌋ = 21 − 3 = 18.
Jadi, ∣A ∪ B∣ = 125 + 71 − 18 = 178 bilangan.

                                                                                2
Kunci rentang: untuk rentang (a, b], banyak kelipatan k adalah ⌊b/k⌋ − ⌊a/k⌋. Rumus

ini otomatis membuang kelipatan yang berada di bawah batas bawah.

Soal Latihan

Latihan 1 — Pembagian dengan Kelipatan
Berapa banyak bilangan bulat dari 1 sampai 200 yang habis dibagi 6 atau 8?
Penyelesaian:

  • Kelipatan 6: ⌊200/6⌋ = 33
  • Kelipatan 8: ⌊200/8⌋ = 25
  • Kelipatan 6 dan 8 = kelipatan KPK(6,8) = 24: ⌊200/24⌋ = 8
Hasil: 33 + 25 − 8 = 50 bilangan.

Latihan 2 — Tiga Himpunan pada Survei Mahasiswa
Sebuah survei terhadap 100 mahasiswa menanyakan platform belajar favorit mereka:
Video, Buku, dan Kelas Online. Diketahui:

  • 50 suka Video, 40 suka Buku, 35 suka Kelas Online
  • 20 suka Video & Buku, 15 suka Video & Kelas Online, 12 suka Buku & Kelas Online
  • 5 suka ketiganya
Berapa mahasiswa yang menyukai setidaknya satu platform? Menggunakan rumus
tiga himpunan:

                    ∣V ∪ B ∪ K∣ = 50 + 40 + 35 − 20 − 15 − 12 + 5 = 83

Jadi, 83 mahasiswa menyukai setidaknya satu platform, dan 100 − 83 = 17

mahasiswa tidak menyukai satupun.
Latihan 3 — Rentang dan Komplemen
Berapa banyak bilangan antara 1 sampai 500 yang tidak habis dibagi 3 maupun 5?

  • Kelipatan 3: ⌊500/3⌋ = 166
  • Kelipatan 5: ⌊500/5⌋ = 100
  • Kelipatan 15: ⌊500/15⌋ = 33

                                                                                3
Habis dibagi 3 atau 5: 166 + 100 − 33 = 233. Maka yang tidak habis dibagi keduanya:
500 − 233 = 267.
Rangkuman Tips

  • Selalu identifikasi KPK dari bilangan pembagi untuk mencari irisan. Kelipatan

    bersama dari a dan b adalah kelipatan KPK(a, b).

  • Inklusi-eksklusi bergantian tanda: tambah, kurang, tambah, kurang — untuk
    jumlah himpunan ganjil dan genap.

  • Untuk "tidak habis dibagi", hitung dulu gabungannya lalu ambil komplemen dari
    total.

  • Untuk rentang bukan 1, gunakan pengurangan ⌊b/k⌋ − ⌊a/k⌋.

Prinsip inklusi-eksklusi mungkin terlihat sepele, tetapi fondasinya kuat dan skalanya
luas. Seperti yang tercermin dalam capaian pembelajaran mata kuliah ini —
kemampuan memahami prinsip-prinsip matematika yang dapat diterapkan dalam
lingkup ilmu sistem informasi — keterampilan ini akan terus kamu pakai dalam analisis
basis data, peluang, teori himpunan lanjutan, hingga penghitungan kompleksitas
algoritma. Latihlah dengan soal-soal variasi rentang dan tiga himpunan, dan kamu
akan semakin mahir. Semangat belajar!

                                                                                4
Partisi Himpunan

Partisi Himpunan: Membagi Tanpa Sisa, Menutup Tanpa Celah

Bayangkan kamu punya sekotak permen campur. Kamu ingin memisahkan permen itu
ke dalam beberapa mangkuk berdasarkan warnanya — semua merah ke mangkuk A,
semua hijau ke mangkuk B, dan seterusnya. Setiap permen pasti masuk ke tepat satu
mangkuk, tidak ada yang tertinggal di kotak, dan tidak ada satu permen pun yang
muncul di dua mangkuk sekaligus. Nah, itulah gambaran sederhana dari partisi
himpunan. Konsep ini terlihat sepele, tapi fondasinya sangat penting — ia
menghubungkan himpunan dengan relasi ekuivalen, dua topik yang sering muncul
berdampingan dalam teori himpunan.

Mari kita bedah konsep ini secara menyeluruh, mulai dari definisinya, syarat-syaratnya,
hubungannya dengan relasi ekuivalen, hingga contoh yang benar dan contoh yang
salah.

Definisi Partisi Himpunan
Secara formal, partisi dari sebuah himpunan S adalah himpunan yang terdiri atas
sub-himpunan-sub-himpunan tak kosong dari S, katakanlah A1, A2, A3, … , An,

sedemikian rupa sehingga:

  1. Tidak ada sub-himpunan yang kosong. Setiap Ai = ∅.

 2. Sub-himpunan saling asing (disjoint) satu sama lain. Artinya, untuk setiap

    pasangan Ai dan Aj dengan i = j, berlaku Ai ∩ Aj = ∅. Tidak ada elemen yang

    dimiliki bersama oleh dua blok berbeda.

 3. Gabungan seluruh sub-himpunan sama dengan himpunan asalnya. Yaitu A1 ∪
    A2 ∪ ⋯ ∪ An = S. Tidak ada elemen dari S yang tertinggal.

Ketiga syarat ini harus terpenuhi sekaligus. Jika salah satu saja gagal, maka kumpulan
sub-himpunan tersebut bukan partisi.

Perlu dicatat bahwa sub-himpunan-sub-himpunan dalam partisi sering disebut blok
atau sel. Jumlah blok bisa berapa saja, asalkan memenuhi ketiga syarat di atas.

Bahkan himpunan S itu sendiri, jika kita anggap sebagai satu blok tunggal, merupakan

partisi yang valid (partisi trivial).

Syarat-Syarat Partisi yang Valid

Mari kita rangkum syarat-syarat ini dalam tabel agar lebih mudah diingat.

                                                                                5
No Syarat                     Rumus              Arti Sederhana

1  Blok tidak kosong          Ai = ∅            Setiap mangkuk ada
                                                 isinya
2  Blok saling asing          Ai ∩ Aj = ∅ untuk
                              i = j             Tidak ada elemen yang
3  Gabungan menutupi seluruh  ⋃ni=1 Ai = S       dobel
   himpunan
                                                 Semua elemen
                                                 terwadahi

Mengapa ketiga syarat ini penting? Syarat pertama memastikan tidak ada blok yang
sia-sia — blok kosong tidak memberi informasi apa pun. Syarat kedua menjamin
keunikan keanggotaan: setiap elemen punya "rumah" yang jelas dan hanya satu.
Syarat ketiga memastikan kelengkapan: tidak ada elemen yang tercecer di luar.

Hubungan Partisi dengan Relasi Ekuivalen

Inilah bagian yang paling elegan dari konsep partisi. Ada korespondensi satu-ke-satu
antara partisi dan relasi ekuivalen pada sebuah himpunan.

Sebuah relasi R pada himpunan S disebut relasi ekuivalen jika memenuhi tiga sifat:

  • Refleksif: setiap elemen berelasi dengan dirinya sendiri, yaitu a R a untuk semua
    a ∈ S.

  • Simetris: jika a R b, maka b R a.

  • Transitif: jika a R b dan b R c, maka a R c.

Dari sebuah relasi ekuivalen, kita bisa membentuk kelas-kelas ekuivalen. Kelas

ekuivalen dari elemen a, ditulis [a], adalah himpunan semua elemen yang berelasi
dengan a:

                                        [a] = { x ∈ S ∣ x R a }

Kunci utamanya: kumpulan semua kelas ekuivalen yang berbeda selalu membentuk

partisi dari S. Mengapa demikian?
  • Setiap kelas ekuivalen tidak kosong, karena sifat refleksif menjamin a ∈ [a].

                              6
  • Dua kelas ekuivalen yang berbeda pasti saling asing, karena jika [a] dan [b]

    beririsan, maka ada elemen yang berelasi dengan keduanya, dan dengan sifat
    transitif semua elemen di kedua kelas menjadi berelasi — artinya kelasnya sama.

  • Gabungan semua kelas sama dengan S, karena setiap elemen pasti berada di

    kelasnya sendiri.
Sebaliknya juga berlaku: setiap partisi mendefinisikan sebuah relasi ekuivalen.

Caranya, definisikan a R b jika dan hanya jika a dan b berada dalam blok yang sama.

Relasi ini otomatis memenuhi sifat refleksif, simetris, dan transitif.
Jadi, partisi dan relasi ekuivalen adalah dua sisi dari mata uang yang sama.
Memahami salah satunya berarti memahami yang lain.

Contoh dan Contoh Balasan

Contoh 1: Partisi yang Valid

Misalkan S = {1, 2, 3, 4, 5, 6}. Tinjau kumpulan himpunan berikut:

                                    P = { {1, 2}, {3, 4}, {5, 6} }

Apakah ini partisi? Mari periksa ketiga syaratnya:
  • Tidak ada blok yang kosong.

  • {1, 2} ∩ {3, 4} = ∅, {1, 2} ∩ {5, 6} = ∅, {3, 4} ∩ {5, 6} = ∅ — semua saling asing.
  • {1, 2} ∪ {3, 4} ∪ {5, 6} = {1, 2, 3, 4, 5, 6} = S.
Karena ketiga syarat terpenuhi, P adalah partisi yang valid dari S.

Contoh 2: Bukan Partisi (Ada Elemen yang Tertinggal)

Tinjau kumpulan Q = { {1, 2}, {3, 4} } pada himpunan S = {1, 2, 3, 4, 5, 6} yang

sama.

Di sini, {1, 2} ∪ {3, 4} = {1, 2, 3, 4} = S. Elemen 5 dan 6 tidak tertampung di blok
mana pun. Syarat ketiga gagal, sehingga Q bukan partisi.

Contoh 3: Bukan Partisi (Blok Saling Beririsan)

Tinjau kumpulan R = { {1, 2, 3}, {3, 4, 5}, {6} } pada S = {1, 2, 3, 4, 5, 6}.

                                                                                7
Syarat ketiga terpenuhi, karena gabungannya membentuk S. Namun, {1, 2, 3} ∩
{3, 4, 5} = {3} = ∅. Elemen 3 berada di dua blok sekaligus. Syarat kedua gagal,
sehingga R bukan partisi.

Contoh 4: Bendera Merah — Blok Kosong

Kumpulan T = { {1, 2}, {3, 4}, ∅, {5, 6} } hampir terlihat seperti partisi, tetapi

mengandung blok kosong. Ini melanggar syarat pertama, jadi bukan partisi. Sebuah
partisi tidak boleh menyertakan blok kosong.
Contoh 5: Menghubungkan dengan Relasi Ekuivalen

Pada himpunan bilangan bulat Z, definisikan relasi a R b jika dan hanya jika a − b
habis dibagi 3 (yaitu a ≡ b (mod 3)). Relasi ini adalah relasi ekuivalen, dan kelas-kelas

ekuivalennya adalah:

                                   [0] = {… , −6, −3, 0, 3, 6, … }

                                   [1] = {… , −5, −2, 1, 4, 7, … }

                                   [2] = {… , −4, −1, 2, 5, 8, … }

Ketiga kelas ini saling asing dan gabungannya sama dengan Z. Jadi, { [0], [1], [2] }
adalah partisi dari Z.
Rangkuman Cepat

  • Partisi membagi himpunan menjadi blok-blok tak kosong yang saling asing dan
    menutupi seluruh himpunan.

  • Tiga syarat wajib: tidak kosong, saling asing, dan gabungannya sama dengan
    himpunan asal.

  • Partisi berhubungan erat dengan relasi ekuivalen — kumpulan kelas ekuivalen
    selalu membentuk partisi, dan setiap partisi melahirkan relasi ekuivalen.

  • Contoh balasan yang umum: ada elemen tertinggal, ada blok beririsan, atau ada
    blok kosong.

                                                                                8
Dengan memahami partisi, kamu membuka pintu ke konsep-konsep lanjutan seperti
himpunan ganda, himpunan fuzzy, dan penghitungan dengan prinsip inklusi-eksklusi
— semuanya bertumpu pada gagasan dasar tentang bagaimana kita
mengelompokkan elemen secara rapi dan tuntas. Selamat belajar, dan jangan ragu
untuk bereksperimen dengan contoh-contohmu sendiri!

                                                                                9
Himpunan Ganda (Multiset)

Himpunan Ganda (Multiset): Ketika Elemen Boleh Muncul Berkali-
kali

Halo! Selamat datang di bab yang sangat menarik. Selama ini kita terbiasa dengan
himpunan biasa, di mana setiap elemen hanya boleh muncul satu kali. Namun, dalam
banyak situasi nyata, kita justru perlu mencatat berapa kali sebuah objek muncul. Di
sinilah konsep himpunan ganda atau multiset berperan. Mari kita pelajari bersama
dengan santai namun menyeluruh.

Apa Itu Himpunan Ganda?

Himpunan ganda (multiset) adalah kumpulan objek di mana setiap elemen
diperbolehkan muncul lebih dari satu kali. Berbeda dengan himpunan biasa yang
mengabaikan pengulangan, multiset justru mencatat setiap kemunculan.

Bayangkan sebuah kantong berisi permen. Jika kamu memasukkan tiga permen rasa

jeruk dan dua permen rasa mangga, maka kantong itu bukan sekadar himpunan {
jeruk, mangga}, melainkan multiset yang memperhatikan seberapa banyak tiap rasa

hadir.

Secara notasi, multiset sering ditulis dengan tanda kurung kurawal yang menyertakan
kemunculan berulang, misalnya:

        M = {a, a, a, b, b, c}

Di sini, elemen a muncul tiga kali, b muncul dua kali, dan c muncul satu kali.

Konsep Multiplisitas

Multiplisitas (multiplicity) adalah konsep inti dalam multiset. Multiplisitas suatu elemen
menyatakan berapa kali elemen tersebut muncul di dalam multiset.

Dari contoh M = {a, a, a, b, b, c}, kita dapat merangkumnya dalam tabel multiplisitas

berikut:

Elemen  Multiplisitas

        10
a  3

b  2

c  1

Beberapa catatan penting tentang multiplisitas:

  • Multiplisitas selalu berupa bilangan bulat tak negatif. Nilai 0 berarti elemen tersebut

    tidak hadir dalam multiset.

  • Dua multiset dianggap sama jika dan hanya jika setiap elemen memiliki
    multiplisitas yang sama pada keduanya. Jadi urutan penulisan tidak penting, tetapi
    jumlah kemunculan sangat penting.

  • Berbeda dengan himpunan biasa, multiset {a, a, b} tidak sama dengan {a, b}
    karena multiplisitas a berbeda (2 versus 1).

Kardinalitas Multiset

Kardinalitas sebuah multiset adalah jumlah total elemen dengan menghitung setiap
kemunculan secara terpisah. Inilah yang membedakannya dari kardinalitas
himpunan biasa.

Untuk multiset M = {a, a, a, b, b, c}:

   ∣M ∣ = 3 + 2 + 1 = 6

Jadi, meskipun hanya ada tiga elemen berbeda (a, b, dan c), kardinalitasnya adalah 6

karena kita menghitung semua kemunculan.
Secara umum, jika sebuah multiset memiliki elemen-elemen dengan multiplisitas

m1, m2, … , mk, maka:

                                                                                                      k

                              ∣M ∣ = m1 + m2 + ⋯ + mk = ∑ mi

                                                                                                     i=1

   11
   Ingat! Jumlah elemen berbeda (disebut juga ukuran pendukung/dukungan)
   berbeda dengan kardinalitas. Pada contoh di atas, ada 3 elemen berbeda tetapi
   kardinalitasnya 6.

Himpunan Biasa sebagai Kasus Khusus Multiset

Kabar baiknya: kamu tidak perlu membuang pengetahuan tentang himpunan biasa!
Himpunan biasa adalah kasus khusus dari multiset, yaitu multiset yang seluruh

elemennya memiliki multiplisitas 1 (atau 0 jika tidak hadir).

  • Pada himpunan biasa, setiap elemen muncul paling banyak satu kali, sehingga

    multiplisitasnya selalu 0 atau 1.

  • Akibatnya, kardinalitas himpunan biasa sama dengan jumlah elemen berbedanya.
Dengan kata lain, semua aturan himpunan biasa tetap berlaku, hanya saja multiset
memberikan kebebasan tambahan untuk mengizinkan pengulangan. Inilah mengapa
memahami multiset memperluas, bukan menggantikan, pemahaman kita tentang
himpunan.

Operasi antara Dua Buah Multiset

Karena multiset melibatkan multiplisitas, operasi antar multiset sedikit berbeda dari
operasi himpunan biasa. Berikut operasi-operasi utamanya.
1. Gabungan (Union)
Gabungan dua multiset mengambil multiplisitas maksimum dari setiap elemen:

                                  (A ∪ B)(x) = max(A(x), B(x))

Contoh: jika A = {a, a, b} dan B = {a, b, b, c}, maka A ∪ B = {a, a, b, b, c}.

2. Irisan (Intersection)
Irisan dua multiset mengambil multiplisitas minimum dari setiap elemen:

                                  (A ∩ B)(x) = min(A(x), B(x))

Contoh: A ∩ B = {a, b}.

                                                                               12
3. Selisih (Difference)
Selisih multiset mengurangkan multiplisitas, dengan hasil tidak boleh negatif:

                               (A − B)(x) = max(A(x) − B(x), 0)

Contoh: A − B = {a} (karena a tersisa 2 − 1 = 1, sedangkan b habis).

4. Jumlah Multiset (Sum)
Operasi khas multiset adalah penjumlahan, yang menjumlahkan multiplisitas:

                 (A + B)(x) = A(x) + B(x)

Contoh: A + B = {a, a, a, b, b, b, c} dengan kardinalitas 3 + 3 + 1 = 7.

Mari kita rangkum dalam tabel agar mudah diingat:

Operasi     Aturan Multiplisitas      Contoh (A = {a, a, b}, B = {a, b, b, c})

Gabungan ∪  max                       {a, a, b, b, c}

Irisan ∩    min                       {a, b}

Selisih −   max(A − B, 0)             {a}

Jumlah +    A+B                       {a, a, a, b, b, b, c}

Mengapa Multiset Penting?

Konsep multiset sangat berguna dalam kehidupan nyata maupun matematika diskrit.
Beberapa penerapannya:

  • Menghitung frekuensi suatu data, seperti nilai mahasiswa atau hasil survei.

  • Kombinatorika dengan pengulangan, misalnya menghitung cara memilih objek
    yang boleh sama.

  • Basis data dan pemrograman, di mana kita sering mencatat berapa kali suatu nilai
    muncul (misalnya dalam struktur multiset atau bag).

                                  13
  • Statistika, untuk merepresentasikan data yang memiliki nilai berulang.
Sebagai gambaran nyata: dalam sebuah survei terhadap mahasiswa, kita bisa saja
mencatat bahwa banyak mahasiswa memilih lebih dari satu mata kuliah, sehingga
data pilihannya membentuk pola mirip multiset — objek (mata kuliah) boleh "muncul"
pada banyak responden.

Rangkuman Bab

Mari kita ikat semua konsep yang telah kita pelajari:
  • Himpunan ganda (multiset) memperbolehkan elemen muncul lebih dari sekali.
  • Multiplisitas menyatakan berapa kali sebuah elemen muncul (bilangan bulat tak
    negatif).
  • Kardinalitas multiset adalah jumlah total semua kemunculan, bukan jumlah
    elemen berbeda.
  • Himpunan biasa adalah kasus khusus multiset dengan multiplisitas maksimum
    satu.

  • Operasi multiset meliputi gabungan (max), irisan (min), selisih (max(A − B, 0)),

    dan penjumlahan (jumlahkan multiplisitas).
Dengan memahami multiset, kamu kini memiliki alat yang lebih fleksibel untuk
memodelkan dunia nyata yang penuh pengulangan. Teruslah berlatih dengan contoh-
contoh kecil — semakin sering kamu menghitung multiplisitas dan kardinalitas,
semakin alami konsep ini terasa. Kamu pasti bisa!

                                                                               14
Pembuktian Proposisi Himpunan dengan Diagram Venn

Pengantar: Diagram Venn sebagai Alat Bantu Berpikir

Hai, selamat datang di bab yang menarik ini! Kita akan membahas bagaimana
diagram Venn digunakan dalam konteks proposisi himpunan — khususnya sebagai
alat ilustrasi — serta mengapa ia tidak bisa begitu saja dianggap sebagai pembuktian
formal. Ini penting banget, karena banyak mahasiswa terjebak menganggap gambar
diagram Venn sudah cukup untuk "membuktikan" sesuatu. Padahal, ada nuansa halus
yang perlu kita pahami bersama.

Mari kita mulai dari peran dasarnya.

Penggunaan Diagram Venn untuk Pembuktian

Diagram Venn adalah representasi visual dari himpunan-himpunan yang
digambarkan sebagai lingkaran (atau bentuk tertutup lainnya) di dalam sebuah
persegi yang melambangkan semesta pembicaraan. Dalam praktiknya, diagram Venn
sangat sering dipakai untuk:

  • Mengilustrasikan operasi himpunan, seperti gabungan (A ∪ B), irisan (A ∩ B),
    selisih (A − B), dan komplemen (Ac).

  • Membantu memverifikasi dugaan tentang kesamaan dua ekspresi himpunan.

    Misalnya, kita menduga bahwa A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C). Dengan

    menggambar daerah yang sesuai, kita bisa "melihat" apakah kedua sisi
    menghasilkan daerah yang sama.

  • Menjelaskan konsep kepada audiens secara cepat dan intuitif, terutama dalam
    pengajaran atau presentasi.

  • Memeriksa kasus-kasus khusus, misalnya ketika dua himpunan saling lepas
    (disjoint), salah satu himpunan termuat di himpunan lain, atau ketika keduanya
    saling beririsan sebagian.

Sebagai contoh sederhana, perhatikan pertanyaan: berapa mahasiswa yang

mengambil setidaknya satu dari dua mata kuliah? Jika kita misalkan A adalah
himpunan mahasiswa yang mengambil MK pertama dan B himpunan mahasiswa
yang mengambil MK kedua, maka yang dicari adalah ∣A ∪ B∣. Diagram Venn dengan
dua lingkaran yang beririsan langsung memberi gambaran bahwa daerah A ∪ B
mencakup tiga bagian: hanya A, hanya B, dan irisan A ∩ B. Dari situ kita ingat rumus

inklusi-eksklusi:

                                                                               15
                                   ∣A ∪ B∣ = ∣A∣ + ∣B∣ − ∣A ∩ B∣

Diagram Venn di sini berperan sebagai peta mental yang memudahkan kita
mengingat mengapa irisan harus dikurangkan (karena dihitung dua kali jika kita hanya

menjumlahkan ∣A∣ + ∣B∣).

Keterbatasan Jumlah Himpunan yang Dapat Digambarkan

Nah, ini poin penting yang sering terlewat. Diagram Venn sangat efektif untuk dua atau
tiga himpunan. Untuk dua himpunan, kita cukup menggambar dua lingkaran yang
saling beririsan. Untuk tiga himpunan, kita menggambar tiga lingkaran yang saling
beririsan sedemikian rupa sehingga terbentuk delapan daerah (termasuk daerah di
luar ketiganya).
Namun, begitu kita berurusan dengan empat himpunan atau lebih, keterbatasan
mulai muncul:

  • Secara visual, menggambarkan empat himpunan yang saling beririsan dengan
    semua kemungkinan kombinasi irisan tetap terlihat menjadi sangat rumit.
    Lingkaran-lingkaran tidak lagi cukup; kita perlu bentuk elips atau kurva yang aneh.

  • Untuk empat himpunan, masih mungkin dibuat diagram yang benar (misalnya
    dengan elips), tetapi sudah sulit dibaca.

  • Untuk lima himpunan atau lebih, representasi visual yang bersih dan mudah
    dipahami hampir tidak mungkin dilakukan tanpa mengorbankan kejelasan.

  • Akibatnya, daya generalisasi diagram Venn terbatas. Kita tidak bisa
    mengandalkan gambar untuk membuktikan proposisi yang melibatkan banyak
    himpunan sekaligus.

Inilah salah satu alasan mengapa diagram Venn lebih cocok sebagai alat bantu awal
daripada sebagai metode pembuktian umum.

Sifat Ilustratif versus Pembuktian Formal

Sekarang kita masuk ke inti bab ini. Ada perbedaan mendasar antara ilustrasi dan
pembuktian formal.

  • Ilustrasi bertujuan memberi gambaran, membantu intuisi, dan mempermudah
    komunikasi ide. Diagram Venn termasuk di sini.

                                                                               16
  • Pembuktian formal menuntut langkah-langkah logis yang berlaku untuk semua
    kemungkinan, tanpa bergantung pada satu gambar tertentu. Pembuktian
    biasanya dilakukan dengan:
       ◦ Definisi keanggotaan: menunjukkan bahwa setiap elemen di sisi kiri juga ada di
         sisi kanan, dan sebaliknya.
       ◦ Hukum-hukum aljabar himpunan: seperti hukum distributif, hukum De Morgan,
         hukum identitas, dan sebagainya.
       ◦ Tabel keanggotaan (membership table), yang secara sistematis memeriksa
         semua kombinasi keanggotaan elemen pada tiap himpunan.

Mengapa diagram Venn tidak cukup sebagai pembuktian formal? Karena:
  1. Diagram hanya mewakili satu konfigurasi tertentu. Kita bisa saja menggambar
    dua himpunan yang beririsan, tetapi bagaimana jika kenyataannya salah satu
    himpunan kosong? Atau salah satu termuat di himpunan lain? Diagram tidak
    otomatis menangkap semua kasus ini.
 2. Kesalahan gambar bisa menyesatkan. Jika kita tidak hati-hati menggambar irisan,
    kita bisa "membuktikan" sesuatu yang sebenarnya salah.
 3. Tidak ada langkah deduktif eksplisit. Pembaca tidak bisa melacak alur logika
    langkah demi langkah seperti pada pembuktian berbasis definisi.

Sebagai ilustrasi, anggaplah kita ingin membuktikan A − (B ∪ C) = (A − B) ∩ (A −
C). Diagram Venn dengan tiga lingkaran bisa membantu kita melihat bahwa kedua

sisi menghasilkan daerah yang sama. Tetapi pembuktian yang sahih tetap harus
ditulis, misalnya:

   Ambil sembarang x. x ∈ A − (B ∪ C) jika dan hanya jika x ∈ A dan x ∈/ B ∪ C,
   yang berarti x ∈ A dan x ∈/ B dan x ∈/ C. Ini setara dengan x ∈ A − B dan x ∈
   A − C, yaitu x ∈ (A − B) ∩ (A − C).

Barulah ini disebut pembuktian formal.

Status Diagram Venn dalam Pembuktian Matematis

Lalu, apa sebenarnya status diagram Venn dalam praktik matematika?
  • Sebagai alat heuristik: diagram Venn sangat berharga untuk menemukan dugaan,
    merancang strategi pembuktian, dan memahami struktur masalah.

                                                                               17
  • Sebagai alat komunikasi: dalam makalah, presentasi, atau buku teks, diagram
    Venn sering disertakan untuk memperjelas konsep.

  • Bukan sebagai pembuktian yang berdiri sendiri: dalam standar matematika
    formal, diagram Venn tidak dianggap sebagai bukti yang lengkap. Ia biasanya
    hanya menjadi pelengkap dari pembuktian verbal atau simbolik.

  • Pengecualian terbatas: dalam konteks yang sangat terbatas, misalnya untuk
    menunjukkan bahwa suatu identitas himpunan tidak berlaku (counterexample),
    diagram Venn bisa sangat membantu — tetapi tetap harus disertai penjelasan
    verbal yang eksplisit.

Jadi, kesimpulannya: gunakanlah diagram Venn sebagai sahabat setia dalam
memahami himpunan, tetapi jangan pernah mengandalkannya sebagai satu-
satunya senjata pembuktian. Kombinasikan dengan definisi, hukum aljabar himpunan,
dan penalaran logis yang ketat.
Dengan memahami peran dan batasannya, kamu akan lebih siap menulis pembuktian
proposisi himpunan yang benar-benar meyakinkan. Selamat belajar, dan jangan ragu
untuk berlatih menggambar diagram Venn sekaligus menulis pembuktian formalnya!

                                                                               18
Pembuktian Proposisi Himpunan dengan Tabel
Keanggotaan

Pendahuluan: Mengapa Perlu Membuktikan Proposisi Himpunan?

Halo! Sebelumnya kita sudah belajar bahwa himpunan adalah contoh khusus dari

multiset, di mana semua elemennya dianggap berbeda. Sebagai contoh, jika A =
{1, 1, 1, 2, 2, 3}, maka kardinalitas multiset tersebut adalah ∣A∣ = 6 karena kita

menghitung setiap kemunculan elemen. Dalam himpunan biasa, elemen yang sama
hanya ditulis sekali, sehingga himpunan selalu memiliki multiplisitas 0 atau 1 untuk
setiap elemennya, sedangkan multiset bisa memiliki multiplisitas lebih besar, seperti
multiplisitas 0 sebanyak 4 pada contoh tertentu.

Nah, ketika kita bekerja dengan himpunan, sering kali kita menemukan proposisi
himpunan — yaitu pernyataan yang mengklaim dua ekspresi himpunan itu sama, atau
satu himpunan merupakan bagian dari himpunan lain. Bagaimana cara membuktikan
kebenarannya? Salah satu metode yang paling sistematis dan mudah dipahami
adalah tabel keanggotaan.

Apa Itu Tabel Keanggotaan?

Tabel keanggotaan (membership table) adalah sebuah tabel yang mendaftar semua
kemungkinan kombinasi nilai keanggotaan setiap elemen terhadap himpunan-
himpunan yang terlibat dalam proposisi. Karena sebuah elemen bisa berada di dalam
atau di luar suatu himpunan, setiap himpunan direpresentasikan oleh nilai 1 (berada di
dalam himpunan) atau 0 (tidak berada di dalam himpunan).

Inti idenya sederhana: jika dua ekspresi himpunan menghasilkan kolom nilai
keanggotaan yang identik untuk semua kemungkinan kombinasi, maka kedua ekspresi
tersebut terbukti sama. Sebaliknya, jika ada satu baris saja yang berbeda, proposisi itu
gugur.

Langkah Penyusunan Tabel Keanggotaan

Berikut langkah-langkah yang bisa kamu ikuti, sahabat pembelajar:

  1. Identifikasi himpunan yang terlibat. Misalnya proposisi memuat himpunan A, B,
    dan C. Catat semua simbol yang muncul, lalu hitung banyaknya, sebut saja n.

 2. Tentukan jumlah baris tabel. Karena setiap himpunan punya dua kemungkinan

    nilai (0 atau 1), jumlah baris adalah 2n. Untuk dua himpunan, ada 22 = 4 baris;
    untuk tiga himpunan, 23 = 8 baris.

                                                                               19
 3. Buat kolom untuk setiap himpunan dasar. Kolom-kolom ini berisi semua kombinasi
    nilai 0 dan 1 yang mungkin. Urutkan secara sistematis agar tidak ada kombinasi
    yang terlewat.

 4. Tambahkan kolom untuk setiap sub-ekspresi. Jika proposisinya A ∪ (B ∩ C), buat
    kolom antara seperti B ∩ C, lalu kolom hasil akhir A ∪ (B ∩ C).

 5. Isi setiap kolom berdasarkan operasi himpunan. Gunakan aturan operasi: irisan

    (∩) bernilai 1 hanya jika semua komponen 1; gabungan (∪) bernilai 1 jika salah satu
    komponen 1; komplemen (A) membalik nilai.

 6. Bandingkan kolom hasil akhir. Jika kedua sisi proposisi memiliki pola yang sama
    persis, proposisi terbukti benar.

Contoh Penerapan
Mari buktikan proposisi A ∩ B ⊆ A. Kita buat tabel keanggotaan dengan dua

himpunan:

A        B        A∩B         Apakah (A ∩ B) ⇒ A?

0        0        0           benar (0 → 0)

0        1        0           benar (0 → 0)

1        0        0           benar (0 → 1)

1        1        1           benar (1 → 1)

Karena di setiap baris, nilai A ∩ B tidak pernah bernilai 1 sementara A bernilai 0, maka
A ∩ B selalu merupakan bagian dari A. Proposisi terbukti.
Sekarang, contoh yang lebih menantang: buktikan A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C).

Dengan tiga himpunan, kita butuh 8 baris:

  A B C B ∩ C A ∪ (B ∩ C) A ∪ B A ∪ C (A ∪ B) ∩ (A ∪ C)

0  0  0     0  0           0  0              0

0  0  1     0  0           0  1              0

                       20
0  1    0          0  0                 1          0   0

0  1    1          1  1                 1          1   1

1  0    0          0  1                 1          1   1

1  0    1          0  1                 1          1   1

1  1    0          0  1                 1          1   1

1  1    1          1  1                 1          1   1

Perhatikan kolom A ∪ (B ∩ C) dan kolom (A ∪ B) ∩ (A ∪ C). Keduanya identik baris

demi baris. Inilah yang membuktikan hukum distributif untuk himpunan.

Analisis Hasil Tabel untuk Pembuktian

Setelah tabel selesai, lakukan analisis berikut:
  • Jika kolom hasil identik: proposisi kesamaan terbukti benar.

  • Jika kolom kiri selalu ≤ kolom kanan: proposisi berupa himpunan bagian terbukti.

  • Jika ditemukan satu baris berbeda: proposisi salah; baris tersebut menjadi
    counterexample.

  • Untuk proposisi majemuk: periksa apakah kolom akhir seluruhnya bernilai 1, yang
    berarti proposisi itu tautologi himpunan.

Perbandingan dengan Metode Lain

Tabel keanggotaan bukan satu-satunya cara. Ada beberapa metode pembuktian lain:

Metode                   Kelebihan                     Kekurangan

Tabel keanggotaan        Sistematis, mudah diperiksa,  Panjang jika himpunan
                         cocok untuk pemula
                                                       banyak (2n baris)

Aljabar himpunan         Ringkas, memanfaatkan         Butuh hafal banyak
                         identitas yang sudah ada      hukum himpunan

                                    21
Pembuktian deduktif (ambil  Elegan dan umum      Lebih abstrak, sulit bagi
elemen sembarang)                                pemula

Diagram Venn                Visual dan intuitif  Tidak cukup untuk
                                                 pembuktian formal

Jadi, jika jumlah himpunan relatif sedikit (dua atau tiga), tabel keanggotaan adalah
pilihan terbaik karena setiap langkahnya kasat mata dan sulit dibantah.

Kesimpulan

Tabel keanggotaan adalah alat pembuktian yang jujur dan transparan: ia memaksa
kita memeriksa setiap kemungkinan tanpa kecuali. Selamat mencoba membuat
tabelmu sendiri — semakin sering berlatih, semakin cepat kamu menyusun dan
membaca polanya. Semangat belajar!

                            22
Pembuktian Proposisi Himpunan dengan Aljabar
Himpunan

Halo teman-teman! Pernahkah kalian merasa bingung ketika harus membuktikan

bahwa dua himpunan itu sebenarnya sama? Misalnya, apakah benar A ∩ (B ∪ C) =
(A ∩ B) ∪ (A ∩ C)? Nah, di bab ini kita akan belajar cara membuktikan pernyataan

semacam itu dengan rapi dan meyakinkan menggunakan aljabar himpunan. Ini
adalah cara paling formal dan paling diandalkan, jadi mari kita kuasai bersama.

Mengapa Diagram Venn Tidak Cukup?
Sebelum masuk ke aljabar himpunan, penting kita memahami dulu batas metode lain.

  • Diagram Venn hanya bisa dipakai kalau jumlah himpunan yang digambarkan
    sedikit. Jadi ia tidak praktis untuk kasus yang melibatkan banyak himpunan
    sekaligus.

  • Lebih penting lagi: Diagram Venn itu mengilustrasikan, bukan membuktikan. Ia
    menunjukkan contoh kasus, tetapi tidak menutup kemungkinan ada kasus lain
    yang belum tergambar.

  • Karena alasan itu, Diagram Venn tidak dianggap sebagai metode pembuktian
    yang valid secara formal. Ia berguna untuk intuisi, tetapi tidak cukup untuk ujian
    atau penulisan bukti resmi.

Ada juga metode tabel keanggotaan, yang bekerja dengan mendaftar setiap
kemungkinan keanggotaan elemen pada tiap himpunan. Metode ini lebih sistematis
daripada Diagram Venn, tetapi akan menjadi sangat panjang jika jumlah himpunan
bertambah besar. Di sinilah aljabar himpunan menawarkan jalan yang lebih elegan:
kita memanipulasi himpunan memakai hukum-hukum yang sudah terbukti, tanpa
perlu memeriksa elemen satu per satu.

Hukum-Hukum Aljabar Himpunan
Aljabar himpunan bekerja seperti aljabar biasa: ada identitas, ada sifat komutatif, dan
seterusnya. Berikut hukum-hukum inti yang wajib kalian hafal, karena inilah "senjata"
utama kita saat membuktikan.

Hukum            Bentuk

Hukum Identitas  A∪∅=A;A∩U =A

                         23
Hukum Dominasi     A∪U =U ;A∩∅=∅
                   A∪A=A;A∩A=A
Hukum Idempoten
                   (Ac   c  =  A
Hukum Komplemen
Ganda                   )

Hukum Komutatif    A∪B =B∪A;A∩B =B∩A
Hukum Asosiatif    (A ∪ B) ∪ C = A ∪ (B ∪ C) ; (A ∩ B) ∩ C = A ∩ (B ∩ C)
Hukum Distributif  A ∪ (B ∩ C) = (A ∪ B) ∩ (A ∪ C) ; A ∩ (B ∪ C) = (A ∩
Hukum De Morgan    B) ∪ (A ∩ C)
Hukum Absorpsi     (A ∪ B)c = Ac ∩ Bc ; (A ∩ B)c = Ac ∪ Bc
Hukum Komplemen    A ∪ (A ∩ B) = A ; A ∩ (A ∪ B) = A
                   A ∪ Ac = U ; A ∩ Ac = ∅

Perhatikan bahwa setiap hukum biasanya punya pasangan "kembar": versi untuk ∪
dan versi untuk ∩. Pola berpasangan ini disebut dualitas, dan sangat membantu

mengingat.

Langkah-Langkah Pembuktian dengan Aljabar Himpunan
Untuk membuktikan dua himpunan sama, kita tunjukkan bahwa ruas kiri dapat diubah
menjadi ruas kanan (atau sebaliknya) melalui serangkaian langkah yang sah. Ikuti alur
berikut:

  1. Tuliskan yang akan dibuktikan. Misalnya: buktikan A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩
    C ).

 2. Pilih satu ruas untuk dimanipulasi. Umumnya mulai dari ruas yang paling
    kompleks. Konsistenlah memilih satu sisi agar langkah tidak membingungkan.

 3. Terapkan satu hukum per langkah. Jangan melompati banyak aturan sekaligus;
    cantumkan alasan di setiap baris. Ini membuat bukti mudah diperiksa.

 4. Sederhanakan secara bertahap. Gunakan identitas, dominasi, absorpsi, dan
    sebagainya untuk mengurangi kerumitan.

                                  24
 5. Pastikan hasil akhir sama persis dengan ruas lainnya. Jika sudah identik, bukti

    selesai — tandai dengan simbol ■.

Tips penting: mulailah dari ruas yang punya lebih banyak operasi, dan bergeraklah
menuju bentuk yang lebih sederhana. Bila perlu, gunakan hukum komplemen untuk

mengganti Ac bila muncul U atau ∅.

Contoh Penerapan Identitas
Mari kita buktikan identitas distributif dari kiri ke kanan adalah cukup, karena
kesamaan sudah terlihat dari hukum distributif langsung. Sebaliknya, contoh yang

lebih menantang: buktikan A ∪ (A ∩ B) = A.

                  A ∪ (A ∩ B) = (A ∩ U ) ∪ (A ∩ B) (Hukum Identitas)

                          = A ∩ (U ∪ B) (Hukum Distributif)

                          = A ∩ U (Hukum Dominasi)

                          = A (Hukum Identitas)

Selesai! Perhatikan bagaimana setiap baris hanya memakai satu hukum, sehingga
alur penalarannya jelas.

Sekarang contoh dengan komplemen. Buktikan (A ∪ B)c = Ac ∩ Bc — ini tidak lain

adalah Hukum De Morgan, jadi langsung kita akui sebagai identitas. Namun bila soal

berbentuk  lebih  rumit,  misalnya  membuktikan  (A  ∩  B   c  ∪  C  =  Ac  ∪  Bc  ∪  C,  kita  bisa

                                                           )

menerapkan De Morgan pada (A ∩ B)c sehingga menjadi Ac ∪ Bc, lalu

menyatukannya dengan C lewat hukum asosiatif.

Latihan Pembuktian
Cobalah soal-soal berikut untuk melatih keterampilan kalian. Kerjakan langkah demi
langkah dan sertakan alasan di tiap baris.

  • Buktikan A ∩ (A ∪ B) = A menggunakan hukum absorpsi dan identitas.

                                    25
• Buktikan (A ∪ B) ∩ Ac = B ∩ Ac dengan hukum distributif dan komplemen.

• Tunjukkan bahwa A ∪ (B ∩ Ac) = A ∪ B dan jelaskan hukum apa saja yang

  dipakai.

• Buktikan (A ∩ B) ∪ (A ∩ Bc) = A dengan mendistribusikan A terlebih dahulu.

•  Gunakan  De  Morgan  untuk  membuktikan  (A  ∩  B  ∩  C   c  =  Ac  ∪  Bc  ∪  Cc.

                                                            )

Saat mengerjakan, biasakan menulis "Hukum …" di samping setiap langkah. Kebiasaan
ini bukan sekadar formalitas — ia melatih kalian berpikir tertib dan membuat bukti
kalian mudah dipahami oleh siapa pun yang membacanya.

Rangkuman Cepat
  • Aljabar himpunan adalah metode pembuktian formal dan valid, berbeda dari
    Diagram Venn yang hanya ilustratif.

  • Kunci suksesnya adalah menguasai hukum-hukum dasar dan menerapkannya
    satu per langkah.

  • Selalu mulai dari ruas yang paling kompleks, sederhanakan, lalu cocokkan dengan
    ruas lainnya.

Dengan latihan yang cukup, kalian akan semakin cepat mengenali hukum mana yang
tepat untuk dipakai. Selamat berlatih, dan jangan takut mencoba — setiap langkah
yang keliru justru mengajarkan kita cara berpikir yang lebih tajam!

                               26
Himpunan Fuzzy

Apa Itu Himpunan Fuzzy?

Halo! Selamat datang di bab yang sangat menarik. Kita akan membahas himpunan
fuzzy — sebuah konsep yang mungkin terdengar rumit, tetapi sebenarnya sangat
dekat dengan kehidupan sehari-hari kita. Mari kita mulai dengan pertanyaan
sederhana: apakah kamu termasuk "orang muda"? Kalau usiamu 25 tahun,
jawabannya jelas ya. Kalau 60 tahun, jelas tidak. Tapi bagaimana kalau usiamu 40
tahun? Nah, di sinilah himpunan fuzzy berperan.

Himpunan fuzzy adalah cara berpikir tentang keanggotaan yang tidak hitam-putih,
melainkan bertingkat.

Definisi Himpunan Fuzzy

Himpunan fuzzy adalah himpunan yang elemen-elemennya memiliki derajat
keanggotaan. Berbeda dengan himpunan klasik (himpunan tegas) di mana sebuah
elemen hanya punya dua kemungkinan — menjadi anggota (1) atau bukan anggota
(0) — dalam himpunan fuzzy, keanggotaan bisa berada di antara keduanya.

Bayangkan sebuah saklar lampu versus tombol peredup cahaya:

  • Himpunan klasik seperti saklar lampu: hanya ada ON (1) atau OFF (0).

  • Himpunan fuzzy seperti tombol peredup: cahaya bisa redup, sedang, atau terang —
    ada banyak tingkat di antaranya.

Dengan kata lain, himpunan fuzzy memberikan "kehalusan" pada cara kita
mengelompokkan sesuatu.

Derajat Keanggotaan pada Interval [0,1]

Ini adalah inti dari himpunan fuzzy. Derajat keanggotaan sebuah elemen dalam

himpunan fuzzy terletak pada interval [0, 1].

Artinya, nilai keanggotaan bisa berupa bilangan real apa pun antara 0 dan 1, inklusif.
Mari kita lihat maknanya:

Nilai Derajat Keanggotaan  Makna

0                          Elemen sepenuhnya bukan anggota himpunan

                           27
1  Elemen sepenuhnya anggota himpunan

Antara 0 dan 1 (misalnya 0,3 atau 0,7) Elemen sebagian menjadi anggota

Contoh sederhana: misalkan kita punya himpunan fuzzy "usia muda". Seseorang

berusia 20 tahun mungkin punya derajat keanggotaan 0,9 dalam himpunan ini,
sedangkan seseorang berusia 35 tahun punya derajat keanggotaan 0,4. Keduanya

masih "sebagian muda", tetapi dengan tingkat yang berbeda.

Perhatikan bahwa intervalnya tertutup pada kedua ujung, yaitu [0, 1] dan bukan (0, 1).
Jadi nilai 0 dan 1 tetap sah digunakan — inilah yang menghubungkan himpunan fuzzy

dengan himpunan klasik sebagai kasus khusus.

Sifat Batasan yang Samar

Salah satu ciri khas himpunan fuzzy adalah batasan-batasannya lebih bersifat samar.
Dalam himpunan klasik, batas antara "anggota" dan "bukan anggota" sangat tegas:
usia 39 tahun mungkin bukan "muda", usia 40 tahun mungkin "muda" — ada garis
pemisah yang jelas.

Dalam himpunan fuzzy, batasan itu tidak tajam. Transisi dari "bukan anggota" menjadi
"anggota" terjadi secara bertahap. Inilah yang membuat himpunan fuzzy sangat cocok
untuk memodelkan konsep-konsep dunia nyata yang kabur, seperti:

  • "tinggi", "pendek", "sedang"

  • "panas", "dingin", "hangat"

  • "cepat", "lambat"

  • "muda", "tua"

Konsep-konsep seperti ini tidak memiliki ambang batas yang pasti. Berapa sentimeter
seseorang baru bisa disebut "tinggi"? Berapa derajat Celsius udara baru disebut
"panas"? Tidak ada jawaban tunggal yang tegas — dan himpunan fuzzy merangkul
ketidaktegasan ini alih-alih memaksakan batas yang kaku.

Variabel Linguistik dalam Teori Fuzzy

Dalam teori fuzzy, kita biasanya menggunakan variabel linguistik. Variabel linguistik
adalah variabel yang nilainya berupa kata-kata fuzzy, bukan angka pasti.

   28
Sebagai contoh, alih-alih menggunakan variabel numerik "usia = 42", kita bisa
menggunakan variabel linguistik "usia" dengan nilai-nilai linguistik seperti:

  • muda
  • paruh baya
  • tua
Setiap nilai linguistik ini kemudian dipetakan ke himpunan fuzzy dengan derajat
keanggotaan masing-masing. Inilah yang membuat sistem fuzzy mampu "berbicara"
dalam bahasa manusia sekaligus "menghitung" secara matematis.

Contoh Penerapan: Penggolongan Usia

Mari kita terapkan semua konsep di atas pada contoh penggolongan usia. Ini adalah
contoh klasik yang sering dipakai untuk menggambarkan himpunan fuzzy.
Misalkan kita mendefinisikan tiga himpunan fuzzy:

  • MUDA
  • PARUH BAYA
  • TUA
Seorang berusia 35 tahun bisa menjadi anggota sebagian dari beberapa himpunan
sekaligus. Mari kita lihat ilustrasinya:

Usia   Derajat Keanggotaan  Derajat Keanggotaan  Derajat Keanggotaan
       MUDA                 PARUH BAYA           TUA

20

tahun  0,9                  0,1                  0,0

35

tahun  0,5                  0,7                  0,2

50

tahun  0,1                  0,6                  0,6

70

tahun  0,0                  0,2                  0,9

                                 29
Perhatikan beberapa hal penting:
  • Keanggotaan bisa tumpang tindih. Seseorang berusia 35 tahun bisa sekaligus

    "cukup muda" (0,5) dan "cukup paruh baya" (0,7). Ini tidak mungkin dalam

    himpunan klasik.
  • Transisi berlangsung mulus. Nilai derajat keanggotaan berubah secara bertahap

    seiring bertambahnya usia, mencerminkan sifat samar dari batasan usia.
  • Tidak ada garis pemisah tajam. Tidak ada titik di mana seseorang tiba-tiba

    berubah dari "muda" menjadi "tua".

Mengapa Ini Penting?

Pendekatan fuzzy ini jauh lebih realistis untuk sistem yang berinteraksi dengan
manusia atau fenomena alam. Sistem pengambilan keputusan, pengendalian suhu,
hingga rekomendasi produk sering memanfaatkan logika fuzzy karena dunia nyata
jarang sekali hitam-putih.
Ingat poin-poin kunci berikut:

  • Himpunan fuzzy memberi setiap elemen derajat keanggotaan.

  • Derajat keanggotaan berada di interval [0, 1].

  • Batasan himpunan fuzzy bersifat samar, bukan tegas.
  • Variabel linguistik menggunakan kata-kata fuzzy sebagai nilai.
  • Penggolongan usia adalah contoh nyata yang menunjukkan semua prinsip ini

    bekerja bersama.
Dengan memahami dasar-dasar ini, kamu sudah memiliki fondasi yang kuat untuk
mempelajari operasi dan penerapan himpunan fuzzy lebih lanjut. Selamat belajar, dan
jangan ragu untuk kembali ke bab ini saat kamu butuh penyegaran konsep!

                                                                               30
Integrasi dan Latihan Komprehensif

Selamat datang di bab terakhir! Di sini kita akan menyatukan semua yang sudah kamu
pelajari tentang himpunan. Tujuannya bukan sekadar menghafal rumus, tetapi melatih
cara berpikir: mengenali kapan sebuah soal membutuhkan prinsip inklusi-eksklusi,
kapan cukup dengan diagram Venn, dan kapan harus menulis pembuktian formal.
Mari kita mulai dengan memperkuat fondasi, lalu naik ke latihan terintegrasi.
Mengingat Kembali Peta Konsep
Sebelum masuk latihan, ingat bahwa topik-topik himpunan saling berkait. Operasi
himpunan (gabungan, irisan, selisih) adalah alat dasar. Dari situ lahir prinsip inklusi-
eksklusi, yang pada dasarnya adalah cara menghitung gabungan tanpa menghitung
anggota yang sama dua kali. Diagram Venn membantu memvisualisasikan,
sedangkan pembuktian proposisi melatih penalaran bahwa dua himpunan benar-
benar sama. Semua ini akan muncul kembali dalam soal survei dan sistem informasi.
Latihan Inklusi-Eksklusi: Kasus Kelipatan Bilangan
Prinsip inklusi-eksklusi untuk dua himpunan:

                                   ∣A ∪ B∣ = ∣A∣ + ∣B∣ − ∣A ∩ B∣

Untuk tiga himpunan:

     ∣A ∪ B ∪ C∣ = ∣A∣ + ∣B∣ + ∣C∣ − ∣A ∩ B∣ − ∣A ∩ C∣ − ∣B ∩ C∣ + ∣A ∩ B ∩ C∣

Pola pentingnya: tambah tunggal, kurangi pasangan, tambah tripel. Untuk empat
himpunan, pola berlanjut bergantian.
Contoh: Berapa banyak bilangan bulat dari 1 sampai 100 yang habis dibagi 2 atau 3?

  • A = kelipatan 2: ∣A∣ = ⌊100/2⌋ = 50
  • B = kelipatan 3: ∣B∣ = ⌊100/3⌋ = 33
  • A ∩ B = kelipatan 6: ∣A ∩ B∣ = ⌊100/6⌋ = 16
  • Maka ∣A ∪ B∣ = 50 + 33 − 16 = 67.

                                                                               31
Tips: Untuk kelipatan, gunakan pembulatan ke bawah ⌊⋅⌋, dan irisan berarti kelipatan

KPK (Kelipatan Persekutuan Terkecil).

Latihan Survei dan Gabungan Himpunan
Soal survei selalu bercerita tentang orang yang menyukai dua atau tiga hal. Strategi
jitu: gambar diagram Venn, isi dari irisan terdalam, lalu keluar ke daerah tunggal.

Contoh: Dari 40 siswa, 25 suka matematika, 20 suka fisika, dan 10 suka keduanya.
Berapa yang tidak suka keduanya?

  • ∣M ∪ F ∣ = 25 + 20 − 10 = 35

  • Yang tidak suka keduanya = 40 − 35 = 5 siswa.

Jebakan umum: Angka "suka keduanya" sering dipakai untuk mengisi irisan, bukan
menambah. Selalu cek apakah bilangan yang diberikan adalah gabungan, irisan, atau
tunggal.

Latihan Pembuktian Proposisi Himpunan

Pembuktian biasanya memakai dua arah: tunjukkan A ⊆ B dan B ⊆ A, maka A = B.

Contoh proposisi: A ∩ (B ∪ C) = (A ∩ B) ∪ (A ∩ C) (hukum distributif).

  • Ambil x ∈ A ∩ (B ∪ C). Maka x ∈ A dan x ∈ B ∪ C. Jika x ∈ B, maka x ∈ A ∩ B;
    jika x ∈ C, maka x ∈ A ∩ C. Jadi x ada di ruas kanan.

  • Sebaliknya, jika x ∈ (A ∩ B) ∪ (A ∩ C), maka x ∈ A dan x di B atau C, sehingga
    x ∈ A ∩ (B ∪ C).

Karena kedua arah terbukti, kesamaan berlaku. Cara lain adalah memakai tabel
keanggotaan (benar/salah) untuk semua kombinasi.

x∈A  x∈B  x∈C  x ∈ A ∩ (B ∪ C)  x ∈ (A ∩ B) ∪ (A ∩ C)

B    B    B    B                B

B    B    S    B                B

B    S    B    B                B

B    S    S    S                S

                  32
Review Keterkaitan Antar Topik
  • Operasi himpunan menjadi kosakata dasar untuk semua soal.

  • Diagram Venn adalah alat visual untuk soal survei.

  • Inklusi-eksklusi adalah rumus untuk gabungan besar.

  • Pembuktian memastikan identitas himpunan benar secara logis.

  • Sistem informasi memakai semua ini untuk mengelola data.

Penerapan dalam Sistem Informasi
Di dunia sistem informasi, himpunan dipakai untuk pencarian database dan
pengelolaan pengguna. Misalnya, pengguna dengan atribut tertentu membentuk
himpunan; pencarian "pengguna yang aktif atau berlangganan premium" adalah
gabungan, sedangkan "aktif dan premium" adalah irisan. Prinsip inklusi-eksklusi
dipakai untuk menghitung total pengguna unik saat data diambil dari beberapa
sumber yang mungkin tumpang tindih.

Seperti pada contoh klasifikasi usia — bayi, anak-anak, remaja, dewasa — himpunan
membantu kita mengelompokkan data. Satu orang biasanya masuk tepat satu

kategori, sehingga kategori-kategori itu saling lepas (A ∩ B = ∅). Jika ada tumpang

tindih, inklusi-eksklusi kembali berperan.

Rangkuman Cepat

Konsep         Rumus / Ide Kunci                 Kapan Dipakai

Gabungan dua   ∣A ∪ B∣ = ∣A∣ + ∣B∣ − ∣A ∩ B∣     Hitung total unik
himpunan

Tiga himpunan  Tambah tunggal, kurang pasangan,  Survei tiga
               tambah tripel                     kategori

Kelipatan      Gunakan ⌊n/k⌋ dan KPK             Soal bilangan

Pembuktian     Tunjukkan dua arah ⊆              Identitas
                                                 himpunan

Kamu sudah menempuh perjalanan panjang! Latihan terintegrasi seperti ini
melatihmu berpindah antar konsep dengan lancar. Semakin sering berlatih, semakin

               33
cepat kamu mengenali pola soal. Selamat belajar, dan sampai jumpa di petualangan
himpunan berikutnya!

                                                                               34
