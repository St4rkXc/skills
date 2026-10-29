---
mode: detailed
pages: 35
words: 7049
---

      pelajarin.ai

Pendahuluan dan Ringkasan Materi Sebelumnya

Halo! Selamat datang kembali di pembahasan logika. Sebelum kita melangkah ke
materi yang lebih menantang, mari kita segarkan kembali ingatan tentang fondasi
yang sudah kita pelajari. Anggap saja sesi ini sebagai "pemanasan" — karena semua
konsep lanjutan nanti akan berdiri di atas dasar yang kita ulas di sini. Kalau fondasinya
kuat, materi berikutnya akan terasa jauh lebih mudah. Yuk, kita mulai!

Mengingat Kembali: Apa Itu Proposisi?

Proposisi adalah kalimat deklaratif, yaitu kalimat yang menyatakan suatu fakta, yang
nilainya bisa benar atau salah, tetapi tidak mungkin keduanya sekaligus. Ini poin
penting: sebuah proposisi harus punya nilai kebenaran yang jelas dan tunggal. Kalau
sebuah kalimat tidak bisa dinilai benar atau salah, maka ia bukan proposisi.
Perhatikan contoh-contoh berikut:

  • "Ibukota Provinsi Jawa Tengah adalah Semarang" → ini proposisi, dan nilainya Benar
    (T).

  • "42 + 8 = 26" → ini proposisi, dan nilainya Salah (F), karena hasil yang benar
    adalah 50.

Dari dua contoh ini kita bisa melihat pola sederhananya: proposisi selalu berupa
pernyataan yang bisa kita "cek" kebenarannya.

Menggabungkan Proposisi

Proposisi tunggal bisa kita gabungkan menjadi proposisi baru yang lebih kompleks.
Ada tiga operasi dasar penggabungan yang wajib kita kuasai:

  • Negasi — membalik nilai kebenaran sebuah proposisi.
  • Konjungsi — menggabungkan dua proposisi dengan kata "dan".
  • Disjungsi — menggabungkan dua proposisi dengan kata "atau".
Mari kita bedah satu per satu, lengkap dengan tabel kebenarannya.
Negasi
Negasi adalah operasi yang paling sederhana: ia hanya membalik nilai. Kalau

proposisi p bernilai benar, maka ∼ p (dibaca "tidak p") bernilai salah, dan sebaliknya.

                                                                                1
p        ∼p

T        F

F        T

Konjungsi

Konjungsi (p ∧ q) bernilai benar hanya jika kedua proposisi benar. Kalau salah satu

saja salah, hasilnya salah.

p  q         p∧q

T  T         T

T  F         F

F  T         F

F  F         F

Disjungsi

Disjungsi (p ∨ q) bernilai benar jika minimal salah satu proposisi benar. Ia hanya salah

ketika kedua proposisi salah.

p  q         p∨q

T  T         T

T  F         T

F  T         T

F  F         F

Tiga tabel kebenaran di atas adalah "kamus" yang akan sering kita pakai. Kalau kamu
sudah hafal polanya, materi lanjutan akan terasa jauh lebih ringan.

      2
Peta Materi yang Akan Datang

Setelah fondasi ini, kita akan menaiki tangga materi berikutnya. Berikut gambaran
besar apa yang akan kita pelajari:

  • Disjungsi Eksklusif (XOR) — variasi dari disjungsi yang punya aturan berbeda.
  • Operasi Logika dalam Komputer — bagaimana logika diterapkan di dunia

    pemrograman.
  • Proposisi Bersyarat (Implikasi) — proposisi berbentuk "jika ... maka ...".
  • Varian Proposisi Bersyarat — konvers, invers, dan kontraposisi dari implikasi.
  • Bikondisional (Bi-implikasi) — proposisi berbentuk "jika dan hanya jika".
  • Inferensi — cara menarik kesimpulan yang sah.
  • Argumen — menyusun dan menilai validitas sebuah argumen.
Setiap topik ini akan kita bahas tuntas di bab-bab berikutnya, jadi pastikan dasar di
bab ini benar-benar sudah kamu kuasai.

Sedikit Bocoran: Disjungsi Eksklusif

Sebagai gambaran awal, kata "atau" ternyata punya dua makna berbeda dalam
logika — dan membedakannya itu penting!

  1. Inclusive or — "atau" berarti "p atau q atau keduanya". Contoh: "Tenaga IT yang

    dibutuhkan harus menguasai Bahasa C++ atau Java." Di sini, menguasai keduanya
    justru nilai plus, jadi keduanya boleh benar.

 2. Exclusive or (XOR) — "atau" berarti "p atau q tetapi bukan keduanya". Contoh: "Ia

    dihukum 5 tahun atau denda 10 juta." Di sini, tidak mungkin keduanya terjadi
    sekaligus — hanya salah satu.
Perbedaan halus inilah yang akan kita dalami di bab berikutnya, karena XOR punya
tabel kebenaran tersendiri yang berbeda dari disjungsi biasa.

Sedikit Bocoran: Logika di Dunia Komputer

Logika bukan cuma teori di atas kertas — ia hidup di dalam komputer! Bahasa
pemrograman umumnya menyediakan tipe data boolean untuk menampung nilai
logika. Contohnya tipe boolean di Bahasa Pascal, atau logical di Bahasa Fortran.

                                                                                3
Tipe boolean hanya punya dua konstanta nilai: true dan false . Peubah (variabel)
yang bertipe boolean disebut peubah boolean, dan nilainya hanya salah satu dari dua
itu.

Operasi boolean dinyatakan dalam ekspresi logika (atau ekspresi boolean), dengan
operator AND, OR, XOR, dan NOT. Hasilnya selalu salah satu dari true atau false .

Menariknya, ekspresi boolean di pemrograman berkorespondensi langsung dengan
notasi logika kita. Misalnya, jika x1 , x2 , x3 , dan x4 adalah peubah boolean dalam
Bahasa Pascal, maka ekspresi berikut valid:

•  x1  and  x2   ↔  x    ∧  x

                      1       2

•  x1  or  (not  (x2     and  x3))  ↔  x    ∨  ∼  (x2  ∧  x3)

                                         1

Jadi apa yang kamu pelajari di logika itu persis apa yang dijalankan komputer. Selain
itu, ada juga operasi bit, karena komputer merepresentasikan seluruh informasi
menggunakan bit — satuan terkecil data yang bernilai 0 atau 1.

Penutup

Sampai di sini, kamu sudah menyegarkan kembali tiga pilar utama: definisi proposisi,
operasi penggabungan (negasi, konjungsi, disjungsi), dan tabel kebenarannya.
Dengan bekal ini, kamu siap menaklukkan materi lanjutan — dari disjungsi eksklusif,
operasi logika komputer, implikasi beserta variannya, bikondisional, hingga inferensi
dan argumen. Jangan ragu untuk kembali ke bab ini kalau ada yang perlu diulang.
Selamat belajar, dan sampai jumpa di bab berikutnya!

                                                          4
Disjungsi Eksklusif (XOR)

Memahami Dua Wajah Kata "Atau"

Halo, teman-teman! Pernahkah kalian memperhatikan bahwa kata "atau" dalam
kehidupan sehari-hari ternyata punya dua makna yang berbeda? Kadang "atau"
berarti "salah satu, boleh keduanya", tapi kadang juga berarti "salah satu, tapi tidak
boleh keduanya". Nah, dalam logika, kedua makna ini punya nama dan aturan yang
jelas. Mari kita bedah bersama!

Dalam logika, kita bekerja dengan proposisi — pernyataan yang bisa bernilai benar
(true/T) atau salah (false/F). Menariknya, nilai kebenaran ini bisa kita wakilkan dengan
sebuah bit, yaitu angka yang hanya punya dua kemungkinan nilai: 1 atau 0. Kita
sepakat menyatakan 1 untuk merepresentasikan true (T) dan 0 untuk
merepresentasikan false (F).

Karena itu, ada korespondensi indah antara operasi pada bit dan operasi logika.
Misalnya, operasi bit 1 ⊕ 0 bersesuaian dengan operasi logika T ⊕ F . Notasi yang
akan sering kita pakai adalah:

  • ~ untuk melambangkan operator NOT
  • ⋀ untuk melambangkan operator AND
  • ∨ untuk melambangkan operator OR
  • ⊕ untuk melambangkan operator XOR

Perhatikan khususnya dua operator terakhir: ∨ (OR) dan ⊕ (XOR). Keduanya sering
diterjemahkan sebagai "atau", namun keduanya sangat berbeda. Inilah inti bab ini.

Inclusive Or: "p atau q atau keduanya"

Inclusive or adalah makna "atau" yang paling longgar. Ia menyatakan bahwa
pernyataan majemuk benar apabila minimal salah satu dari p atau q benar —
termasuk jika keduanya benar sekaligus. Dengan kata lain, hasilnya benar kecuali p
dan q keduanya salah.
Ciri khas inclusive or adalah kalimat "p atau q atau keduanya". Operator ini
dilambangkan dengan ∨ .

Mari lihat contohnya dalam kalimat sehari-hari:
  • "Untuk masuk ke acara ini, kamu harus membawa kartu undangan atau
    menunjukkan email konfirmasi."

                                                                                5
  • "Menu sarapan tersedia kopi atau teh."
  • "Dia mahir berbahasa Inggris atau Prancis."
Pada contoh pertama, seorang tamu yang membawa kartu undangan dan juga
menunjukkan email konfirmasi tetap diperbolehkan masuk. Tidak ada larangan untuk
memenuhi kedua syarat sekaligus. Inilah semangat inclusive or: semua kombinasi
yang mengandung minimal satu kebenaran tetap dianggap benar.

Dalam pemrograman dan matematika, ketika kita menulis "A atau B" tanpa penjelasan
tambahan, biasanya yang dimaksud adalah inclusive or, kecuali dinyatakan lain.

Exclusive Or: "p atau q tetapi bukan keduanya"

Nah, sekarang datang si kembarannya. Exclusive or (sering disingkat XOR) memiliki
makna yang lebih ketat. Ia menyatakan bahwa pernyataan majemuk benar hanya
apabila tepat satu dari p atau q bernilai benar — tidak boleh keduanya benar, dan
tentu tidak boleh keduanya salah.
Ciri khasnya adalah kalimat "p atau q tetapi bukan keduanya". Operator ini
dilambangkan dengan ⊕ .

Contoh dalam kalimat sehari-hari:
  • "Kamu boleh memilih es krim atau kue sebagai hidangan penutup."
  • "Pemenang undian hanya bisa menerima uang tunai atau hadiah barang, tidak
    keduanya."
  • "Lampu ruangan ini menyala atau mati — hanya satu kondisi yang berlaku."

Pada contoh pertama, jika kamu mengambil es krim dan kue sekaligus, itu melanggar
aturan. Kamu harus memilih tepat satu. Inilah perbedaan mendasar dengan inclusive
or.

XOR juga sangat akrab di dunia komputer. Operasi ⊕ sering dipakai dalam kriptografi,
deteksi kesalahan (error detection), dan logika rangkaian digital, karena sifatnya yang
"tepat satu" sangat berguna untuk mendeteksi perbedaan atau ketidakcocokan.

Tabel Kebenaran XOR

Cara paling jernih untuk memahami XOR adalah melalui tabel kebenarannya. Karena
ada dua proposisi (p dan q), ada empat kombinasi nilai kebenaran yang mungkin.
Namun, kita akan tampilkan sekaligus dalam bentuk logika (T/F) dan bentuk bit (1/0),
sesuai korespondensi yang sudah kita bahas.

                                                                                6
p  q     p⊕q  Keterangan

T  T     F    Keduanya benar → XOR salah (karena "bukan keduanya")

T  F     T    Tepat satu benar (p) → XOR benar

F  T     T    Tepat satu benar (q) → XOR benar

F  F     F    Keduanya salah → XOR salah

Dan dalam bentuk bit, tabelnya terlihat seperti ini:

p             q                                       p⊕q

1             1                                       0

1             0                                       1

0             1                                       1

0             0                                       0

Perhatikan pola yang cantik: XOR menghasilkan 1 (benar) ketika p dan q berbeda, dan
menghasilkan 0 (salah) ketika p dan q sama. Inilah sebabnya XOR sering disebut
"operator perbedaan" (difference operator). Bandingkan dengan OR biasa ( ∨ ), yang
menghasilkan benar pada tiga dari empat baris — hanya salah ketika kedua proposisi
salah.

Membandingkan OR dan XOR secara Langsung

Agar perbedaan keduanya semakin mengendap, mari kita susun keduanya
berdampingan:

p     q          p ∨ q (Inclusive)                       p ⊕ q (Exclusive)

T     T          T                                       F

T     F          T                                       T

                          7
F  T  T     T

F  F  F     F

Lihatlah baris pertama! Di sinilah kedua operator berbeda secara dramatis. Untuk p
dan q yang keduanya benar: inclusive or berkata T (karena "atau keduanya"),
sedangkan exclusive or berkata F (karena "bukan keduanya"). Pada tiga baris lainnya,
keduanya menghasilkan nilai yang sama. Jadi, satu-satunya titik perbedaan adalah
ketika kedua proposisi bernilai benar.

Kesimpulan dan Kunci Mengingat

Untuk membedakan keduanya dengan mudah, ingatlah frasa kuncinya:

  • Inclusive or ( ∨ ): "p atau q atau keduanya" → benar jika setidaknya satu benar.

  • Exclusive or ( ⊕ ): "p atau q tetapi bukan keduanya" → benar jika tepat satu benar.

Dalam praktik, XOR sangat berguna ketika kita ingin menyatakan pilihan yang saling
meniadakan (mutually exclusive), sedangkan inclusive or dipakai ketika memenuhi
kedua opsi sekaligus tetap diperbolehkan.

Satu catatan penting sebelum kita akhiri: XOR berbeda dari proposisi bersyarat
(implikasi) yang berbentuk "jika p, maka q" dan dinotasikan p → q . Implikasi punya
struktur logika tersendiri dengan hipotesis (antesenden) dan konklusi (konsekuen),
sehingga akan dibahas lebih dalam di catatan tersendiri.

Selamat belajar! Dengan memahami dua wajah kata "atau" ini, kemampuanmu
menalar proposisi majemuk akan semakin tajam. Semangat!

         8
Operasi Logika dalam Komputer

Tipe Data Boolean dalam Bahasa Pemrograman

Halo! Mari kita pelajari salah satu fondasi terpenting dalam ilmu komputer: operasi
logika. Topik ini menghubungkan konsep logika formal yang kita pelajari di
matematika dengan cara komputer "berpikir" menggunakan bit dan gerbang logika.
Sebelum masuk ke detail, mari kita pahami dulu apa itu tipe data boolean. Boolean
adalah tipe data yang hanya memiliki dua nilai kemungkinan: benar (true) atau salah
(false). Nama "boolean" berasal dari matematikawan George Boole yang
mengembangkan aljabar logika.
Dalam bahasa pemrograman, representasi boolean bervariasi:

  • Pascal: menggunakan kata kunci boolean dengan nilai true dan false
  • Fortran: menggunakan tipe LOGICAL dengan nilai .TRUE. dan .FALSE.
  • Bahasa modern (seperti C, Java, Python): umumnya menggunakan true / false

    atau 1 / 0
Tipe data ini sangat fundamental karena hampir semua pengambilan keputusan
dalam program—mulai dari validasi input hingga kontrol alur—bergantung padanya.

Ekspresi Boolean dan Operator Boolean

Ekspresi boolean adalah ekspresi yang menghasilkan nilai benar atau salah. Ekspresi
ini dibangun dari operasi perbandingan (seperti > , < , = , >= , <= , != ) yang
digabungkan dengan operator boolean.
Terdapat empat operator boolean utama yang wajib kamu kuasai:

1. AND (Konjungsi) — Notasi: ∧

Menghasilkan benar hanya jika kedua operand benar. Dalam notasi formal: p ∧ q.

2. OR (Disjungsi) — Notasi: ∨

Menghasilkan benar jika minimal satu operand benar. Dalam notasi formal: p ∨ q.

3. XOR (Exclusive OR) — Notasi: ⊕

Menghasilkan benar jika tepat satu operand benar (tidak keduanya). Dalam notasi

formal: p ⊕ q.

                                                                                9
4. NOT (Negasi) — Notasi: ¬ atau ∼

Membalikkan nilai: benar menjadi salah, salah menjadi benar.

Tabel Kebenaran Operator Boolean

Mari kita lihat bagaimana keempat operator ini bekerja. Tabel berikut menunjukkan

hasil untuk semua kombinasi nilai p dan q:

p  q  p∧q  p∨q  p⊕q  ¬p

B  B  B    B    S    S

B  S  S    B    B    S

S  B  S    B    B    B

S  S  S    S    S    B

Perhatikan pola penting: AND hanya benar pada satu baris, sementara OR salah hanya
pada satu baris. XOR adalah "OR yang eksklusif"—benar hanya ketika kedua operand
berbeda.

Contoh Ekspresi Boolean dan Padanan dalam Logika Formal

Mari kita lihat contoh nyata dari sumber materi. Perhatikan proposisi berikut:

   "Syarat cukup agar pom bensin meledak adalah percikan api dari rokok."

Untuk mengubahnya menjadi bentuk standar "Jika p maka q", kita perlu memahami

konsep syarat cukup. Ingat aturan penting ini:

   p → q dapat dibaca "p adalah syarat cukup untuk q"

Maka langkahnya adalah:

  1. Identifikasi proposisi atomik: p = "api memercik dari rokok", q = "pom bensin

    meledak"
 2. Susun sesuai format: Karena percikan api adalah syarat cukup, kita dapatkan "Jika

    api memercik dari rokok, maka pom bensin meledak."

           10
Inilah padanan langsung antara bahasa sehari-hari dengan logika formal—suatu
keterampilan yang sangat berguna saat menulis kondisi dalam program.

Implikasi dalam Bahasa Pemrograman: Struktur If-Then
Konsep implikasi p → q diwujudkan dalam pemrograman melalui struktur if-then:

    if c then S

  • c adalah ekspresi logika yang menyatakan syarat/kondisi
  • S adalah satu atau lebih pernyataan yang dieksekusi
  • S dieksekusi jika c benar, dan tidak dieksekusi jika c salah

Contoh Kasus: Analisis Eksekusi If-Then
Misalkan dalam program Pascal terdapat pernyataan:

    if x > y then y := x + 10;

Mari kita hitung nilai y setelah eksekusi untuk dua skenario:
Skenario 1: x = 2, y = 1

  • Ekspresi x > y → 2 > 1 bernilai benar
  • Pernyataan y := x + 10 dilaksanakan
  • Nilai y sekarang menjadi 2 + 10 = 12
Skenario 2: x = 3, y = 5
  • Ekspresi x > y → 3 > 5 bernilai salah
  • Pernyataan y := x + 10 tidak dilaksanakan
  • Nilai y tetap 5

Contoh ini menunjukkan bagaimana ekspresi boolean mengontrol jalannya program—
inilah inti dari operasi logika dalam praktik.

Operasi Bit: Representasi True dan False

Sekarang pertanyaan menariknya: bagaimana komputer benar-benar menyimpan
nilai boolean? Jawabannya ada di level bit—unit terkecil data digital.

                                                                                11
Komputer merepresentasikan nilai boolean menggunakan bit:
  • 1 mewakili true (benar)
  • 0 mewakili false (salah)

Kesetaraan Operator Logika dan Operasi Bit

Inilah bagian yang indah: setiap operator logika boolean memiliki padanan langsung
sebagai operasi bit. Operasi bit bekerja pada level bit individual, memungkinkan
pemrosesan paralel yang sangat efisien.

Operator Logika  Notasi  Operasi Bit (Bitwise)                Simbol dalam Pemrograman

AND              ∧ atau ∼ Bitwise AND                         &
OR
XOR              ∨       Bitwise OR                           |
NOT
                 ⊕       Bitwise XOR                          ^

                 ¬       Bitwise NOT                          ~

Bagaimana Operasi Bit Bekerja?

Mari kita lihat contoh dengan bilangan 4-bit. Misalkan a = 1100 dan b = 1010:
Bitwise AND (a&b): Bandingkan setiap bit; hasil 1 hanya jika kedua bit 1.

                                          1100 ∧ 1010 = 1000
Bitwise OR (a ∣ b): Hasil 1 jika minimal satu bit 1.

                                          1100 ∨ 1010 = 1110
Bitwise XOR (a ⊕ b): Hasil 1 jika bit berbeda.

                         1100 ⊕ 1010 = 0110

                         12
Bitwise NOT (∼ a): Membalik semua bit.

                                             ∼ 1100 = 0011

Perhatikan bahwa operasi bit ini menerapkan tabel kebenaran yang sama persis
dengan operator logika pada setiap posisi bit secara independen—inilah yang disebut
operasi paralel bit-by-bit.

Mengapa Ini Penting?

Keindahan dari kesetaraan ini adalah: logika formal, tipe data boolean, dan operasi bit
semuanya adalah wajah berbeda dari konsep yang sama. Ketika kamu menulis if (x
> 0) && (y < 10) , di balik layar komputer menjalankan operasi bit pada level perangkat
keras. Memahami hubungan ini membantumu:

  1. Menulis kode yang efisien dengan memanfaatkan operasi bit untuk komputasi
    cepat

 2. Memahami kontrol alur program secara lebih mendalam
 3. Menghubungkan teori logika matematika dengan implementasi praktis di

    komputer
Dengan menguasai boolean, ekspresi boolean, operator logika, dan operasi bit ini,
kamu telah membuka pintu menuju pemahaman yang lebih dalam tentang
bagaimana komputer benar-benar "berpikir" dan membuat keputusan. Selamat
belajar!

                                                                               13
Proposisi Bersyarat (Implikasi)

Halo! Kali ini kita akan membahas salah satu jenis proposisi majemuk yang paling
penting dan paling sering muncul, baik di matematika maupun di dunia
pemrograman: proposisi bersyarat atau yang biasa disebut implikasi. Selamat belajar
— topik ini sebenarnya sangat logis dan menyenangkan begitu kamu memahami
polanya!

Apa Itu Proposisi Bersyarat?

Proposisi bersyarat (disebut juga proposisi kondisional atau implikasi) adalah
proposisi majemuk yang berbentuk "jika p maka q". Proposisi ini menghubungkan dua
proposisi tunggal, yaitu p dan q, dengan sebuah hubungan sebab-akibat atau syarat.

Dalam implikasi, kita mengenal beberapa istilah penting:
  • p disebut hipotesis, antesenden, atau premis (bagian "jika").
  • q disebut konklusi atau konsekuen (bagian "maka").

Notasi untuk implikasi adalah:

      p→q

Dibaca: "jika p maka q". Bagian p adalah syarat yang harus terpenuhi, sedangkan q
adalah akibat yang mengikuti.

Tabel Kebenaran Implikasi

Kunci memahami implikasi adalah tabel kebenarannya. Perhatikan bahwa implikasi
hanya bernilai salah ketika hipotesis benar tetapi konklusi salah. Di semua
kemungkinan lain, implikasi bernilai benar.

p  q       p→q

B  B       B

B  S       S

S  B       B

      14
S  S      B

Mengapa baris ketiga dan keempat bernilai benar? Karena jika hipotesisnya sudah
salah, kita tidak bisa "menyalahkan" implikasi tersebut — janji yang tidak pernah
ditepati karena syaratnya tidak terpenuhi tetap dianggap tidak dilanggar.

Berbagai Cara Mengekspresikan Implikasi

Kalimat "jika p maka q" bisa diungkapkan dengan banyak cara. Semuanya bermakna
sama:

  • Jika p, maka q.

  • Jika p, q.

  • p mengakibatkan q.

  • q jika p.

  • q hanya jika p.

  • p adalah syarat cukup untuk q.

  • q adalah syarat perlu untuk p.

  •p⟹q

  • q apabila p.

Contoh dalam Kalimat Sehari-hari

Perhatikan kalimat berikut: "Jika Amir mempunyai mobil, maka ia orang kaya."
Kalimat ini adalah sebuah implikasi, dengan p = "Amir mempunyai mobil" dan q =
"Amir orang kaya".

Terkadang, sebuah proposisi belum berbentuk standar "jika p maka q". Misalnya
pernyataan "Perlu ada angin agar layang-layang bisa terbang." Untuk mengubahnya
ke bentuk standar, kita susun ulang menjadi: "Jika layang-layang bisa terbang, maka
ada angin." Jadi, hati-hatilah dalam menentukan mana yang menjadi p dan mana
yang menjadi q.

Konvers, Invers, dan Kontraposisi
Dari sebuah implikasi p → q, kita dapat membentuk tiga varian proposisi bersyarat:

  • Konvers: q → p — menukar posisi p dan q.

      15
  • Invers: ¬p → ¬q — menegasikan kedua bagian.
  • Kontraposisi: ¬q → ¬p — menukar posisi sekaligus menegasikan keduanya.

Contoh: Dari pernyataan "Jika Amir mempunyai mobil, maka ia orang kaya":
  • Konvers: Jika Amir orang kaya, maka ia mempunyai mobil.
  • Invers: Jika Amir tidak mempunyai mobil, maka ia bukan orang kaya.
  • Kontraposisi: Jika Amir bukan orang kaya, maka ia tidak mempunyai mobil.

Yang menarik, kontraposisi selalu bernilai benar yang sama dengan implikasi aslinya
(ekuivalen), sedangkan konvers dan invers belum tentu. Perhatikan tabel kebenaran
keempatnya:

p  q  p→q  Konvers q → p  Invers ¬p → ¬q  Kontraposisi ¬q → ¬p

B  B  B    B              B               B

B  S  S    B              B               S

S  B  B    S              S               B

S  S  B    B              B               B

Dari tabel terlihat jelas bahwa kolom implikasi identik dengan kolom kontraposisi,
tetapi tidak dengan konvers maupun invers.

Implikasi dalam Bahasa Pemrograman

Konsep implikasi sangat erat kaitannya dengan struktur if-then dalam pemrograman.
Pernyataan logika "jika p maka q" diterjemahkan menjadi blok kode seperti:

    y=5
    if suhu > 30:

           y = 10

Di sini, p = kondisi ( suhu > 30 ) dan q = aksi ( y = 10 ). Cara kerja eksekusinya
mencerminkan tabel kebenaran implikasi:

  • Jika kondisi benar, maka blok di dalamnya dieksekusi sehingga nilai y berubah
    menjadi 10.

                          16
  • Jika kondisi salah, blok tidak dilakukan, sehingga nilai y tetap seperti sebelumnya,
    yaitu 5.

Inilah wujud nyata dari "implikasi": aksi hanya terjadi saat syaratnya terpenuhi. Ketika
syarat tidak terpenuhi, tidak ada yang berubah — konsisten dengan baris ketiga dan
keempat tabel kebenaran implikasi yang tetap bernilai benar.

Catatan tentang Bikondisional (Sekilas)

Sebagai pembanding, ada juga bikondisional (bi-implikasi) dengan bentuk "p jika

dan hanya jika q" dan notasi p ↔ q. Bentuk ini setara dengan gabungan dua implikasi:

                                    p ↔ q ⇔ (p → q) ∧ (q → p)

Artinya, "p jika dan hanya jika q" dapat dibaca "jika p maka q, dan jika q maka p". Cara
lain menyatakannya antara lain "p adalah syarat perlu dan cukup untuk q", "jika p
maka q dan sebaliknya", atau "p iff q".
Contoh: "Anda orang kaya jika dan hanya jika anda mempunyai banyak uang, dan
sebaliknya." Konjungsi dua implikasi ini menghasilkan pernyataan bikondisional yang
kuat.

Penutup

Proposisi bersyarat adalah fondasi penting dalam logika, karena ia menjadi dasar bagi
aturan inferensi — aturan yang digunakan untuk membangun suatu argumen yang
valid. Dengan menguasai tabel kebenaran, varian konvers/invers/kontraposisi, serta
kaitannya dengan if-then di pemrograman, kamu sudah memiliki bekal kuat untuk
memahami penalaran logis yang lebih kompleks. Terus berlatih mengubah kalimat
sehari-hari ke bentuk "jika p maka q", ya — semangat!

                                                                               17
Varian Proposisi Bersyarat

Varian Proposisi Bersyarat: Konvers, Invers, dan Kontraposisi

Halo! Setelah sebelumnya kita belajar tentang aturan inferensi (seperti modus ponen,
modus tollen, silogisme hipotetis, dan silogisme disjungtif), sekarang kita akan
menyelami topik yang masih berkaitan erat: varian proposisi bersyarat. Materi ini
penting karena sering muncul saat kita menganalisis keabsahan sebuah argumen.
Yuk, kita pelajari pelan-pelan!
Mengingat Kembali Proposisi Bersyarat

Proposisi bersyarat (implikasi) adalah pernyataan berbentuk "jika p maka q", yang

ditulis secara simbolik sebagai:

                                                   p→q

Di sini, p disebut hipotesis (anteseden), sedangkan q disebut konklusi (konsekuen).
Dari satu implikasi p → q, kita bisa membentuk tiga pernyataan baru yang disebut

varian proposisi bersyarat. Tiga varian tersebut adalah konvers, invers, dan
kontraposisi.
Definisi Konvers, Invers, dan Kontraposisi

  • Konvers diperoleh dengan menukar posisi hipotesis dan konklusi. Jadi, konvers dari

    p → q adalah q → p.

  • Invers diperoleh dengan menegasikan (menambahkan "tidak") pada kedua

    bagian. Jadi, invers dari p → q adalah ∼ p →∼ q.

  • Kontraposisi diperoleh dengan menukar posisi sekaligus menegasikan keduanya.

    Jadi, kontraposisi dari p → q adalah ∼ q →∼ p.

Cara mudah mengingatnya: konvers hanya "menukar", invers hanya "menegasikan",
sedangkan kontraposisi melakukan keduanya.
Tabel Kebenaran Keempat Pernyataan
Kita perlu memeriksa nilai kebenaran setiap varian. Perhatikan tabel berikut dengan
cermat, karena di sinilah letak keunikannya:

                                                                               18
p  q  p→q  Konvers q → p  Invers ∼ p →∼ q  Kontraposisi ∼ q →∼ p

B  B  B    B              B                B

B  S  S    B              B                S

S  B  B    S              S                B

S  S  B    B              B                B

Dari tabel di atas, ada dua fakta menarik yang wajib kamu ingat:

  1. Implikasi selalu ekuivalen dengan kontraposisinya. Perhatikan kolom p → q dan
    kolom kontraposisi — nilainya identik di setiap baris. Jadi, p → q ≡∼ q →∼ p. Inilah

    yang membuat kontraposisi sangat berguna dalam pembuktian.
 2. Konvers selalu ekuivalen dengan invers. Kolom konvers dan kolom invers juga

    identik di setiap baris, sehingga q → p ≡∼ p →∼ q.

Sedangkan hubungan antara implikasi dengan konvers (atau invers) tidak selalu
ekuivalen, sehingga keduanya tidak bisa saling menggantikan begitu saja.

Contoh Menentukan Konvers, Invers, dan Kontraposisi
Agar lebih paham, mari kita kerjakan contoh. Misalkan pernyataan aslinya:

   "Jika n habis dibagi oleh 3, maka n2 habis dibagi oleh 9."

Kita tetapkan p = "n habis dibagi oleh 3" dan q = "n² habis dibagi oleh 9". Maka:
  • Konvers (q → p): "Jika n2 habis dibagi oleh 9, maka n habis dibagi oleh 3."
  • Invers (∼ p →∼ q): "Jika n tidak habis dibagi oleh 3, maka n2 tidak habis dibagi

    oleh 9."

  • Kontraposisi (∼ q →∼ p): "Jika n2 tidak habis dibagi oleh 9, maka n tidak habis

    dibagi oleh 3."
Perhatikan bahwa kontraposisi memiliki makna logis yang sama persis dengan
pernyataan aslinya, sementara konvers dan invers bisa saja berubah nilai
kebenarannya.
Contoh kedua:

                          19
   "Jika saya belajar dengan giat, maka saya lulus ujian."
  • Konvers: "Jika saya lulus ujian, maka saya belajar dengan giat."
  • Invers: "Jika saya tidak belajar dengan giat, maka saya tidak lulus ujian."
  • Kontraposisi: "Jika saya tidak lulus ujian, maka saya tidak belajar dengan giat."
Kaitan dengan Modus Tollen
Nah, inilah jembatan menarik antara materi ini dengan aturan inferensi yang sudah
kamu pelajari. Ingat modus tollen?

                                        [∼ q ∧ (p → q)] →∼ p

Kaidah ini sah justru karena p → q ekuivalen dengan kontraposisinya, ∼ q →∼ p.
Ketika kita tahu ∼ q benar, kita bisa menyimpulkan ∼ p melalui kontraposisi tersebut.

Inilah mengapa memahami varian proposisi bersyarat membuat kita lebih mudah
menerima dan membuktikan validitas modus tollen.
Latihan Mandiri
Coba tentukan konvers, invers, dan kontraposisi dari pernyataan-pernyataan berikut:

  1. "Jika hari ini hujan, maka lalu lintas macet."

 2. "Jika 20 habis dibagi 2, maka 20 adalah bilangan genap."

 3. "Jika saya lulus ujian, maka saya cepat menikah."
Setelah selesai, periksa jawabanmu menggunakan pola berikut:

  • Konvers: tukar hipotesis dan konklusi.
  • Invers: negasikan keduanya tanpa menukar.
  • Kontraposisi: tukar dan negasikan keduanya.
Sebagai contoh penyelesaian untuk nomor 1:
  • Konvers: "Jika lalu lintas macet, maka hari ini hujan."
  • Invers: "Jika hari ini tidak hujan, maka lalu lintas tidak macet."
  • Kontraposisi: "Jika lalu lintas tidak macet, maka hari ini tidak hujan."

                                                                               20
Rangkuman Singkat

Nama               Bentuk        Cara Membentuk
                                 Permis asli
Implikasi          p→q           Menukar posisi
Konvers            q→p           Menegasikan keduanya
Invers             ∼ p →∼ q      Menukar dan menegasikan
Kontraposisi       ∼ q →∼ p

Ingat dua ekuivalensi kuncinya: implikasi ≡ kontraposisi, dan konvers ≡ invers. Dengan

bekal ini, kamu akan lebih mudah menganalisis argumen, membuktikan teorema, dan
menghindari kesalahan berpikir. Selamat berlatih, dan jangan ragu untuk kembali ke
tabel kebenaran setiap kali kamu merasa ragu!

                             21
Bikondisional (Bi-Implikasi)

Apa Itu Proposisi Bikondisional?

Halo, teman-teman! Setelah kita mempelajari implikasi (pernyataan "jika... maka..."),
sekarang saatnya kita berkenalan dengan bikondisional atau bi-implikasi. Ini adalah
salah satu jenis proposisi majemuk yang sangat penting dalam logika matematika,
terutama karena ia menggabungkan dua arah implikasi sekaligus.
Secara sederhana, proposisi bikondisional adalah pernyataan majemuk yang
menyatakan bahwa dua proposisi memiliki nilai kebenaran yang sama. Artinya,
keduanya benar bersama-sama, atau keduanya salah bersama-sama. Tidak boleh
salah satu benar dan yang lain salah.

Definisi dan Notasi
Definisi: Proposisi bikondisional dari proposisi p dan q, ditulis dengan notasi:

                                                   p↔q

dibaca sebagai "p jika dan hanya jika q" (dalam bahasa Inggris: p if and only if q).
Simbol ↔ disebut operator bikondisional. Dalam beberapa buku, Anda mungkin juga
menemukan simbol ⇔ untuk menyatakan hal serupa, namun perhatikan konteks

penggunaannya — yang pertama digunakan untuk membentuk proposisi majemuk,
sedangkan yang kedua sering dipakai untuk menyatakan ekuivalensi logis.
Frasa "jika dan hanya jika" inilah yang membedakan bikondisional dari implikasi biasa.

Implikasi p → q hanya menuntut satu arah ("jika p maka q"), sedangkan bikondisional

menuntut dua arah sekaligus.

Ekuivalensi dengan Implikasi Ganda

Inilah inti dari bikondisional. Ada hubungan yang sangat elegan antara bikondisional
dan implikasi, yaitu:

                                     p ↔ q ≡ (p → q) ∧ (q → p)

                                                                               22
Mari kita bedah maknanya:

  • (p → q) berarti "jika p maka q" — arah maju.
  • (q → p) berarti "jika q maka p" — arah balik (konvers).
  • Tanda ∧ (konjungsi) berarti kedua implikasi tersebut harus benar sekaligus.
Jadi, p ↔ q benar jika dan hanya jika kedua implikasi p → q dan q → p sama-sama

bernilai benar. Jika salah satu saja salah, maka bikondisionalnya salah.

Tabel Kebenaran
Untuk memantapkan pemahaman, mari kita lihat tabel kebenaran bikondisional:

p  q  p→q  q→p      (p → q) ∧ (q → p)  p↔q

B  B  B    B        B                  B

B  S  S    B        S                  S

S  B  B    S        S                  S

S  S  B    B        B                  B

Dari tabel di atas, terlihat jelas pola pentingnya: p ↔ q bernilai benar hanya ketika p
dan q memiliki nilai kebenaran yang sama (baris pertama dan baris terakhir). Itulah

sebabnya mengapa bikondisional sering dianggap sebagai "operator kesamaan nilai
kebenaran".

Cara-cara Menyatakan Bi-Implikasi
Ada beberapa cara mengungkapkan proposisi bikondisional p ↔ q dalam bahasa

sehari-hari, antara lain:

  • "p jika dan hanya jika q" — bentuk paling baku dan paling sering dipakai.

  • "p adalah syarat perlu dan syarat cukup bagi q" — karena kedua arah implikasi
    terpenuhi, maka p menjadi syarat yang perlu sekaligus cukup untuk q.

  • "Jika p maka q, dan jika q maka p" — bentuk eksplisit yang menampakkan kedua

    arah implikasi.

  • "p ekuivalen dengan q" — dalam konteks tertentu, kedua proposisi saling

    menggantikan.

                23
  • "p apabila dan hanya apabila q" — variasi gaya bahasa.

Memahami berbagai cara penyataan ini penting agar kita tidak bingung ketika
menjumpai soal dengan redaksi yang berbeda-beda.

Contoh-contoh Proposisi Majemuk Berbentuk Bi-Implikasi

Mari kita lihat beberapa contoh agar konsep ini semakin konkret.
Contoh 1: "Seorang mahasiswa lulus ujian jika dan hanya jika ia mengerjakan semua
soal dengan benar."

Misalkan p = "Mahasiswa lulus ujian" dan q = "Mahasiswa mengerjakan semua soal
dengan benar". Pernyataan ini berbentuk p ↔ q, yang setara dengan (p → q) ∧ (q →
p):

  • Jika lulus, maka ia mengerjakan semua soal dengan benar.

  • Jika ia mengerjakan semua soal dengan benar, maka ia lulus.
Contoh 2: "Hamid adalah mahasiswa ITB jika dan hanya jika Hamid terdaftar di ITB."

Ini menegaskan bahwa kedua kondisi tersebut saling mengikat dua arah — tidak
mungkin salah satu benar tanpa yang lain.

Contoh 3: "Bilangan n adalah bilangan genap jika dan hanya jika n habis dibagi 2."

Ini adalah contoh klasik bikondisional dalam matematika, di mana definisi dan sifat
saling bertimbal balik.
Contoh 4: "Taslim mengambil kuliah Matematika Diskrit jika dan hanya jika Taslim
terdaftar pada mata kuliah tersebut."

Kedua proposisi ini harus memiliki nilai kebenaran yang sama agar bikondisionalnya
benar.

Mengapa Bikondisional Penting?

Bikondisional memegang peranan besar dalam pembuktian matematika. Ketika kita
ingin membuktikan sebuah teorema berbentuk "jika dan hanya jika", kita wajib

membuktikan dua arah secara terpisah: arah maju (→) dan arah balik (←). Inilah

alasan mengapa pemahaman tentang bikondisional menjadi fondasi penting
sebelum melangkah ke materi argumen dan pembuktian yang lebih kompleks.
Selain itu, dalam konteks kaidah-kaidah penarikan kesimpulan seperti simplifikasi,
penjumlahan, dan konjungsi yang kita pelajari sebelumnya, semua kaidah tersebut
sejatinya dibangun di atas tautologi — dan bikondisional membantu kita memahami

                                                                               24
bahwa kebenaran logis dapat dinyatakan dalam berbagai bentuk yang saling
ekuivalen.

Rangkuman Singkat
  • Bikondisional p ↔ q dibaca "p jika dan hanya jika q".
  • Secara ekuivalen: p ↔ q ≡ (p → q) ∧ (q → p).
  • Bikondisional benar hanya jika p dan q memiliki nilai kebenaran yang sama; salah

    jika keduanya berbeda.
  • Beberapa cara penyataan: "jika dan hanya jika", "syarat perlu dan cukup", "ekuivalen

    dengan".
  • Bikondisional menjadi dasar penting dalam pembuktian dua arah di matematika.
Semoga penjelasan ini membantumu memahami bikondisional dengan lebih baik!
Jangan ragu untuk berlatih membuat tabel kebenaran sendiri agar konsep ini benar-
benar melekat. Selamat belajar!

                                                                               25
Inferensi

Pengantar: Apa Itu Argumen yang Sahih?

Sebelum masuk ke aturan-aturan inferensi, kita perlu menyepakati dulu apa yang
dimaksud dengan argumen yang sahih. Sebuah argumen dikatakan sahih (valid) jika
konklusinya benar bilamana semua hipotesisnya (premis-premisnya) benar.
Sebaliknya, argumen dikatakan palsu — dikenal sebagai fallacy atau invalid.

Jika sebuah argumen sahih, kita bisa mengatakan bahwa secara logika konklusi
mengikuti hipotesis. Cara formal untuk memperlihatkannya adalah dengan
membuktikan bahwa implikasi berikut merupakan tautologi (selalu benar):

(p1  ∧  p    ∧  ⋯   ∧  pn)  →  q

          2

Sebaliknya, argumen yang palsu menunjukkan proses penalaran yang tidak benar —
kesimpulannya bisa saja kebetulan benar, tetapi tidak diharuskan benar oleh premis-
premisnya.

Ada dua cara umum untuk membuktikan kesahihan sebuah argumen:
  1. Tabel kebenaran langsung — periksa apakah pada setiap baris di mana semua
    hipotesis benar, konklusinya juga benar.
 2. Uji tautologi — perlihatkan bahwa bentuk implikasi gabungan dari seluruh premis
    menuju konklusi selalu bernilai benar.

Mari kita pelajari aturan-aturan inferensi satu per satu, lengkap dengan contohnya.

Modus Ponen (Law of Detachment)

Modus ponen adalah aturan inferensi paling dasar dan paling sering dipakai.
Bentuknya:

                                           p → q, p ∴ q

Artinya: jika kita tahu "jika p maka q" dan kita juga tahu bahwa p benar, maka kita boleh
menyimpulkan q.

                26
Contoh. Perhatikan argumen berikut:
  • Jika air laut surut setelah gempa di laut, maka tsunami datang.
  • Air laut surut setelah gempa di laut.
  • Karena itu tsunami datang.

Misalkan p: "Air laut surut setelah gempa di laut" dan q: "Tsunami datang". Argumen ini
berbentuk p → q, p, ∴ q.
Mengapa sahih? Kita bisa memeriksa tabel kebenaran untuk p, q, dan p → q. Argumen

dikatakan sahih jika setiap kali semua hipotesisnya benar, konklusinya benar. Hipotesis

di sini adalah p dan p → q. Keduanya benar bersama-sama hanya pada satu baris,
yaitu ketika p benar dan q benar. Pada baris itu, q juga benar. Jadi argumennya sahih.
Cara kedua: perlihatkan bahwa [p ∧ (p → q)] → q adalah tautologi. Ternyata memang

demikian, sehingga argumen tersebut sahih. Kesimpulannya: modus ponen adalah
argumen yang sahih.

Modus Tollen
Modus tollen bekerja "dari belakang". Jika kita tahu "jika p maka q" tetapi ternyata q
tidak terjadi, maka p pasti tidak terjadi:

                                         p → q, ¬q ∴ ¬p

Contoh.
  • Jika hari ini hujan, maka jalanan basah.
  • Jalanan tidak basah.
  • Karena itu, hari ini tidak hujan.

Perhatikan bahwa modus tollen tidak bisa "dibalik" sembarangan. Dari p → q dan ¬p,
kita tidak boleh menyimpulkan ¬q — itu adalah kekeliruan (fallacy). Modus tollen
hanya sahih bila yang dinegasikan adalah akibat (q).
Silogisme Hipotetis

Silogisme hipotetis merangkai dua implikasi menjadi satu implikasi baru:

                                                                               27
                                     p → q, q → r ∴ p → r

Contoh.
  • Jika saya belajar tekun, maka saya lulus ujian.
  • Jika saya lulus ujian, maka saya mendapat hadiah.
  • Karena itu, jika saya belajar tekun, maka saya mendapat hadiah.

Aturan ini sangat berguna untuk membangun rantai penalaran yang panjang. Selama
implikasi-implikasi tersambung (akibat yang satu menjadi syarat bagi yang
berikutnya), kita dapat "menjahitnya" menjadi satu implikasi tunggal.

Silogisme Disjungtif

Silogisme disjungtif berkaitan dengan pernyataan "atau". Bentuknya:

                                           p ∨ q, ¬p ∴ q

Jika salah satu kemungkinan pada disjungsi terbukti salah, maka kemungkinan lainnya
harus benar.
Contoh. Diberikan dua premis:

  • (i) Logika sulit atau tidak banyak mahasiswa yang menyukai logika.
  • (ii) Jika matematika ... (premis kedua melengkapi penalaran).

Dari premis (i), jika kita mengetahui bahwa "logika sulit" ternyata tidak benar (¬p),

maka kita boleh menyimpulkan bahwa "tidak banyak mahasiswa yang menyukai

logika" (q) adalah benar. Inilah penerapan silogisme disjungtif: menyingkirkan satu opsi

untuk memastikan opsi lainnya.

Simplifikasi

Simplifikasi memungkinkan kita mengambil salah satu bagian dari sebuah konjungsi:

                                               p∧q ∴p

                                                                               28
Jika kita tahu bahwa "keduanya benar", maka masing-masing komponennya pasti
benar. Aturan ini tampak sederhana, tetapi sangat penting saat kita bekerja dengan
premis majemuk.
Contoh.

  • Saya membeli buku dan saya membeli pulpen.

  • Karena itu, saya membeli buku.

Kita juga sah menyimpulkan "saya membeli pulpen". Keduanya valid karena konjungsi
menjamin kebenaran semua komponennya.

Penjumlahan

Penjumlahan (addition) adalah kebalikan semangat simplifikasi: dari satu pernyataan
benar, kita boleh menambahkannya ke pernyataan lain dengan "atau":

                                               p ∴p∨q

Contoh.
  • Hari ini cuaca cerah.
  • Karena itu, hari ini cuaca cerah atau saya pergi ke pantai.

Kesimpulan ini sahih karena dalam disjungsi, cukup satu komponen yang benar agar

seluruh pernyataan bernilai benar. Fakta bahwa q belum diketahui tidak menjadi
masalah — selama p benar, p ∨ q pasti benar.

Konjungsi

Konjungsi menggabungkan dua pernyataan yang masing-masing sudah diketahui
benar menjadi satu konjungsi:

                           p, q ∴ p ∧ q

Contoh.
  • Saya suka matematika.
  • Saya suka logika.

                           29
  • Karena itu, saya suka matematika dan logika.

Aturan ini memungkinkan kita mengemas beberapa fakta menjadi satu premis
gabungan, yang kemudian bisa digunakan bersama aturan lain (misalnya simplifikasi
atau modus ponen).

Ringkasan Aturan Inferensi

Aturan        Bentuk          Contoh Singkat

Modus Ponen   p → q, p ∴ q    Hujan → jalanan basah; hujan ∴ jalanan

                              basah

Modus Tollen  p → q, ¬q ∴ ¬p  Hujan → jalanan basah; jalanan tidak basah ∴
              p → q, q → r ∴
Silogisme     p→r             tidak hujan
Hipotetis
Silogisme     p ∨ q, ¬p ∴ q   Belajar → lulus; lulus → hadiah ∴ belajar →
Disjungtif    p∧q ∴ p
Simplifikasi  p∴p∨q           hadiah
Penjumlahan   p, q ∴ p ∧ q
                              Logika sulit atau tak disukai; tidak sulit ∴ tak
Konjungsi
                              disukai

                              Beli buku dan pulpen ∴ beli buku

                              Cerah ∴ cerah atau ke pantai

                              Suka matematika; suka logika ∴ suka

                              keduanya

Dengan menguasai ketujuh aturan ini, kamu sudah memiliki perangkat dasar untuk
membangun dan memeriksa argumen yang sahih. Ingatlah bahwa kesahihan
argumen bergantung pada bentuk penalarannya, bukan pada isi kebetulan
pernyataannya. Selamat berlatih!

                              30
Argumen

Memahami Argumen dalam Logika

Halo! Senang sekali kamu mau belajar logika sampai di titik ini. Jangan khawatir kalau
awalnya terasa abstrak — argumen itu sebenarnya cuma cara rapi untuk berpikir. Yuk
kita bedah pelan-pelan.

Apa Itu Argumen?
Dalam logika, argumen bukan berarti "pertengkaran", melainkan deret proposisi yang
terdiri dari dua bagian:

• Hipotesis (premis): satu atau lebih proposisi yang dijadikan dasar atau asumsi.

Dilambangkan  dengan       p    ,  p2,  …    ,  pn   .

                             1

• Konklusi (kesimpulan): proposisi tunggal q yang ditarik dari premis-premis

tersebut.

Pola umumnya seperti ini:

                                        p1,     p    ,  …,  pn  ∴  q

                                                  2

Contoh sederhana dari materi:

   Premis 1: Jika matematika mudah, maka logika tidak sulit. Premis 2: Matematika
   mudah. Konklusi: Logika tidak sulit.

Argumen ini tersusun rapi: ada dua premis dan satu konklusi yang diklaim
mengikutinya.

Argumen Sahih vs. Argumen Palsu
Inilah inti pembahasan kita. Perhatikan bahwa kesahihan argumen tidak bergantung
pada benar-salahnya isi pernyataan, melainkan pada hubungan logis antara premis
dan konklusi.

  • Argumen sahih (valid): argumen di mana konklusi pasti benar jika semua
    premisnya benar. Tidak mungkin premis benar semua tetapi konklusi salah.

                                                        31
  • Argumen palsu (invalid / fallacy): argumen di mana konklusi belum tentu benar
    meskipun semua premis benar. Ada kemungkinan premisnya benar tetapi
    konklusinya salah.

Kunci penting: Sebuah argumen bisa punya premis yang faktanya salah, tetapi tetap
sahih secara struktur. Sebaliknya, argumen dengan premis benar semua bisa tetap
palsu kalau konklusinya tidak benar-benar mengikuti.

Jembatan ke Konsep Implikasi
Bagaimana cara mengubah "penilaian kesahihan" menjadi perhitungan yang bisa

diuji? Kita gabungkan semua premis dengan konjungsi (∧), lalu hubungkan ke konklusi
dengan implikasi (→):

                            (p1    ∧  p    ∧  ⋯   ∧  pn)  →  q

                                        2

Aturan emasnya:

Argumen  sahih   jika  dan  hanya  jika  proposisi   (p1  ∧  p    ∧  ⋯  ∧  pn)  →  q  adalah

                                                               2

tautologi — yaitu selalu bernilai benar pada semua kombinasi nilai kebenaran

variabelnya.

Tautologi inilah yang menjadi bukti formal bahwa argumen tersebut sahih. Jika ada
satu saja baris yang bernilai salah, argumen itu palsu.

Metode 1: Membuktikan Kesahihan dengan Tabel Kebenaran

Tabel kebenaran mengecek semua kombinasi nilai B (benar) dan S (salah). Mari kita

uji contoh di atas:

Misalkan:

  • p: Matematika mudah.
  • q: Logika sulit. (Maka "logika tidak sulit" adalah ¬q.)
Premis 1: p → ¬q Premis 2: p Konklusi: ¬q
Bentuk implikasinya: ((p → ¬q) ∧ p) → ¬q

p  q             ¬q         p → ¬q                (p → ¬q) ∧ p                  Implikasi total

                                              32
B  B  S  S      S  B

B  S  B  B      B  B

S  B  S  B      S  B

S  S  B  B      S  B

Karena kolom terakhir seluruhnya B, maka ekspresi tersebut adalah tautologi,
sehingga argumennya sahih. Perhatikan baris kedua — baris di mana semua premis

benar (p benar dan p → ¬q benar) — konklusinya juga benar.

Metode 2: Membuktikan dengan Menunjukkan Tautologi
Selain tabel penuh, kita bisa membuktikannya lewat penalaran langsung
menggunakan sifat-sifat logika.

Langkah 1. Perhatikan bentuk argumen ini persis mengikuti Modus Ponens:

                                          p → ¬q, p ∴ ¬q

Langkah 2. Kita tunjukkan bahwa ((p → ¬q) ∧ p) → ¬q selalu benar. Ekspresi ini
berstruktur (A ∧ C) → D dengan A = p → ¬q, C = p, dan D = ¬q. Karena Modus
Ponens adalah pola implikasi yang sudah dikenal sahih, maka konjungsinya dengan p

selalu mengarah ke konklusi yang benar — membuktikan bahwa ekspresi itu tautologi
tanpa perlu menuliskan seluruh tabel.
Langkah 3. Karena ekspresi tersebut tautologi, maka argumennya sahih.
Metode ini lebih cepat, tetapi kita harus yakin pola logisnya benar. Tabel kebenaran
adalah pembuktian paling meyakinkan karena memeriksa semua kemungkinan.
Menganalisis Konklusi dari Premis
Sekarang kita terapkan pada latihan. Diberikan dua premis:

   Premis 1: Jika matematika mudah, maka logika tidak sulit. Premis 2: Matematika
   mudah.

Kita lambangkan: p = matematika mudah, q = logika sulit.

            33
(a) Konklusi: "Matematika tidak mudah atau logika sulit."

Bentuknya ¬p ∨ q, yang menurut hukum implikasi setara dengan p → q.
Apakah ((p → ¬q) ∧ p) → (p → q) sebuah tautologi? Uji dengan baris kritis: ambil p =
B, q = B.

  • Premis 1: p → ¬q = B → S = S. (premis tidak semuanya benar)
  • Premis 2: p = B.

  • Konjungsi premis = S.

  • Konklusi p → q = B → B = B.

  • Implikasi total = S → B = B. ✓
Ambil p = B, q = S (di sini semua premis benar):

  • p → ¬q = B → B = B, p = B, konjungsi = B.
  • Konklusi p → q = B → S = S.
  • Implikasi total = B → S = S. ✗

Karena ada baris yang bernilai salah, konklusi (a) tidak sah (palsu). Memang, konklusi
ini bertentangan dengan yang seharusnya.
(b) Konklusi: "Matematika tidak mudah, jika banyak mahasiswa menyukai logika."

Misalkan r = banyak mahasiswa menyukai logika. Konklusinya berbentuk r → ¬p.
Sekarang, apakah r muncul di premis? Tidak! Premis hanya berbicara tentang p dan q.
Karena r bisa bernilai benar atau salah bebas, kita bisa membuat konklusi menjadi
salah. Ambil r = B dan p = B (premis benar), maka r → ¬p = B → S = S. Jadi implikasi
total menjadi B → S = S, yang berarti tidak sah. Variabel yang tidak muncul di premis

tidak bisa disimpulkan.

Rangkuman Cepat

Konsep           Penjelasan Singkat

Argumen          Deret  proposisi:  premis  p    …  pn  menuju  konklusi  q
Sahih (valid)
                                              1

                 Konklusi pasti benar bila semua premis benar

Palsu (invalid)  Ada kemungkinan premis benar semua tapi konklusi salah

                                    34
Uji tautologi  (p1 ∧ ⋯ ∧ pn) → q harus selalu B
Alat uji
               Tabel kebenaran atau pembuktian pola logis

Kesimpulan

Menguji kesahihan argumen itu seperti menjadi detektif: kita periksa apakah konklusi
benar-benar "dipaksa" oleh premis. Kuncinya adalah mengubah argumen menjadi
implikasi tunggal, lalu mengecek apakah ia tautologi. Jika ya — sahih! Jika ada satu
saja kemungkinan yang membuatnya salah — palsu. Dengan latihan rutin, matamu
akan makin tajam mengenali argumen yang sah dan yang menyesatkan. Selamat
berlatih!

               35
