# EMT_Annisa Nur Rohmah_22305141031
Nama    : Annisa Nur Rohmah


NIM     : 22305141031


Kelas   : Matematika E


---

# Pendahuluan dan Pengenalan Cara Kerja EMT

Selamat datang! Ini adalah pengantar pertama ke Euler Math Toolbox
(disingkat EMT atau Euler). EMT adalah sistem terintegrasi yang
merupakan perpaduan kernel numerik Euler dan program komputer aljabar
Maxima.


* 
Bagian numerik, GUI, dan komunikasi dengan Maxima telah dikembangkan
* oleh R. Grothmann, seorang profesor matematika di Universitas
* Eichstätt, Jerman. Banyak algoritma numerik dan pustaka software open
* source yang digunakan di dalamnya.


* 
Maxima adalah program open source yang matang dan sangat kaya untuk
* perhitungan simbolik dan aritmatika tak terbatas. Software ini
* dikelola oleh sekelompok pengembang di internet.


* 
Beberapa program lain (LaTeX, Povray, Tiny C Compiler, Python) dapat
* digunakan di Euler untuk memungkinkan perhitungan yang lebih cepat
* maupun tampilan atau grafik yang lebih baik.


Yang sedang Anda baca (jika dibaca di EMT) ini adalah berkas notebook
di EMT. Notebook aslinya bawaan EMT (dalam bahasa Inggris) dapat
dibuka melalui menu File, kemudian pilih "Open Tutorias and Example",
lalu pilih file "00 First Steps.en". Perhatikan, file notebook EMT
memiliki ekstensi ".en". Melalui notebook ini Anda akan belajar
menggunakan software Euler untuk menyelesaikan berbagai masalah
matematika.


Panduan ini ditulis dengan Euler dalam bentuk notebook Euler, yang
berisi teks (deskriptif), baris-baris perintah, tampilan hasil
perintah (numerik, ekspresi matematika, atau gambar/plot), dan gambar
yang disisipkan dari file gambar.


Untuk menambah jendela EMT, Anda dapat menekan [F11]. EMT akan
menampilkan jendela grafik di layar desktop Anda. Tekan [F11] lagi
untuk kembali ke tata letak favorit Anda. Tata letak disimpan untuk
sesi berikutnya.


Anda juga dapat menggunakan [Ctrl]+[G] untuk menyembunyikan jendela
grafik. Selanjutnya Anda dapat beralih antara grafik dan teks dengan
tombol [TAB].


Seperti yang Anda baca, notebook ini berisi tulisan (teks) berwarna
hijau, yang dapat Anda edit dengan mengklik kanan teks atau tekan menu
Edit -&gt; Edit Comment atau tekan [F5], dan juga baris perintah EMT yang
ditandai dengan "&gt;" dan berwarna merah. Anda dapat menyisipkan baris
perintah baru dengan cara menekan tiga tombol bersamaan:
[Shift]+[Ctrl]+[Enter].


## Komentar (Teks Uraian)

Komentar atau teks penjelasan dapat berisi beberapa "markup" dengan
sintaks sebagai berikut.


   - * Judul  
   - ** Sub-Judul  
   - latex: F (x) = \int_a^x f (t) \, dt  
   - mathjax: \frac{x^2-1}{x-1} = x + 1  
   - maxima: 'integrate(x^3,x) = integrate(x^3,x) + C  
   - http://www.euler-math-toolbox.de  
   - See: http://www.google.de | Let's Go to Google  
   - image: Aomine Daiki.jpg  
   - ---  

Hasil sintaks-sintaks di atas (tanpa diawali tanda strip) adalah
sebagai berikut.


# Judul

## Sub-Judul

$$F (x) = \int_a^x f(t) \, dt$$$$\frac{x^2-1}{x-1} = x + 1$$
$$\int {x^3}{\;dx}=C+\frac{x^4}{4}$$  <a href="http://www.euler-math-toolbox.de">http://www.euler-math-toolbox.de</a>  

  <a href="http://www.google.de">Let's Go to Google</a>  

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-004.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-004.png)

---

Gambar diambil dari folder images di tempat file notebook berada dan
tidak dapat dibaca dari Web. Untuk "See:", tautan (URL)web lokal dapat
digunakan.


Paragraf terdiri atas satu baris panjang di editor. Pergantian baris
akan memulai baris baru. Paragraf harus dipisahkan dengan baris
kosong.


\>// baris perintah diawali dengan \>, komentar (keterangan) diawali dengan //


# Baris Perintah

Mari kita tunjukkan cara menggunakan EMT sebagai kalkulator yang
sangat canggih.


EMT berorientasi pada baris perintah. Anda dapat menuliskan satu atau
lebih perintah dalam satu baris perintah. Setiap perintah harus
diakhiri dengan koma atau titik koma.


* 
Titik koma menyembunyikan output (hasil) dari perintah.

* 
Sebuah koma mencetak hasilnya.

* 
Setelah perintah terakhir, koma diasumsikan secara otomatis (boleh
* tidak ditulis).


Dalam contoh berikut, kita mendefinisikan variabel r yang diberi nilai
1,25. Output dari definisi ini adalah nilai variabel. Tetapi karena
tanda titik koma, nilai ini tidak ditampilkan. Pada kedua perintah di
belakangnya, hasil kedua perhitungan tersebut ditampilkan.


\>r=1.25; pi\*r^2, 2\*pi\*r


    4.90873852123
    7.85398163397

## Latihan untuk Anda

* 
Sisipkan beberapa baris perintah baru

* 
Tulis perintah-perintah baru untuk melakukan suatu perhitungan yang
* Anda inginkan, boleh menggunakan variabel, boleh tanpa variabel.


## Jawab

\> 3\*5 + 3, 100/3 - 15, frac(100/3 - 15)


    18
    18.3333333333
    55/3

\> n = -2; -3n^3-6n^2, cos(-3n^3-6n^2)


    0
    1

---



Beberapa catatan yang harus Anda perhatikan tentang penulisan sintaks
perintah EMT.


* 
Pastikan untuk menggunakan titik desimal, bukan koma desimal untuk
* bilangan!

* 
Gunakan * untuk perkalian dan ^ untuk eksponen (pangkat).

* 
Seperti biasa, * dan / bersifat lebih kuat daripada + atau -.

* 
^ mengikat lebih kuat dari *, sehingga pi * r ^ 2 merupakan rumus
* luas lingkaran.

* 
Jika perlu, Anda harus menambahkan tanda kurung, seperti pada 2 ^ (2
* ^ 3).


Perintah r = 1.25 adalah menyimpan nilai ke variabel di EMT. Anda juga
dapat menulis r: = 1.25 jika mau. Anda dapat menggunakan spasi sesuka
Anda.


Anda juga dapat mengakhiri baris perintah dengan komentar yang diawali
dengan dua garis miring (//).


\>r := 1.25 // Komentar: Menggunakan  := sebagai ganti =


    1.25

Argumen atau input untuk fungsi ditulis di dalam tanda kurung.


\>sin(45°), cos(pi), log(sqrt(E))


    0.707106781187
    -1
    0.5

Seperti yang Anda lihat, fungsi trigonometri bekerja dengan radian,
dan derajat dapat diubah dengan °. Jika keyboard Anda tidak memiliki
karakter derajat tekan [F7], atau gunakan fungsi deg() untuk
mengonversi.


EMT menyediakan banyak sekali fungsi dan operator matematika.Hampir
semua fungsi matematika sudah tersedia di EMT. Anda dapat melihat
daftar lengkap fungsi-fungsi matematika di EMT pada berkas Referensi
(klik menu Help -&gt; Reference)


Untuk membuat rangkaian komputasi lebih mudah, Anda dapat merujuk ke
hasil sebelumnya dengan "%". Cara ini sebaiknya hanya digunakan untuk
merujuk hasil perhitungan dalam baris perintah yang sama.


\>(sqrt(5)+1)/2, %^2-%+1 // Memeriksa solusi x^2-x+1=0


    1.61803398875
    2

## Latihan untuk Anda

* 
Buka berkas Reference dan baca fungsi-fungsi matematika yang
* tersedia di EMT.

* 
Sisipkan beberapa baris perintah baru.

* 
Lakukan contoh-contoh perhitungan menggunakan fungsi-fungsi
* matematika di EMT.


## Jawab

\> factor(gcd(12,60)), lcm(12,60)


    [2,  2,  3]
    60

\> [1:10], isprime(1:10), primes(10), sum(isprime(1:10)), sum(primes(10))


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10]
    [0,  1,  1,  0,  1,  0,  1,  0,  0,  0]
    [2,  3,  5,  7]
    4
    17

---

# Satuan

EMT dapat mengubah unit satuan menjadi sistem standar internasional
(SI). Tambahkan satuan di belakang angka untuk konversi sederhana.


\>1miles  // 1 mil = 1609,344 m


    1609.344

Beberapa satuan yang sudah dikenal di dalam EMT adalah sebagai
berikut. Semua unit diakhiri dengan tanda dolar ($), namun boleh tidak
perlu ditulis dengan mengaktifkan easyunits.


kilometer$:=1000;


km$:=kilometer$;


cm$:=0.01;


mm$:=0.001;


minute$:=60;


min$:=minute$;


minutes$:=minute$;


hour$:=60*minute$;


h$:=hour$;


hours$:=hour$;


day$:=24*hour$;


days$:=day$;


d$:=day$;


year$:=365.2425*day$;


years$:=year$;


y$:=year$;


inch$:=0.0254;


in$:=inch$;


feet$:=12*inch$;


foot$:=feet$;


ft$:=feet$;


yard$:=3*feet$;


yards$:=yard$;


yd$:=yard$;


mile$:=1760*yard$;


miles$:=mile$;


kg$:=1;


sec$:=1;


ha$:=10000;


Ar$:=100;


Tagwerk$:=3408;


Acre$:=4046.8564224;


pt$:=0.376mm;


Untuk konversi ke dan antar unit, EMT menggunakan operator khusus,
yakni -&gt;.


\>4km -\> miles, 4inch -\> " mm", 1m -\> km, 1km -\> m, 1000mm -\> km, 1h, 1h \* 24, 1d


    2.48548476895
    101.6 mm
    0.001
    1000
    0.001
    3600
    86400
    86400

# Format Tampilan Nilai

Akurasi internal untuk nilai bilangan di EMT adalah standar IEEE,
sekitar 16 digit desimal. Aslinya, EMT tidak mencetak semua digit
suatu bilangan. Ini untuk menghemat tempat dan agar terlihat lebih
baik. Untuk mengatrtamilan satu bilangan, operator berikut dapat
digunakan.


\>pi


    3.14159265359

\>longest pi


          3.141592653589793 

\>long pi


    3.14159265359

\>short pi


    3.1416

\>shortest pi


       3.1 

\>fraction pi


    312689/99532

\>short 1200\*1.03^10, long E, longest pi


    1612.7
    2.71828182846
          3.141592653589793 

Format aslinya untuk menampilkan nilai menggunakan sekitar 10 digit.
Format tampilan nilai dapat diatur secara global atau hanya untuk satu
nilai.


Anda dapat mengganti format tampilan bilangan untuk semua perintah
selanjutnya. Untuk mengembalikan ke format aslinya dapat digunakan
perintah "defformat" atau "reset".


\>longestformat; pi, 100/7, longformat; pi, 100/7, defformat; pi, 100/7, ...  
\>   shortest pi, shortest 100/7, shortest 10/7


    3.141592653589793
    14.28571428571429
    3.14159265359
    14.2857142857
    3.14159265359
    14.2857142857
       3.1 
        14 
       1.4 

Kernel numerik EMT bekerja dengan bilangan titik mengambang (floating
point) dalam presisi ganda IEEE (berbeda dengan bagian simbolik EMT).
Hasil numerik dapat ditampilkan dalam bentuk pecahan.


\>1/7+1/4, fraction %, frac(1/7+1/4)


    0.392857142857
    11/28
    11/28

# Perintah Multibaris

Perintah multi-baris membentang di beberapa baris yang terhubung
dengan "..." di setiap akhir baris, kecuali baris terakhir. Untuk
menghasilkan tanda pindah baris tersebut, gunakan tombol
[Ctrl]+[Enter]. Ini akan menyambung perintah ke baris berikutnya dan
menambahkan "..." di akhir baris sebelumnya. Untuk menggabungkan suatu
baris ke baris sebelumnya, gunakan [Ctrl]+[Backspace].


Contoh perintah multi-baris berikut dapat dijalankan setiap kali
kursor berada di salah satu barisnya. Ini juga menunjukkan bahwa ...
harus berada di akhir suatu baris meskipun baris tersebut memuat
komentar.


\>a=4; b=15; c=2; // menyelesaikan a\*x^2+b\*x+c=0 secara manual ...  
\>   D=sqrt(b^2/(a^2\*4)-c/a); ...  
\>   -b/(2\*a) + D, ...  
\>   -b/(2\*a) - D


    -0.138444501319
    -3.61155549868

\>a=4; b=15; c=2; // menyelesaikan a\*x^2+b\*x+c=0 secara manual  ...  
\>   D=sqrt(b^2/(a^2\*4)-c/a), D


    1.73655549868
    1.73655549868

# Menampilkan Daftar Variabel

Untuk menampilkan semua variabel yang sudah pernah Anda definisikan
sebelumnya (dan dapat dilihat kembali nilainya), gunakan perintah
"listvar".


\>listvar


    r                   1.25
    n                   -2
    a                   4
    b                   15
    c                   2
    D                   1.73655549868123

Perintah listvar hanya menampilkan variabel buatan pengguna.
Dimungkinkan untuk menampilkan variabel lain, dengan menambahkan
string  termuat di dalam nama variabel yang diinginkan.


Perlu Anda perhatikan, bahwa EMT membedakan huruf besar dan huruf
kecil. Jadi variabel "d" berbeda dengan variabel "D".


Contoh berikut ini menampilkan semua unit yang diakhiri dengan "m"
dengan mencari semua variabel yang berisi "m$".


\>listvar m$


    km$                 1000
    cm$                 0.01
    mm$                 0.001
    nm$                 1853.24496
    gram$               0.001
    m$                  1
    hquantum$           6.62606957e-34
    atm$                101325

\>listvar m$, listvar s$


    No variable containing m$, found.
    englishmonths$      Type: String Vector
    minutes$            60
    tons$               1000
    hours$              3600
    days$               86400
    years$              31556952
    yards$              0.9144
    miles$              1609.344
    kts$                0.514790266666667
    Rgas$               8.3144621
    electronmass$       9.10938291e-31
    protonmass$         1.672621777e-27
    neutronmass$        1.674927351e-27
    mumass$             0.001
    calories$           4.1868

Untuk menghapus variabel tanpa harus memulai ulang EMT gunakan
perintah "remvalue".


\>remvalue a,b,c,D

\>D


    Variable D not found!
    Error in:
    D ...
     ^

# Menampilkan Panduan

Untuk mendapatkan panduan tentang penggunaan perintah atau fungsi di
EMT, buka jendela panduan dengan menekan [F1] dan cari fungsinya. Anda
juga dapat mengklik dua kali pada fungsi yang tertulis di baris
perintah atau di teks untuk membuka jendela panduan.


Coba klik dua kali pada perintah "intrandom" berikut ini!


\>intrandom(10), intrandom(10)


    7
    3

\>intrandom(10,6), intrandom(6,10) ...  
\>   //(a,b), a=banyak bilangan, b=rentang bil. acak


    [6,  2,  4,  2,  3,  2,  2,  6,  2,  5]
    [3,  5,  4,  10,  2,  5]

\>intrandom(6,5,10), intrandom(3,10,25) ...  
\>   //(a,b,c)=([a,b],c), a=baris, b=kolom, c=rentang bil. acak


                1             6             5             8             5 
                4             6             6             2             3 
                9             6             5             7             7 
               10             2            10             1            10 
                1             4             6             5             2 
                2             3             8             5             4 
    Real 3 x 10 matrix
    
                9             5            12             6     ...
               23            10            17             2     ...
                3            16             6            25     ...

\>intrandom([6,5],10) //([a,b],c), a=baris, b=kolom, c=rentang bil. acak


                2             5             8             3             9 
                5             4             8             4             3 
                1             2             4             5             4 
                4             2             6             9            10 
               10             1             4             2             3 
               10             5             2             1             2 

Di jendela panduan, Anda dapat mengklik kata apa saja untuk menemukan
referensi atau fungsi.


Misalnya, coba klik kata "random" di jendela panduan. Kata tersebut
boleh ada dalam teks atau di bagian "See:" pada panduan. Anda akan
menemukan penjelasan fungsi "random", untuk menghasilkan bilangan acak
berdistribusi uniform antara 0,0 dan 1,0. Dari panduan untuk "random"
Anda dapat menampilkan panduan untuk fungsi "normal", dll.


\>random()


    0.777527902317

\>random(10) // mencetak 0<bil. acak<1 10 kali


    [0.237424,  0.978964,  0.0367821,  0.191109,  0.642479,  0.233536,
    0.0910807,  0.899334,  0.983636,  0.21102]

\>random(3,2), random([2,1]) //(a,b)=([a,b]), a=baris, b=kolom


         0.552777      0.494142 
         0.579784      0.811875 
         0.983877      0.262956 
         0.993804 
         0.901832 

\>normal(10), normal(6)


    [-1.29602,  0.679832,  -0.640637,  -0.456261,  -0.743291,  1.16909,
    -2.07702,  1.35647,  0.239489,  -0.471085]
    [-1.35778,  -1.10799,  -1.6828,  -1.89383,  -0.210226,  -1.07112]

# Matriks dan Vektor

EMT merupakan suatu aplikasi matematika yang mengerti "bahasa
matriks". Artinya, EMT menggunakan vektor dan matriks untuk
perhitungan-perhitungan tingkat lanjut. Suatu vektor atau matriks
dapat didefinisikan dengan tanda kurung siku. Elemen-elemennya
dituliskan di dalam tanda kurung siku, antar elemen dalam satu baris
dipisahkan oleh koma(,), antar baris dipisahkan oleh titik koma (;).


Vektor dan matriks dapat diberi nama seperti variabel biasa.


\>v=[4,5,6,3,2,1]


    [4,  5,  6,  3,  2,  1]

\>A=[1,2,3;4,5,6;7,8,9]


                1             2             3 
                4             5             6 
                7             8             9 

Karena EMT mengerti bahasa matriks, EMT memiliki kemampuan yang sangat
canggih untuk melakukan perhitungan matematis untuk masalah-masalah
aljabar linier, statistika, dan optimisasi.


Vektor juga dapat didefinisikan dengan menggunakan rentang nilai
dengan interval tertentu menggunakan tanda titik dua (:),seperti
contoh berikut ini.


\>c=1:5


    [1,  2,  3,  4,  5]

\>w=0:0.1:1, p=1:3:20


    [0,  0.1,  0.2,  0.3,  0.4,  0.5,  0.6,  0.7,  0.8,  0.9,  1]
    [1,  4,  7,  10,  13,  16,  19]

\>mean(w^2), w^2, sum(%), sum(w^2), %/11


    0.35
    [0,  0.01,  0.04,  0.09,  0.16,  0.25,  0.36,  0.49,  0.64,  0.81,  1]
    3.85
    3.85
    0.35

# Bilangan Kompleks

EMT juga dapat menggunakan bilangan kompleks. Tersedia banyak fungsi
untuk bilangan kompleks di EMT. Bilangan imaginer


 -inputnya =&gt;  latex: i = \sqrt{-1}  
 -outputnya :  

$$i = \sqrt{-1}$$dituliskan dengan huruf I (huruf besar I), namun akan ditampilkan
dengan huruf i (i kecil).


  re(x) : bagian riil pada bilangan kompleks x.  
  im(x) : bagian imaginer pada bilangan kompleks x.  
  complex(x) : mengubah bilangan riil x menjadi bilangan kompleks.  
  conj(x) : Konjugat untuk bilangan bilangan komplkes x.  
  arg(x) : argumen (sudut dalam radian) bilangan kompleks x.  
  real(x) : mengubah x menjadi bilangan riil.  

Apabila bagian imaginer x terlalu besar, hasilnya akan menampilkan
pesan kesalahan.


  &gt;sqrt(-1) // Error!  
  &gt;sqrt(complex(-1))  

\>sqrt(complex(-1)), z=2+3\*I, re(z), im(z), conj(z), arg(z),  ...  
\>   deg(arg(z)), deg(arctan(3/2))


    0+1i
    2+3i
    2
    3
    2-3i
    0.982793723247
    56.309932474
    56.309932474

\>deg(arg(I)) // 90°


    90

\>sqrt(-1)


    Floating point error!
    Error in sqrt
    Error in:
    sqrt(-1) ...
            ^

\>sqrt(complex(-1))


    0+1i

EMT selalu menganggap semua hasil perhitungan berupa bilangan riil dan
tidak akan secara otomatis mengubah ke bilangan kompleks.


Jadi akar kuadrat -1 akan menghasilkan kesalahan, tetapi akar kuadrat
kompleks didefinisikan untuk bidang koordinat dengan cara seperti
biasa. Untuk mengubah bilangan riil menjadi kompleks, Anda dapat
menambahkan 0i atau menggunakan fungsi "complex".


\>complex(-1), sqrt(%)


    -1+0i 
    0+1i

# Matematika Simbolik

EMT dapat melakukan perhitungan matematika simbolis (eksak) dengan
bantuan software Maxima. Software Maxima otomatis sudah terpasang di
komputer Anda ketika Anda memasang EMT. Meskipun demikian, Anda dapat
juga memasang software Maxima tersendiri (yang terpisah dengan
instalasi Maxima di EMT).


Pengguna Maxima yang sudah mahir harus memperhatikan bahwa terdapat
sedikit perbedaan dalam sintaks antara sintaks asli Maxima dan sintaks
ekspresi simbolik di EMT.


Untuk melakukan perhitungan matematika simbolis di EMT, awali perintah
Maxima dengan tanda "&amp;". Setiap ekspresi yang dimulai dengan "&amp;"
adalah ekspresi simbolis dan dikerjakan oleh Maxima.


\>&(a+b)^2 //masih belum tahu cara menampilkan a nya dulu


    
                                          2
                                   (b + a)
    

\>&expand((a+b)^2), &factor(x^2+5\*x+6)  ...  
\>   //masih belum tahu cara menampilkan a nya dulu


    
                                2            2
                               b  + 2 a b + a
    
    
                               (x + 2) (x + 3)
    

\>&solve(a\*x^2+b\*x+c,x) // rumus abc


    
                         2                         2
                 - sqrt(b  - 4 a c) - b      sqrt(b  - 4 a c) - b
            [x = ----------------------, x = --------------------]
                          2 a                        2 a
    

\>&(a^2-b^2)/(a+b), &ratsimp(%) // ratsimp menyederhanakan bentuk pecahan


    
                                    2    2
                                   a  - b
                                   -------
                                    b + a
    
    
                                    a - b
    

\>10! // nilai faktorial (modus EMT)


    3628800

\>&10! //nilai faktorial (simbolik dengan Maxima)


    
                                   3628800
    

Untuk menggunakan perintah Maxima secara langsung (seperti perintah
pada layar Maxima) awali perintahnya dengan tanda "::" pada baris
perintah EMT. Sintaks Maxima disesuaikan dengan sintaks EMT (disebut
"modus kompatibilitas").


\>factor(1000) // mencari semua faktor 1000 (EMT)


    [2,  2,  2,  5,  5,  5]

\>:: factor(1000) // faktorisasi prima 1000 (dengan Maxima) 


    
                                     3  3
                                    2  5
    

\>:: factor(20!)


    
                            18  8  4  2
                           2   3  5  7  11 13 17 19
    

Jika Anda sudah mahir menggunakan Maxima, Anda dapat menggunakan
sintaks asli perintah Maxima dengan menggunakan tanda ":::" untuk
mengawali setiap perintah Maxima di EMT. Perhatikan, harus ada spasi
antara ":::" dan perintahnya.


\>::: binomial(5,2); // nilai C(5,2)


    
                                      10
    

\>::: binomial(m,4); // C(m,4)=m!/(4!(m-4)!)


    
                          (m - 3) (m - 2) (m - 1) m
                          -------------------------
                                     24
    

\>::: trigexpand(cos(x+y)); // rumus cos(x+y) = cos(x)cos(y) - sin(x)sin(y) 


    
                        cos(x) cos(y) - sin(x) sin(y)
    

\>::: trigexpand(sin(x+y));


    
                        cos(x) sin(y) + sin(x) cos(y)
    

\>::: trigsimp(((1-sin(x)^2)\*cos(x))/cos(x)^2+tan(x)\*sec(x)^2) //mnyderhnakn fungsi trig


    
                                           4
                               sin(x) + cos (x)
                               ----------------
                                      3
                                   cos (x)
    

Untuk menyimpan ekspresi simbolik ke dalam suatu variabel digunakan tanda "&amp;=".


\>p1 &= (x^3+1)/(x+1)


    
                                     3
                                    x  + 1
                                    ------
                                    x + 1
    

\>&ratsimp(p1) //'simp' itu kayak menyederhanakan


    
                                   2
                                  x  - x + 1
    

Untuk mensubstitusikan suatu nilai ke dalam variabel dapat digunakan perintah
"with".


\>&p1 with x=3 // (3^3+1)/(3+1)


    
                                      7
    

\>&p1 with x=a+b, &ratsimp(%) //substitusi dengan variabel baru dan  ...  
\>   masih belum tahu cara menampilkan a nya dulu


    
                                        3
                                 (b + a)  + 1
                                 ------------
                                  b + a + 1
    
    
                         2                  2
                        b  + (2 a - 1) b + a  - a + 1
    

\>&diff(p1,x) //turunan p1 terhadap x


    
                                  2      3
                               3 x      x  + 1
                               ----- - --------
                               x + 1          2
                                       (x + 1)
    

\>&integrate(p1,x) // integral p1 terhadap x


    
                                 3      2
                              2 x  - 3 x  + 6 x
                              -----------------
                                      6
    

# Tampilan Matematika Simbolik dengan LaTeX

Anda dapat menampilkan hasil perhitunagn simbolik secara lebih bagus
menggunakan LaTeX. Untuk melakukan hal ini, tambahkan tanda dolar ($)
di depan tanda &amp; pada setiap perintah Maxima.


Perhatikan, hal ini hanya dapat menghasilkan tampilan yang diinginkan
apabila komputer Anda sudah terpasang software LaTeX.


\>$&(a+b)^2


$$\left(b+a\right)^2$$\>$&expand((a+b)^2), $&factor(x^2+5\*x+6)


$$\left(x+2\right)\,\left(x+3\right)$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-008.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-008.png)

\>$&solve(a\*x^2+b\*x+c,x) // rumus abc


$$\left[ x=\frac{-\sqrt{b^2-4\,a\,c}-b}{2\,a} , x=\frac{\sqrt{b^2-4\,  a\,c}-b}{2\,a} \right] $$\>$&(a^2-b^2)/(a+b), $&ratsimp(%)


$$a-b$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-011.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-011.png)

# Selamat Belajar dan Berlatih!

Baik, itulah sekilas pengantar penggunaan software EMT. Masih banyak
kemampuan EMT yang akan Anda pelajari dan praktikkan.


Sebagai latihan untuk memperlancar penggunaan perintah-perintah EMT
yang sudah dijelaskan di atas, silakan Anda lakukan hal-hal sebagai
berikut.


* 
Carilah soal-soal matematika dari buku-buku Matematika.

* 
Tambahkan beberapa baris perintah EMT pada notebook ini.

* 
Selesaikan soal-soal matematika tersebut dengan menggunakan EMT.
* Pilih soal-soal yang sesuai dengan perintah-perintah yang sudah
* dijelaskan dan dicontohkan di atas.


\>plot3d("y^2-x^2", angle=145°, grid=15) : //kalkuls purcell edisi 9 jilid 2 hal 236


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-012.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-012.png)

\>plot2d("(x^2)/3+(sin(x))^3", -10, 10) : //coba-coba


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-013.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-013.png)

\>&integrate(1/(x-1)^(2/3),x), &integrate(1/(x-1)^(2/3),x,0,3),  ...  
\>   $&integrate(1/(x-1)^(2/3),x,0,3)  //kalkulus purcell edisi 9 jilid 2 hal 62


    
                                          1/3
                                 3 (x - 1)
    
    
                                     1/3
                                  3 2    + 3
    

$$3\,2^{\frac{1}{3}}+3$$---

---

---

# EMT untuk Perhitungan Aljabar

Pada notebook ini Anda belajar menggunakan EMT untuk melakukan
berbagai perhitungan terkait dengan materi atau topik dalam Aljabar.
Kegiatan yang harus Anda lakukan adalah sebagai berikut:


* 
Membaca secara cermat dan teliti notebook ini;

* 
Menerjemahkan teks bahasa Inggris ke bahasa Indonesia;

* 
Mencoba contoh-contoh perhitungan (perintah EMT) dengan cara
* meng-ENTER setiap perintah EMT yang ada (pindahkan kursor ke baris
* perintah)

* 
Jika perlu Anda dapat memodifikasi perintah yang ada dan memberikan
* keterangan/penjelasan tambahan terkait hasilnya.

* 
Menyisipkan baris-baris perintah baru untuk mengerjakan soal-soal
* Aljabar dari file PDF yang saya berikan;

* 
Memberi catatan hasilnya.

* 
Jika perlu tuliskan soalnya pada teks notebook (menggunakan format
* LaTeX).

* 
Gunakan tampilan hasil semua perhitungan yang eksak atau simbolik
* dengan format LaTeX. (Seperti contoh-contoh pada notebook ini.)


## Contoh pertama

Menyederhanakan bentuk aljabar:


$$6x^{-3}y^5\times-7x^2y^{-9}$$\>$&6\*x^(-3)\*y^5\*-7\*x^2\*y^(-9)


$$-\frac{42}{x\,y^4}$$Menjabarkan:


$$(6x^{-3}+y^5)(-7x^2-y^{-9})$$\>$&showev('expand((6\*x^(-3)+y^5)\*(-7\*x^2-y^(-9))))


$${\it expand}\left(\left(-\frac{1}{y^9}-7\,x^2\right)\,\left(y^5+  \frac{6}{x^3}\right)\right)=-7\,x^2\,y^5-\frac{1}{y^4}-\frac{6}{x^3  \,y^9}-\frac{42}{x}$$## Baris Perintah

Baris perintah Euler terdiri dari satu atau beberapa perintah Euler
yang diikuti dengan titik koma ";" atau koma ",". Titik koma mencegah
pencetakan hasil. Koma setelah perintah terakhir dapat dihilangkan.


Baris perintah berikut ini hanya akan mencetak hasil dari ekspresi,
bukan penugasan atau perintah format.


\>r:=2; h:=4; pi\*r^2\*h/3


    16.7551608191

Perintah harus dipisahkan dengan tanda kosong. Baris perintah berikut
ini mencetak dua hasilnya.


\>pi\*2\*r\*h, %+2\*pi\*r\*h // Ingat tanda % menyatakan hasil perhitungan terakhir sebelumnya


    50.2654824574
    100.530964915

Baris perintah dieksekusi sesuai urutan pengguna menekan tombol
return. Jadi, Anda mendapatkan nilai baru setiap kali Anda
mengeksekusi baris kedua.


\>x := 1;

\>x := cos(x) // nilai cosinus (x dalam radian)


    0.540302305868

\>x := cos(x)


    0.857553215846

Jika dua baris dihubungkan dengan "...", kedua baris tersebut akan
selalu dieksekusi secara bersamaan.


\>x := 1.5; ...  
\>   x := (x+2/x)/2, x := (x+2/x)/2, x := (x+2/x)/2, 


    1.41666666667
    1.41421568627
    1.41421356237

Ini juga merupakan cara yang baik untuk membagi perintah yang panjang
menjadi dua baris atau lebih. Anda dapat menekan Ctrl+Return untuk
membagi baris menjadi dua pada posisi kursor saat ini, atau Ctlr+Back
untuk menggabungkan kedua baris.


Untuk melipat semua multi-baris, tekan Ctrl+L. Kemudian garis-garis
berikutnya hanya akan terlihat, jika salah satu dari mereka memiliki
fokus. Untuk melipat satu baris multi-baris, mulai baris pertama
dengan "%+ ".


\>%+ x=4+5; ...  
\>    // Baris ini tidak akan terlihat setelah kursor keluar dari baris


Garis yang dimulai dengan %% tidak akan terlihat sama sekali.


    81

Euler mendukung perulangan dalam baris perintah, selama perulangan
tersebut masuk ke dalam satu baris tunggal atau beberapa baris. Dalam
program, tentu saja pembatasan ini tidak berlaku. Untuk informasi
lebih lanjut, baca pengantar berikut ini.


\>x=1; for i=1 to 5; x := (x+2/x)/2, end; // menghitung akar 2


    1.5
    1.41666666667
    1.41421568627
    1.41421356237
    1.41421356237

Tidak masalah untuk menggunakan multi-baris. Pastikan baris diakhiri
dengan "...".


\>x := 1.5; // comments go here before the ...  
\>   repeat xnew:=(x+2/x)/2; until xnew~=x; ...  
\>      x := xnew; ...  
\>   end; ...  
\>   x,


    1.41421356237

Struktur bersyarat juga bisa digunakan.


\>if E^pi\>pi^E; then "Thought so!", endif;


    Thought so!

Ketika Anda menjalankan perintah, kursor dapat berada di posisi mana
pun dalam baris perintah. Anda dapat kembali ke perintah sebelumnya
atau melompat ke perintah berikutnya dengan tombol panah. Atau Anda
dapat mengklik bagian komentar di atas perintah untuk membuka perintah
tersebut.


Ketika Anda menggerakkan kursor di sepanjang baris, pasangan tanda
kurung atau tanda kurung pembuka dan penutup akan disorot. Juga,
perhatikan baris status. Setelah tanda kurung pembuka dari fungsi
sqrt(), baris status akan menampilkan teks bantuan untuk fungsi
tersebut. Jalankan perintah dengan tombol return.


\>sqrt(sin(10°)/cos(20°))


    0.429875017772

Untuk melihat bantuan untuk perintah terbaru, buka jendela bantuan
dengan F1. Di sana, Anda dapat memasukkan teks yang akan dicari. Pada
baris kosong, bantuan untuk jendela bantuan akan ditampilkan. Anda
dapat menekan escape untuk mengosongkan baris, atau menutup jendela
bantuan.


Anda dapat mengklik dua kali pada perintah apa pun untuk membuka
bantuan untuk perintah ini. Coba klik dua kali perintah exp di bawah
ini pada baris perintah.


\>exp(log(2.5))


    2.5

Anda juga dapat menyalin dan menempel di Euler. Gunakan Ctrl-C dan
Ctrl-V untuk ini. Untuk menandai teks, seret mouse atau gunakan shift
bersamaan dengan tombol kursor. Selain itu, Anda dapat menyalin tanda
kurung yang disorot.


## Sintaksis Dasar

Euler mengetahui fungsi matematika yang biasa. Seperti yang telah Anda
lihat di atas, fungsi trigonometri bekerja dalam radian atau derajat.
Untuk mengonversi ke derajat, tambahkan simbol derajat (dengan tombol
F7) ke nilai, atau gunakan fungsi rad(x). Fungsi akar kuadrat disebut
sqrt dalam Euler. Tentu saja, x^(1/2) juga dapat digunakan.


Untuk mengatur variabel, gunakan "=" atau ":=". Demi kejelasan,
pengantar ini menggunakan bentuk yang terakhir. Spasi tidak menjadi
masalah. Tetapi spasi antar perintah diharapkan.


Beberapa perintah dalam satu baris dipisahkan dengan "," atau ";".
Titik koma menekan output dari perintah. Pada akhir baris perintah,
"," diasumsikan, jika ";" tidak ada.


\>g:=9.81; t:=2.5; 1/2\*g\*t^2


    30.65625

EMT menggunakan sintaks pemrograman untuk ekspresi. Untuk memasukkan


$$e^2\cdot\left(\frac{1}{3+4\log(0.6)}+\frac{1}{7}\right)$$Anda harus mengatur tanda kurung yang benar dan menggunakan / untuk
pecahan. Perhatikan tanda kurung yang disorot untuk mendapatkan
bantuan. Perhatikan bahwa konstanta Euler e diberi nama E dalam EMT.


\>E^2\*(1/(3+4\*log(0.6))+1/7)


    8.77908249441

Untuk menghitung ekspresi yang rumit seperti


$$\left(\frac{\frac17 + \frac18 + 2}{\frac13 + \frac12}\right)^2\pi$$Anda harus memasukkannya dalam bentuk baris.


\>((1/7 + 1/8 + 2) / (1/3 + 1/2))^2 \* pi


    23.2671801626

Letakkan tanda kurung di sekitar sub-ekspresi yang perlu dihitung
terlebih dahulu. EMT membantu Anda dengan menyorot ekspresi yang
diselesaikan oleh tanda kurung penutup. Anda juga harus memasukkan
nama "pi" untuk huruf Yunani pi.


Hasil dari perhitungan ini adalah angka floating point. Secara default
dicetak dengan akurasi sekitar 12 digit. Pada baris perintah berikut,
kita juga belajar bagaimana kita dapat merujuk ke hasil sebelumnya
dalam baris yang sama.


\>1/3+1/7, fraction %


    0.47619047619
    10/21

Perintah Euler dapat berupa ekspresi atau perintah primitif. Ekspresi
terbuat dari operator dan fungsi. Jika perlu, ekspresi tersebut harus
mengandung tanda kurung untuk memaksa urutan eksekusi yang benar. Jika
ragu, mengatur tanda kurung adalah ide yang bagus. Perhatikan bahwa
EMT menampilkan tanda kurung pembuka dan penutup saat mengedit baris
perintah.


\>(cos(pi/4)+1)^3\*(sin(pi/4)+1)^2


    14.4978445072

Operator numerik Euler meliputi


 + unary atau operator plus  
 - unary atau operator minus  
 *, /  
 . produk matriks  
 pangkat a^b untuk a positif atau bilangan bulat b (a**b juga bisa  

digunakan)


 n! operator faktorial


dan masih banyak lagi.


Berikut adalah beberapa fungsi yang mungkin Anda perlukan. Masih
banyak lagi.


 sin, cos, tan, atan, asin, acos, rad, deg  
 log, exp, log10, sqrt, logbase  
 bin, logbin, logfac, mod, floor, ceil, round, abs, sign  
 conj,re,im,arg,conj,real,complex  
 beta,betai,gamma,complexgamma,ellrf,ellf,ellrd,elle  
 bitand, bitor, bitxor, bitnot  

Beberapa perintah memiliki alias, misalnya ln untuk log.


\>ln(E^2), arctan(tan(0.5))


    2
    0.5

\>sin(30°)


    0.5

Pastikan untuk menggunakan tanda kurung (tanda kurung bulat), kapan
pun ada keraguan tentang urutan eksekusi! Berikut ini tidak sama
dengan (2^3)^4, yang merupakan default untuk 2^3^4 di EMT (beberapa
sistem numerik melakukannya dengan cara lain).


\>2^3^4, (2^3)^4, 2^(3^4)


    2.41785163923e+24
    4096
    2.41785163923e+24

## Bilangan Real

Tipe data utama dalam Euler adalah bilangan real. Bilangan real
direpresentasikan dalam format IEEE dengan akurasi sekitar 16 digit
desimal.


\>longest 1/3


         0.3333333333333333 

Representasi ganda internal membutuhkan 8 byte.


\>printdual(1/3)


    1.0101010101010101010101010101010101010101010101010101*2^-2

\>printhex(1/3)


    5.5555555555554*16^-1

## String

String dalam Euler didefinisikan dengan "...".


\>"A string can contain anything."


    A string can contain anything.

String dapat digabungkan dengan | atau dengan +. Ini juga berfungsi
dengan angka, yang dikonversi menjadi string dalam kasus tersebut.


\>"The area of the circle with radius " + 2 + " cm is " + pi\*4 + " cm^2."


    The area of the circle with radius 2 cm is 12.5663706144 cm^2.

Fungsi cetak juga mengonversi angka ke string. Fungsi ini dapat
mengambil sejumlah digit dan sejumlah tempat (0 untuk output padat),
dan secara optimal satu unit.


\>"Golden Ratio : " + print((1+sqrt(5))/2,5,0)


    Golden Ratio : 1.61803

Ada string khusus tidak ada, yang tidak mencetak. Dikembalikan oleh
beberapa fungsi, ketika hasilnya tidak penting. (Dikembalikan secara
otomatis, jika fungsi tidak memiliki pernyataan pengembalian).


\>none


Untuk mengonversi string menjadi angka, cukup evaluasi string
tersebut. Ini juga berlaku untuk ekspresi (lihat di bawah).


\>"1234.5"()


    1234.5

Untuk mendefinisikan vektor string, gunakan notasi vektor [...].


\>v:=["affe","charlie","bravo"]


    affe
    charlie
    bravo

Vektor string kosong dilambangkan dengan [none]. Vektor string dapat
digabungkan.


\>w:=[none]; w|v|v //w itu string kosong, trus diisi v, diisi v lagi


    affe
    charlie
    bravo
    affe
    charlie
    bravo

String dapat berisi karakter Unicode. Secara internal, string ini
berisi kode UTF-8. Untuk membuat string seperti itu, gunakan u"..."
dan salah satu entitas HTML.


String Unicode dapat digabungkan seperti string lainnya.


\>u"&alpha; = " + 45 + u"&deg;" // pdfLaTeX mungkin gagal menampilkan secara benar


    α = 45°

I


Dalam komentar, entitas yang sama seperti α, β dll. dapat
digunakan. Ini bisa menjadi alternatif yang cepat untuk Latex. (Detail
lebih lanjut tentang komentar di bawah).


Ada beberapa fungsi untuk membuat atau menganalisis string unicode.
Fungsi strtochar() akan mengenali string Unicode, dan menerjemahkannya
dengan benar.


\>v=strtochar(u"&Auml; is a German letter")


    [196,  32,  105,  115,  32,  97,  32,  71,  101,  114,  109,  97,  110,
    32,  108,  101,  116,  116,  101,  114]

\>v=strtochar(u"afaantuh")


    [97,  102,  97,  97,  110,  116,  117,  104]

Hasilnya adalah sebuah vektor angka Unicode. Fungsi kebalikannya
adalah chartoutf().


\>v[1]=strtochar(u"&Auml;")[1]; chartoutf(v)


    Äfaantuh

\>v[2]=strtochar(u"afaantuh")[2]; chartoutf(v)


    Äfaantuh

Fungsi utf() dapat menerjemahkan sebuah string dengan entitas dalam
sebuah variabel menjadi sebuah string Unicode.


\>s="We have &alpha;=&beta;."; utf(s) // pdfLaTeX mungkin gagal menampilkan secara benar


    We have α=β.

Dimungkinkan juga untuk menggunakan entitas numerik.


\>u"&#196;hnliches", u"&#220;dahlah"


    Ähnliches
    Üdahlah

## Nilai Boolean

Nilai Boolean direpresentasikan dengan 1 = benar atau 0 = salah dalam
Euler. String dapat dibandingkan, seperti halnya angka.


\>2<1, "apel"<"banana"


    0
    1

"dan" adalah operator "&amp;&amp;" dan "atau" adalah operator "||", seperti
dalam bahasa C. (Kata "dan" dan "atau" hanya dapat digunakan dalam
kondisi "jika").


\>2<E && E<3


    1

Operator Boolean mematuhi aturan bahasa matriks.


\>(1:10)\>5, nonzeros(%)


    [0,  0,  0,  0,  0,  1,  1,  1,  1,  1]
    [6,  7,  8,  9,  10]

Anda dapat menggunakan fungsi nonzeros() untuk mengekstrak elemen
tertentu dari sebuah vektor. Pada contoh, kita menggunakan kondisional
isprime(n).


\>N=2|3:2:99 // N berisi elemen 2 dan bilangan2 ganjil dari 3 s.d. 99


    [2,  3,  5,  7,  9,  11,  13,  15,  17,  19,  21,  23,  25,  27,  29,
    31,  33,  35,  37,  39,  41,  43,  45,  47,  49,  51,  53,  55,  57,
    59,  61,  63,  65,  67,  69,  71,  73,  75,  77,  79,  81,  83,  85,
    87,  89,  91,  93,  95,  97,  99]

\>N[nonzeros(isprime(N))] //pilih anggota2 N yang prima


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47,
    53,  59,  61,  67,  71,  73,  79,  83,  89,  97]

## Format Keluaran

Format output default EMT mencetak 12 digit. Untuk memastikan bahwa
kita melihat format default, kita atur ulang formatnya.


\>defformat; pi


    3.14159265359

Secara internal, EMT menggunakan standar IEEE untuk angka ganda dengan
sekitar 16 digit desimal. Untuk melihat jumlah digit penuh, gunakan
perintah "longestformat", atau kami menggunakan operator "longest"
untuk menampilkan hasil dalam format terpanjang.


\>longest pi


          3.141592653589793 

Berikut ini adalah representasi heksadesimal internal dari angka
ganda.


\>printhex(pi)


    3.243F6A8885A30*16^0

Format output dapat diubah secara permanen dengan perintah format.


\>format(12,7); 1/3, pi, sin(1) //format(12,n)=12 itu default, n itu byk angka dblkg koma


      0.3333333 
      3.1415927 
      0.8414710 

Standarnya adalah format(12).


\>format(12); 1/3


    0.333333333333

Fungsi seperti "shortestformat", "shortformat", "longformat" bekerja
untuk vektor dengan cara berikut.


\>shortestformat; random(3,8) //3 baris 8 kolom


      0.21   0.79   0.64   0.26   0.52   0.44   0.42   0.67 
      0.83   0.76   0.47   0.77   0.59  0.064   0.17    0.8 
      0.72   0.49   0.27   0.43   0.17  0.098   0.99      0 

Format default untuk skalar adalah format(12). Tetapi ini dapat
diubah.


\>setscalarformat(7); pi 


    3.141593

Fungsi "longestformat" juga menetapkan format skalar.


\>longestformat; pi


    3.141592653589793

Sebagai referensi, berikut ini adalah daftar format output yang paling
penting.


shortestformat shortformat longformat, longestformat


format(length,digits) goodformat(length)


fracformat(length)


defformat


Akurasi internal EMT adalah sekitar 16 tempat desimal, yang merupakan
standar IEEE. Angka disimpan dalam format internal ini.


Tetapi format keluaran EMT dapat diatur dengan cara yang fleksibel.


\>longestformat; pi,


    3.141592653589793

\>format(10,5); pi


      3.14159 

Standarnya adalah defformat().


\>defformat; // default format


Ada operator pendek yang hanya mencetak satu nilai. Operator " longest
" akan mencetak semua digit angka yang valid.


\>longest pi^2/2


          4.934802200544679 

Terdapat juga operator singkat untuk mencetak hasil dalam format
pecahan. Kami sudah menggunakannya di atas.


\>fraction 1+1/2+1/3+1/4


    25/12

Karena format internal menggunakan cara biner untuk menyimpan angka,
maka nilai 0,1 tidak akan terwakili dengan tepat. Kesalahan bertambah
sedikit, seperti yang Anda lihat dalam perhitungan berikut ini.


\>longest 0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


     -1.110223024625157e-16 

Tetapi, dengan "longformat" default, Anda tidak akan melihat hal ini.
Untuk kenyamanan, output angka yang sangat kecil adalah 0.


\>0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


    0

# Ekspresi

String atau nama dapat digunakan untuk menyimpan ekspresi matematika,
yang dapat dievaluasi oleh EMT. Untuk ini, gunakan tanda kurung
setelah ekspresi. Jika Anda bermaksud menggunakan string sebagai
ekspresi, gunakan konvensi untuk menamainya "fx" atau "fxy", dll.
Ekspresi lebih diutamakan daripada fungsi.


Variabel global dapat digunakan dalam evaluasi.


\>r:=2; fx:="pi\*r^2"; longest fx()


          12.56637061435917 

Parameter ditetapkan ke x, y, dan z dalam urutan tersebut. Parameter
tambahan dapat ditambahkan dengan menggunakan parameter yang
ditetapkan.


\>fx:="a\*sin(x)^2"; fx(5,a=-1)


    -0.919535764538

Perhatikan bahwa ekspresi akan selalu menggunakan variabel global,
meskipun ada variabel dalam fungsi dengan nama yang sama. (Jika tidak,
evaluasi ekspresi dalam fungsi dapat memberikan hasil yang sangat
membingungkan bagi pengguna yang memanggil fungsi tersebut).


\>at:=4; function f(expr,x,at) := expr(x); ...  
\>   f("at\*x^2",3,5) // computes 4\*3^2 not 5\*3^2 ...  
\>   //at sudah didef sbg 4 tp di fungsi f ada lagi variabel bernama at dg nilai yg berbeda ...  
\>   (di sini nilainya 5) tapi tetap yg dipakai adalah at yg pertama yaitu 4 karena var. global 


    36

Jika Anda ingin menggunakan nilai lain untuk "at" selain nilai global,
Anda perlu menambahkan "at=value".


\>at:=4; function f(expr,x,a) := expr(x,at=a); ...  
\>   f("at\*x^2",3,5) // di sini memakai at=5


    45

Sebagai referensi, kami menyatakan bahwa koleksi panggilan (dibahas di
tempat lain) dapat berisi ekspresi. Jadi kita dapat membuat contoh di
atas sebagai berikut.


\>at:=4; function f(expr,x) := expr(x); ...  
\>   f({{"at\*x^2",at=5}},3) 


    45

Ekspresi dalam x sering digunakan seperti halnya fungsi.


Perhatikan bahwa mendefinisikan fungsi dengan nama yang sama seperti
ekspresi simbolik global akan menghapus variabel ini untuk menghindari
kebingungan antara ekspresi simbolik dan fungsi.


\>f &= 5\*x;

\>function f(x) := 6\*x;

\>f(2)


    12

Sesuai dengan konvensi, ekspresi simbolik atau numerik harus diberi
nama fx, fxy, dll. Skema penamaan ini tidak boleh digunakan untuk
fungsi.


\>fx &= diff(x^x,x); $&fx


$$x^{x}\,\left(\log x+1\right)$$Bentuk khusus dari sebuah ekspresi memungkinkan variabel apa pun
sebagai parameter tanpa nama untuk evaluasi ekspresi, bukan hanya "x",
"y", dll. Untuk ini, mulailah ekspresi dengan "@(variabel)...".


\>"@(a,b) a^2+b^2", %(4,5)


    @(a,b) a^2+b^2
    41

Hal ini memungkinkan untuk memanipulasi ekspresi dalam variabel lain
untuk fungsi EMT yang membutuhkan ekspresi dalam "x".


Cara paling dasar untuk mendefinisikan fungsi sederhana adalah dengan
menyimpan rumusnya dalam ekspresi simbolik atau numerik. Jika variabel
utamanya adalah x, ekspresi tersebut dapat dievaluasi seperti halnya
sebuah fungsi.


Seperti yang Anda lihat pada contoh berikut, variabel global terlihat
selama evaluasi.


\>fx &= x^3-a\*x;  ...  
\>   a=1.2; fx(0.5)


    -0.475

Semua variabel lain dalam ekspresi dapat ditentukan dalam evaluasi
menggunakan parameter yang ditetapkan.


\>fx(0.5,a=1.1)


    -0.425

Sebuah ekspresi tidak perlu berbentuk simbolik. Hal ini diperlukan,
jika ekspresi mengandung fungsi-fungsi, yang hanya dikenal di kernel
numerik, bukan di Maxima.


# Matematika Simbolik

EMT melakukan matematika simbolik dengan bantuan Maxima. Untuk
detailnya, mulailah dengan tutorial berikut ini, atau telusuri
referensi untuk Maxima. Para ahli dalam Maxima harus memperhatikan
bahwa ada perbedaan dalam sintaks antara sintaks asli Maxima dan
sintaks default dari ekspresi simbolik dalam EMT.


Matematika simbolik diintegrasikan secara mulus ke dalam Euler dengan
&amp;. Ekspresi apapun yang dimulai dengan &amp; adalah sebuah ekspresi
simbolik. Ekspresi ini dievaluasi dan dicetak oleh Maxima.


Pertama-tama, Maxima memiliki aritmatika "infinite" yang dapat
menangani angka yang sangat besar.


\>$&44!


$$2658271574788448768043625811014615890319638528000000000$$Dengan cara ini, Anda dapat menghitung hasil yang besar secara tepat.
Mari kita hitung


$$C(44,10) = \frac{44!}{34!\cdot 10!}$$\>$& 44!/(34!\*10!) // nilai C(44,10)


$$2481256778$$Tentu saja, Maxima memiliki fungsi yang lebih efisien untuk hal ini
(seperti halnya bagian numerik EMT).


\>$binomial(44,10) //menghitung C(44,10) menggunakan fungsi binomial()


$$2481256778$$Untuk mempelajari lebih lanjut tentang fungsi tertentu, klik dua kali
pada fungsi tersebut. Sebagai contoh, coba klik dua kali pada
"&amp;binomial" di baris perintah sebelumnya. Ini akan membuka dokumentasi
Maxima yang disediakan oleh pembuat program tersebut.


Anda akan mengetahui bahwa perintah-perintah berikut ini juga dapat
digunakan.


$$C(x,3) = \frac{x!}{(x-3)!3!}=\frac{(x-2)(x-1)x}{6}$$\>$binomial(x,3) // C(x,3)


$$\frac{\left(x-2\right)\,\left(x-1\right)\,x}{6}$$Jika Anda ingin mengganti x dengan nilai tertentu, gunakan "with".


\>$&binomial(x,3) with x=10 // substitusi x=10 ke C(x,3)


$$120$$Dengan begitu, Anda dapat menggunakan solusi dari sebuah persamaan
dalam persamaan lain.


Ekspresi simbolik dicetak oleh Maxima dalam bentuk 2D. Alasannya
adalah sebuah bendera simbolik khusus dalam string.


Seperti yang telah Anda lihat pada contoh sebelumnya dan contoh
berikut, jika Anda telah menginstal LaTeX, Anda dapat mencetak
ekspresi simbolik dengan Latex. Jika tidak, perintah berikut ini akan
mengeluarkan error massage.


Untuk mencetak ekspresi simbolik dengan LaTeX, gunakan $ di depan &amp;
(atau Anda dapat menghilangkan &amp;) sebelum perintah. Jangan jalankan
perintah Maxima dengan $, jika Anda tidak memiliki LaTeX.


\>$(3+x)/(x^2+1)


$$\frac{x+3}{x^2+1}$$Ekspresi simbolik diuraikan oleh Euler. Jika Anda membutuhkan sintaks
yang kompleks dalam satu ekspresi, Anda dapat mengapit ekspresi dalam
"...". Menggunakan lebih dari satu ekspresi sederhana dimungkinkan,
tetapi sangat tidak disarankan.


\>&"v := 5; v^2"


    
                                      25
    

Untuk kelengkapan, kami menyatakan bahwa ekspresi simbolik dapat
digunakan dalam program, tetapi harus diapit dengan tanda kutip.
Selain itu, akan jauh lebih efektif untuk memanggil Maxima pada saat
kompilasi jika memungkinkan.


\>$&expand((1+x)^4), $&factor(diff(%,x)) // diff: turunan, factor: faktor


$$4\,\left(x+1\right)^3$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-031.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-031.png)

Sekali lagi, % mengacu pada hasil sebelumnya.


Untuk mempermudah, kita menyimpan solusi ke dalam sebuah variabel
simbolik. Variabel simbolik didefinisikan dengan "&amp;=".


\>fx &= (x+1)/(x^4+1); $&fx


$$\frac{x+1}{x^4+1}$$Ekspresi simbolik dapat digunakan dalam ekspresi simbolik lainnya.


\>$&factor(diff(fx,x))


$$\frac{-3\,x^4-4\,x^3+1}{\left(x^4+1\right)^2}$$Masukan langsung dari perintah Maxima juga tersedia. Mulai baris
perintah dengan "::". Sintaks Maxima disesuaikan dengan sintaks EMT
(disebut "compatibility mode").


\>&factor(20!)


    
                             2432902008176640000
    

\>::: factor(10!)


    
                                   8  4  2
                                  2  3  5  7
    

\>:: factor(20!)


    
                            18  8  4  2
                           2   3  5  7  11 13 17 19
    

\>::: factor(20!)


    
                            18  8  4  2
                           2   3  5  7  11 13 17 19
    

Jika Anda adalah seorang ahli dalam Maxima, Anda mungkin ingin
menggunakan sintaks asli Maxima. Anda dapat melakukan ini dengan
":::".


\>::: av:y$ av^2;


    
                                       2
                                      y
    

\>fx &= x^3\*exp(x), $fx


    
                                     3  x
                                    x  E
    

$$x^3\,e^{x}$$Variabel tersebut dapat digunakan dalam ekspresi simbolik lainnya.
Perhatikan, bahwa pada perintah berikut ini, sisi kanan dari &amp;=
dievaluasi sebelum penugasan ke Fx.


\>&(fx with x=5), $%, &float(%)


    
                                         5
                                    125 E
    

$$125\,e^5$$    
                              18551.64488782208
    

\>fx(5)


    18551.6448878

Untuk mengevaluasi ekspresi dengan nilai variabel tertentu, Anda dapat
menggunakan operator "with".


Baris perintah berikut ini juga mendemonstrasikan bahwa Maxima dapat
mengevaluasi sebuah ekspresi secara numerik dengan float().


\>&(fx with x=10)-(fx with x=5), &float(%)


    
                                    10        5
                              1000 E   - 125 E
    
    
                             2.20079141499189e+7
    

\>$factor(diff(fx,x,2))


$$x\,\left(x^2+6\,x+6\right)\,e^{x}$$Untuk mendapatkan kode Latex untuk sebuah ekspresi, Anda dapat
menggunakan perintah tex.


\>tex(fx)


    x^3\,e^{x}

Seperti ini latex nya:


$$x^3\,e^{x}$$Ekspresi simbolik dapat dievaluasi seperti halnya ekspresi numerik.


\>fx(0.5)


    0.206090158838

Dalam ekspresi simbolik, hal ini tidak dapat dilakukan, karena Maxima
tidak mendukungnya. Sebagai gantinya, gunakan sintaks "with" (bentuk
yang lebih baik dari perintah at(...) pada Maxima).


\>$&fx with x=1/2


$$\frac{\sqrt{e}}{8}$$Penugasan ini juga bisa bersifat simbolis.


\>$&fx with x=1+t


$$\left(t+1\right)^3\,e^{t+1}$$Perintah solve menyelesaikan ekspresi simbolik untuk sebuah variabel
di Maxima. Hasilnya adalah sebuah vektor solusi.


\>$&solve(x^2+x=4,x)


$$\left[ x=\frac{-\sqrt{17}-1}{2} , x=\frac{\sqrt{17}-1}{2} \right] $$Bandingkan dengan perintah "solve" numerik di Euler, yang membutuhkan
nilai awal, dan secara opsional nilai target.


\>solve("x^2+x",1,y=4)


    1.56155281281

Nilai numerik dari solusi simbolik dapat dihitung dengan evaluasi
hasil simbolik. Euler akan membaca penugasan x= etc. Jika Anda tidak
membutuhkan hasil numerik untuk perhitungan lebih lanjut, Anda juga
bisa membiarkan Maxima menemukan nilai numeriknya.


\>sol &= solve(x^2+2\*x=4,x); $&sol, sol(), $&float(sol)


$$\left[ x=-\sqrt{5}-1 , x=\sqrt{5}-1 \right] $$    [-3.23607,  1.23607]

$$\left[ x=-3.23606797749979 , x=1.23606797749979 \right] $$Untuk mendapatkan solusi simbolik yang spesifik, seseorang dapat
menggunakan " with " dan indeks.


\>$&solve(x^2+x=1,x), x2 &= x with %[2]; $&x2


$$\frac{\sqrt{5}-1}{2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-044.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-044.png)

Untuk menyelesaikan sistem persamaan, gunakan vektor persamaan.
Hasilnya adalah vektor solusi.


\>sol &= solve([x+y=3,x^2+y^2=5],[x,y]); $&sol, $&x\*y with sol[1]


$$2$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-046.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-046.png)

Ekspresi simbolik dapat memiliki bendera, yang menunjukkan perlakuan
khusus di Maxima. Beberapa flag dapat digunakan sebagai perintah juga,
namun ada juga yang tidak. Bendera ditambahkan dengan "|" (bentuk yang
lebih baik dari "ev(...,flags)")


\>$& diff((x^3-1)/(x+1),x) //turunan bentuk pecahan


$$\frac{3\,x^2}{x+1}-\frac{x^3-1}{\left(x+1\right)^2}$$\>$& diff((x^3-1)/(x+1),x) | ratsimp //menyederhanakan pecahan


$$\frac{2\,x^3+3\,x^2+1}{x^2+2\,x+1}$$\>$&factor(%)


$$\frac{2\,x^3+3\,x^2+1}{\left(x+1\right)^2}$$# Fungsi

Dalam EMT, fungsi adalah program yang ditentukan dengan perintah
"function". Fungsi dapat berupa fungsi satu baris atau fungsi
multibaris.


Fungsi satu baris dapat berupa numerik atau simbolik. Fungsi satu
baris numerik didefinisikan dengan ":=".


\>function f(x) := x\*sqrt(x^2+1)


Sebagai gambaran umum, kami menunjukkan semua definisi yang mungkin
untuk fungsi satu baris. Sebuah fungsi dapat dievaluasi seperti halnya
fungsi Euler bawaan.


\>f(2)


    4.472135955

Fungsi ini juga dapat digunakan untuk vektor, mengikuti bahasa matriks
Euler, karena ekspresi yang digunakan dalam fungsi ini adalah vektor.


\>f(0:0.1:1)


    [0,  0.100499,  0.203961,  0.313209,  0.430813,  0.559017,  0.699714,
    0.854459,  1.0245,  1.21083,  1.41421]

Fungsi dapat diplot. Alih-alih ekspresi, kita hanya perlu memberikan
nama fungsi.


Berbeda dengan ekspresi simbolik atau numerik, nama fungsi harus
disediakan dalam bentuk string.


\>solve("f",1,y=1)


    0.786151377757

Secara default, jika Anda perlu menimpa fungsi built-in, Anda harus
menambahkan kata kunci "overwrite". Menimpa fungsi bawaan berbahaya
dan dapat menyebabkan masalah bagi fungsi lain yang bergantung pada
fungsi tersebut.


Anda masih dapat memanggil fungsi bawaan sebagai "_...", jika fungsi
tersebut merupakan fungsi dalam inti Euler.


\>function overwrite sin (x) := \_sin(x°) // redine sine in degrees

\>sin(45)


    0.707106781187

Sebaiknya kita hilangkan definisi ulang tentang sin ini.


\>forget sin; sin(pi/4)


    0.707106781187

## Parameter Default

Fungsi numerik dapat memiliki parameter default.


\>function f(x,a=1) := a\*x^2


Menghilangkan parameter ini menggunakan nilai default.


\>f(4)


    16

Menetapkannya akan menimpa nilai default.


\>f(4,5)


    80

Parameter yang ditetapkan juga menimpanya. Ini digunakan oleh banyak
fungsi Euler seperti plot2d, plot3d.


\>f(4,a=1)


    16

Jika sebuah variabel bukan parameter, maka variabel tersebut harus
bersifat global. Fungsi satu baris dapat melihat variabel global.


\>function f(x) := a\*x^2

\>a=6; f(2)


    24

Tetapi parameter yang ditetapkan akan menggantikan nilai global.


Jika argumen tidak ada dalam daftar parameter yang telah ditetapkan
sebelumnya, argumen tersebut harus dideklarasikan dengan ":="!


\>f(2,a:=5)


    20

Fungsi simbolik didefinisikan dengan "&amp;=". Fungsi-fungsi ini
didefinisikan dalam Euler dan Maxima, dan dapat digunakan di kedua
bahasa tersebut. Ekspresi pendefinisian dijalankan melalui Maxima
sebelum definisi.


\>function g(x) &= x^3-x\*exp(-x); $&g(x)


$$x^3-x\,e^ {- x }$$Fungsi simbolis dapat digunakan dalam ekspresi simbolis.


\>$&diff(g(x),x), $&% with x=4/3


$$\frac{e^ {- \frac{4}{3} }}{3}+\frac{16}{3}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-052.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-052.png)

Fungsi ini juga dapat digunakan dalam ekspresi numerik. Tentu saja,
ini hanya akan berfungsi jika EMT dapat menginterpretasikan semua yang
ada di dalam fungsi.


\>g(5+g(1))


    178.635099908

Mereka dapat digunakan untuk mendefinisikan fungsi atau ekspresi
simbolis lainnya.


\>function G(x) &= factor(integrate(g(x),x)); $&G(c) // integrate: mengintegralkan


$$\frac{e^ {- c }\,\left(c^4\,e^{c}+4\,c+4\right)}{4}$$\>solve(&g(x),0.5)


    0.703467422498

Hal berikut ini juga dapat digunakan, karena Euler menggunakan
ekspresi simbolik dalam fungsi g, jika tidak menemukan variabel
simbolik g, dan jika ada fungsi simbolik g.


\>solve(&g,0.5)


    0.703467422498

\>function P(x,n) &= (2\*x-1)^n; $&P(x,n)


$$\left(2\,x-1\right)^{n}$$\>function Q(x,n) &= (x+2)^n; $&Q(x,n)


$$\left(x+2\right)^{n}$$\>$&P(x,4), $&expand(%)


$$16\,x^4-32\,x^3+24\,x^2-8\,x+1$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-057.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-057.png)

\>P(3,4)


    625

\>$&P(x,4)+ Q(x,3), $&expand(%)


$$16\,x^4-31\,x^3+30\,x^2+4\,x+9$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-059.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-059.png)

\>$&P(x,4)-Q(x,3), $&expand(%), $&factor(%)


$$16\,x^4-33\,x^3+18\,x^2-20\,x-7$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-061.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-061.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-062.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-062.png)

\>$&P(x,4)\*Q(x,3), $&expand(%), $&factor(%)


$$\left(x+2\right)^3\,\left(2\,x-1\right)^4$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-064.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-064.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-065.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-065.png)

\>$&P(x,4)/Q(x,1), $&expand(%), $&factor(%)


$$\frac{\left(2\,x-1\right)^4}{x+2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-067.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-067.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-068.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-068.png)

\>function f(x) &= x^3-x; $&f(x)


$$x^3-x$$Dengan &amp;=, fungsi ini bersifat simbolis, dan dapat digunakan dalam
ekspresi simbolis lainnya.


\>$&integrate(f(x),x)


$$\frac{x^4}{4}-\frac{x^2}{2}$$Dengan := fungsi tersebut berupa angka. Contoh yang baik adalah
integral pasti seperti


$$f(x) := \int_1^x t^t\, dt,$$yang tidak dapat dievaluasi secara simbolik.


Jika kita mendefinisikan ulang fungsi tersebut dengan kata kunci
"map", maka fungsi tersebut dapat digunakan untuk vektor x. Secara
internal, fungsi tersebut dipanggil untuk semua nilai x satu kali, dan
hasilnya disimpan dalam sebuah vektor.


\>function map f(x) := integrate("x^x",1,x)

\>f(0:0.5:2)


    [-0.783431,  -0.410816,  0,  0.676863,  2.05045]

Fungsi dapat memiliki nilai default untuk parameter.


\>function mylog (x,base=10) := ln(x)/ln(base);


Sekarang, fungsi ini dapat dipanggil dengan atau tanpa parameter
"base".


\>mylog(100), mylog(2^6.7,2)


    2
    6.7

Selain itu, dimungkinkan untuk menggunakan parameter yang ditetapkan.


\>mylog(E^2,base=E)


    2

Sering kali, kita ingin menggunakan fungsi untuk vektor di satu
tempat, dan untuk masing-masing elemen di tempat lain. Hal ini
dimungkinkan dengan parameter vektor.


\>function f([a,b]) &= a^2+b^2-a\*b+b; $&f(a,b), $&f(x,y)


$$y^2-x\,y+y+x^2$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-073.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-073.png)

Fungsi simbolik seperti itu dapat digunakan untuk variabel simbolik.


Tetapi fungsi ini juga dapat digunakan untuk vektor numerik.


\>v=[3,4]; f(v)


    17

Ada juga fungsi yang murni simbolis, yang tidak dapat digunakan secara
numerik.


\>function lapl(expr,x,y) &&= diff(expr,x,2)+diff(expr,y,2)//turunan parsial kedua


    
                     diff(expr, y, 2) + diff(expr, x, 2)
    

\>$&realpart((x+I\*y)^4), $&lapl(%,x,y)


$$0$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-075.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-075.png)

Tetapi tentu saja, semua itu bisa digunakan dalam ekspresi simbolis
atau dalam definisi fungsi simbolis.


\>function f(x,y) &= factor(lapl((x+y^2)^5,x,y)); $&f(x,y)


$$10\,\left(y^2+x\right)^3\,\left(9\,y^2+x+2\right)$$Untuk meringkas


* 
&amp;= mendefinisikan fungsi simbolik,

* 
:= mendefinisikan fungsi numerik,

* 
&amp;&amp;= mendefinisikan fungsi simbolik murni.


# Memecahkan Ekspresi

Ekspresi dapat diselesaikan secara numerik dan simbolik.


Untuk menyelesaikan ekspresi sederhana dari satu variabel, kita dapat
menggunakan fungsi solve(). Fungsi ini membutuhkan nilai awal untuk
memulai pencarian. Secara internal, solve() menggunakan metode secant.


\>solve("x^2-2",1)


    1.41421356237

Hal ini juga bisa digunakan untuk ekspresi simbolis. Perhatikan fungsi
berikut ini.


\>$&solve(x^2=2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(x^2-2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(a\*x^2+b\*x+c=0,x)


$$\left[ x=\frac{-\sqrt{b^2-4\,a\,c}-b}{2\,a} , x=\frac{\sqrt{b^2-4\,  a\,c}-b}{2\,a} \right] $$\>$&solve([a\*x+b\*y=c,d\*x+e\*y=f],[x,y])


$$\left[ \left[ x=-\frac{c\,e}{b\,\left(d-5\right)-a\,e} , y=\frac{c  \,\left(d-5\right)}{b\,\left(d-5\right)-a\,e} \right]  \right] $$\>px &= 4\*x^8+x^7-x^4-x; $&px


$$4\,x^8+x^7-x^4-x$$Sekarang kita mencari titik, di mana polinomialnya adalah 2. Dalam
solve(), nilai target default y=0 dapat diubah dengan variabel yang
ditetapkan.


Kami menggunakan y=2 dan mengeceknya dengan mengevaluasi polinomial
pada hasil sebelumnya.


\>solve(px,1,y=2), px(%)


    0.966715594851
    2

Memecahkan sebuah ekspresi simbolik dalam bentuk simbolik
mengembalikan sebuah daftar solusi. Kami menggunakan pemecah simbolik
solve() yang disediakan oleh Maxima.


\>sol &= solve(x^2-x-1,x); $&sol


$$\left[ x=\frac{1-\sqrt{5}}{2} , x=\frac{\sqrt{5}+1}{2} \right] $$Cara termudah untuk mendapatkan nilai numerik adalah dengan
mengevaluasi solusi secara numerik seperti sebuah ekspresi.


\>longest sol()


        -0.6180339887498949       1.618033988749895 

Untuk menggunakan solusi secara simbolis dalam ekspresi lain, cara
termudah adalah " with ".


\>$&x^2 with sol[1], $&expand(x^2-x-1 with sol[2])


$$0$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-084.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-084.png)

Menyelesaikan sistem persamaan secara simbolik dapat dilakukan dengan
vektor persamaan dan pemecah simbolik solve(). Jawabannya adalah
sebuah daftar daftar persamaan.


\>$&solve([x+y=2,x^3+2\*y+x=4],[x,y])


$$\left[ \left[ x=-1 , y=3 \right]  , \left[ x=1 , y=1 \right]  ,   \left[ x=0 , y=2 \right]  \right] $$Fungsi f() dapat melihat variabel global. Tetapi seringkali kita ingin
menggunakan parameter lokal.


$$a^x-x^a = 0.1$$with a = 3.


\>function f(x,a) := x^a-a^x;


Salah satu cara untuk mengoper parameter tambahan ke f() adalah dengan
menggunakan sebuah daftar yang berisi nama fungsi dan parameternya
(cara lainnya adalah dengan menggunakan parameter titik koma).


\>solve({{"f",3}},2,y=0.1)


    2.54116291558

Hal ini juga dapat dilakukan dengan ekspresi. Namun, elemen daftar
bernama harus digunakan. (Lebih lanjut tentang daftar dalam tutorial
tentang sintaks EMT).


\>solve({{"x^a-a^x",a=3}},2,y=0.1)


    2.54116291558

# Menyelesaikan Pertidaksamaan

Untuk menyelesaikan pertidaksamaan, EMT tidak akan dapat melakukannya,
melainkan dengan bantuan Maxima, artinya secara eksak (simbolik).
Perintah Maxima yang digunakan adalah fourier_elim(), yang harus
dipanggil dengan perintah "load(fourier_elim)" terlebih dahulu.


\>&load(fourier\_elim)


    
            C:/Program Files/Euler x64/maxima/share/maxima/5.35.1/share/f\
    ourier_elim/fourier_elim.lisp
    

\>$&fourier\_elim([x^2 - 1\>0],[x]) // x^2-1 \> 0


$$\left[ 1<x \right] \lor \left[ x<-1 \right] $$\>$&fourier\_elim([x^2 - 1<0],[x]) // x^2-1 < 0


$$\left[ -1<x , x<1 \right] $$\>$&fourier\_elim([x^2 - 1 # 0],[x]) // x^-1 <\> 0


$$\left[ -1<x , x<1 \right] \lor \left[ 1<x \right] \lor \left[ x<-1   \right] $$\>$&fourier\_elim([x # 6],[x])


$$\left[ x<6 \right] \lor \left[ 6<x \right] $$\>$&fourier\_elim([x < 1, x \> 1],[x]) // tidak memiliki penyelesaian


$${\it emptyset}$$\>$&fourier\_elim([minf < x, x < inf],[x]) // solusinya R


$${\it universalset}$$\>$&fourier\_elim([x^3 - 1 \> 0],[x])


$$\left[ 1<x , x^2+x+1>0 \right] \lor \left[ x<1 , -x^2-x-1>0   \right] $$\>$&fourier\_elim([cos(x) < 1/2],[x]) // ??? gagal


$$\left[ 1-2\,\cos x>0 \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[x,y]) // sistem pertidaksamaan


$$\left[ y-5<x , x<y+7 , 10<y \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[y,x])


$$\left[ {\it max}\left(10 , x-7\right)<y , y<x+5 , 5<x \right] $$\>$&fourier\_elim((x + y < 5) and (x - y \>8),[x,y])


$$\left[ y+8<x , x<5-y , y<-\frac{3}{2} \right] $$\>$&fourier\_elim(((x + y < 5) and x < 1) or  (x - y \>8),[x,y])


$$\left[ y+8<x \right] \lor \left[ x<{\it min}\left(1 , 5-y\right)   \right] $$\>&fourier\_elim([max(x,y) \> 6, x # 8, abs(y-1) \> 12],[x,y])


    
            [6 &lt; x, x &lt; 8, y &lt; - 11] or [8 &lt; x, y &lt; - 11]
     or [x &lt; 8, 13 &lt; y] or [x = y, 13 &lt; y] or [8 &lt; x, x &lt; y, 13 &lt; y]
     or [y &lt; x, 13 &lt; y]
    

\>$&fourier\_elim([(x+6)/(x-9) <= 6],[x])


$$\left[ x=12 \right] \lor \left[ 12<x \right] \lor \left[ x<9   \right] $$# Bahasa Matriks

Dokumentasi inti EMT berisi diskusi rinci tentang bahasa matriks
Euler.


Vektor dan matriks dimasukkan dengan tanda kurung siku, elemen
dipisahkan dengan koma, baris dipisahkan dengan titik koma.


\>A=[1,2;3,4]


                1             2 
                3             4 

Hasil kali matriks dilambangkan dengan sebuah titik.


\>b=[3;4]


                3 
                4 

\>b' // transpose b


    [3,  4]

\>inv(A) //inverse A


               -2             1 
              1.5          -0.5 

\>A.b //perkalian matriks


               11 
               25 

\>A.inv(A)


                1             0 
                0             1 

Poin utama dari bahasa matriks adalah bahwa semua fungsi dan operator
bekerja elemen demi elemen.


\>A.A


                7            10 
               15            22 

\>A^2 //perpangkatan elemen2 A


                1             4 
                9            16 

\>A.A.A


               37            54 
               81           118 

\>power(A,3) //perpangkatan matriks


               37            54 
               81           118 

\>A/A //pembagian elemen-elemen matriks yang seletak


                1             1 
                1             1 

\>A/b //pembagian elemen2 A oleh elemen2 b kolom demi kolom (karena b vektor kolom)


         0.333333      0.666667 
             0.75             1 

\>A\\b // hasilkali invers A dan b, A^(-1)b 


               -2 
              2.5 

\>inv(A).b


               -2 
              2.5 

\>A\\A   //A^(-1)A


                1             0 
                0             1 

\>inv(A).A


                1             0 
                0             1 

\>A\*A //perkalin elemen-elemen matriks seletak


                1             4 
                9            16 

Ini bukan hasil kali matriks, tetapi perkalian elemen demi elemen. Hal
yang sama berlaku untuk vektor.


\>b^2 // perpangkatan elemen-elemen matriks/vektor


                9 
               16 

Jika salah satu operan adalah vektor atau skalar, maka operan tersebut
akan diperluas dengan cara alami.


\>2\*A


                2             4 
                6             8 

Misalnya, jika operan adalah vektor kolom, elemen-elemennya diterapkan
ke semua baris A.


\>[1,2]\*A


                1             4 
                3             8 

Jika ini adalah vektor baris, vektor ini diterapkan ke semua kolom A.


\>A\*[2,3]


                2             6 
                6            12 

Kita dapat membayangkan perkalian ini seolah-olah vektor baris v telah
diduplikasi untuk membentuk matriks dengan ukuran yang sama dengan A.


\>dup([1,2],2) // dup: menduplikasi/menggandakan vektor [1,2] sebanyak 2 kali (baris)


                1             2 
                1             2 

\>A\*dup([1,2],2) 


                1             4 
                3             8 

Hal ini juga berlaku untuk dua vektor di mana satu vektor adalah
vektor baris dan yang lainnya adalah vektor kolom. Kami menghitung i*j
untuk i, j dari 1 sampai 5. Caranya adalah dengan mengalikan 1:5
dengan transposenya. Bahasa matriks Euler secara otomatis menghasilkan
sebuah tabel nilai.


\>(1:5)\*(1:5)' // hasilkali elemen-elemen vektor baris dan vektor kolom


                1             2             3             4             5 
                2             4             6             8            10 
                3             6             9            12            15 
                4             8            12            16            20 
                5            10            15            20            25 

Sekali lagi, ingatlah bahwa ini bukan produk matriks!


\>(1:5).(1:5)' // hasilkali vektor baris dan vektor kolom


    55

\>sum((1:5)\*(1:5)) // sama hasilnya


    55

Bahkan operator seperti &lt; atau == bekerja dengan cara yang sama.


\>(1:10)<6 // menguji elemen-elemen yang kurang dari 6


    [1,  1,  1,  1,  1,  0,  0,  0,  0,  0]

Sebagai contoh, kita dapat menghitung jumlah elemen yang memenuhi
kondisi tertentu dengan fungsi sum().


\>sum((1:10)<6) // banyak elemen yang kurang dari 6


    5

Euler memiliki operator perbandingan, seperti "==", yang memeriksa
kesetaraan.


Kita mendapatkan vektor 0 dan 1, di mana 1 berarti benar.


\>t=(1:10)^2; t==25 //menguji elemen2 t yang sama dengan 25 (hanya ada 1)


    [0,  0,  0,  0,  1,  0,  0,  0,  0,  0]

Dari vektor seperti itu, "nonzeros" memilih elemen yang bukan nol.


Dalam hal ini, kita mendapatkan indeks semua elemen yang lebih besar
dari 50.


\>nonzeros(t\>50) //indeks elemen2 t yang lebih besar daripada 50


    [8,  9,  10]

Tentu saja, kita dapat menggunakan vektor indeks ini untuk mendapatkan
nilai yang sesuai dalam t.


\>t[nonzeros(t\>50)] //elemen2 t yang lebih besar daripada 50


    [64,  81,  100]

Sebagai contoh, mari kita cari semua kuadrat dari angka 1 sampai 1000,
yaitu 5 modulo 11 dan 3 modulo 13.


\>t=1:1000; nonzeros(mod(t^2,11)==5 && mod(t^2,13)==3)


    [4,  48,  95,  139,  147,  191,  238,  282,  290,  334,  381,  425,
    433,  477,  524,  568,  576,  620,  667,  711,  719,  763,  810,  854,
    862,  906,  953,  997]

EMT tidak sepenuhnya efektif untuk komputasi bilangan bulat. EMT
menggunakan floating point presisi ganda secara internal. Akan tetapi,
hal ini sering kali sangat berguna.


Kita dapat memeriksa bilangan prima. Mari kita cari tahu, berapa
banyak kuadrat ditambah 1 yang merupakan bilangan prima.


\>t=1:1000; length(nonzeros(isprime(t^2+1)))


    112

Fungsi nonzeros() hanya bekerja untuk vektor. Untuk matriks, ada
mnonzeros().


\>seed(2); A=random(3,4)


         0.765761      0.401188      0.406347      0.267829 
          0.13673      0.390567      0.495975      0.952814 
         0.548138      0.006085      0.444255      0.539246 

Ini mengembalikan indeks elemen, yang bukan nol.


\>k=mnonzeros(A<0.4) //indeks(baris kolom) elemen2 A yang kurang dari 0,4


                1             4 
                2             1 
                2             2 
                3             2 

Indeks ini dapat digunakan untuk menetapkan elemen ke suatu nilai.


\>mset(A,k,0) //mengganti elemen2 suatu matriks pada indeks tertentu


         0.765761      0.401188      0.406347             0 
                0             0      0.495975      0.952814 
         0.548138             0      0.444255      0.539246 

Fungsi mset() juga dapat mengatur elemen-elemen pada indeks ke
entri-entri matriks lain.


\>mset(A,k,-random(size(A)))


         0.765761      0.401188      0.406347     -0.126917 
        -0.122404     -0.691673      0.495975      0.952814 
         0.548138     -0.483902      0.444255      0.539246 

Dan dimungkinkan untuk mendapatkan elemen-elemen dalam vektor.


\>mget(A,k)


    [0.267829,  0.13673,  0.390567,  0.006085]

Fungsi lain yang berguna adalah extrema, yang mengembalikan nilai
minimal dan maksimal di setiap baris matriks dan posisinya.


\>ex=extrema(A)


         0.267829             4      0.765761             1 
          0.13673             1      0.952814             4 
         0.006085             2      0.548138             1 

Kita bisa menggunakan ini untuk mengekstrak nilai maksimal dalam
setiap baris.


\>ex[,3]'


    [0.765761,  0.952814,  0.548138]

Ini, tentu saja, sama dengan fungsi max().


\>max(A)'


    [0.765761,  0.952814,  0.548138]

Tetapi dengan mget(), kita dapat mengekstrak indeks dan menggunakan
informasi ini untuk mengekstrak elemen-elemen pada posisi yang sama
dari matriks yang lain.


\>j=(1:rows(A))'|ex[,4], mget(-A,j)


                1             1 
                2             4 
                3             1 
    [-0.765761,  -0.952814,  -0.548138]

# Fungsi Matriks Lainnya (Membangun Matriks)

Untuk membangun sebuah matriks, kita dapat menumpuk satu matriks di
atas matriks lainnya. Jika keduanya tidak memiliki jumlah kolom yang
sama, kolom yang lebih pendek akan diisi dengan 0.


\>v=1:3; v\_v


                1             2             3 
                1             2             3 

Demikian juga, kita dapat melampirkan matriks ke matriks lain secara
berdampingan, jika keduanya memiliki jumlah baris yang sama.


\>A=random(3,4); A|v'


         0.032444     0.0534171      0.595713      0.564454             1 
          0.83916      0.175552      0.396988       0.83514             2 
        0.0257573      0.658585      0.629832      0.770895             3 

Jika keduanya tidak memiliki jumlah baris yang sama, matriks yang
lebih pendek diisi dengan 0.


Ada pengecualian untuk aturan ini. Bilangan real yang dilampirkan pada
sebuah matriks akan digunakan sebagai kolom yang diisi dengan bilangan
real tersebut.


\>A|1


         0.032444     0.0534171      0.595713      0.564454             1 
          0.83916      0.175552      0.396988       0.83514             1 
        0.0257573      0.658585      0.629832      0.770895             1 

Dimungkinkan untuk membuat matriks vektor baris dan kolom.


\>[v;v]


                1             2             3 
                1             2             3 

\>[v',v']


                1             1 
                2             2 
                3             3 

Tujuan utama dari hal ini adalah untuk menginterpretasikan vektor
ekspresi untuk vektor kolom.


\>"[x,x^2]"(v')


                1             1 
                2             4 
                3             9 

Untuk mendapatkan ukuran A, kita dapat menggunakan fungsi berikut ini.


\>C=zeros(2,4); rows(C), cols(C), size(C), length(C)


    2
    4
    [2,  4]
    4

Untuk vektor, ada length().


\>length(2:10)


    9

Ada banyak fungsi lain yang menghasilkan matriks.


\>ones(2,2)


                1             1 
                1             1 

Ini juga dapat digunakan dengan satu parameter. Untuk mendapatkan
vektor dengan angka selain 1, gunakan yang berikut ini.


\>ones(5)\*6


    [6,  6,  6,  6,  6]

Matriks angka acak juga dapat dibuat dengan acak (uniform
distribution) atau normal (Gauß distribution).


\>random(2,2)


          0.66566      0.831835 
            0.977      0.544258 

Berikut ini adalah fungsi lain yang berguna, yang merestrukturisasi
elemen-elemen matriks menjadi matriks lain.


\>redim(1:9,3,3) // menyusun elemen2 1, 2, 3, ..., 9 ke bentuk matriks 3x3


                1             2             3 
                4             5             6 
                7             8             9 

Dengan fungsi berikut, kita dapat menggunakan fungsi ini dan fungsi
dup untuk menulis fungsi rep(), yang mengulang sebuah vektor sebanyak
n kali.


\>function rep(v,n) := redim(dup(v,n),1,n\*cols(v))


Mari kita uji.


\>rep(1:3,5)


    [1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3]

Fungsi multdup() menduplikasi elemen-elemen sebuah vektor.


\>multdup(1:3,5), multdup(1:3,[2,3,2])


    [1,  1,  1,  1,  1,  2,  2,  2,  2,  2,  3,  3,  3,  3,  3]
    [1,  1,  2,  2,  2,  3,  3]

Fungsi flipx() dan flipy() membalik urutan baris atau kolom dari
sebuah matriks. Misalnya, fungsi flipx() membalik secara horizontal.


\>flipx(1:5) //membalik elemen2 vektor baris


    [5,  4,  3,  2,  1]

Untuk rotasi, Euler memiliki rotleft() dan rotright().


\>rotleft(1:5) // memutar elemen2 vektor baris


    [2,  3,  4,  5,  1]

Fungsi khusus adalah drop(v,i), yang menghapus elemen dengan indeks di
i dari vektor v.


\>drop(10:20,3)


    [10,  11,  13,  14,  15,  16,  17,  18,  19,  20]

Perhatikan bahwa vektor i dalam drop(v,i) merujuk pada indeks elemen
dalam v, bukan nilai elemen. Jika Anda ingin menghapus elemen, Anda
harus menemukan elemen-elemen tersebut terlebih dahulu. Fungsi
indexof(v,x) dapat digunakan untuk menemukan elemen x dalam vektor
terurut v.


\>v=primes(50), i=indexof(v,10:20), drop(v,i)


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47]
    [0,  5,  0,  6,  0,  0,  0,  7,  0,  8,  0]
    [2,  3,  5,  7,  23,  29,  31,  37,  41,  43,  47]

Seperti yang Anda lihat, tidak ada salahnya menyertakan indeks di luar
jangkauan (seperti 0), indeks ganda, atau indeks yang tidak diurutkan.


\>drop(1:10,shuffle([0,0,5,5,7,12,12]))


    [1,  2,  3,  4,  6,  8,  9,  10]

Ada beberapa fungsi khusus untuk mengatur diagonal atau menghasilkan
matriks diagonal.


Kita mulai dengan matriks identitas.


\>A=id(5) // matriks identitas 5x5


                1             0             0             0             0 
                0             1             0             0             0 
                0             0             1             0             0 
                0             0             0             1             0 
                0             0             0             0             1 

Kemudian, kami menetapkan diagonal bawah (-1) ke 1:4.


\>setdiag(A,-1,1:4) //mganti diagonal di bwh diagonal utama (-1 tu 1 d bwhnya diagonal utama)


                1             0             0             0             0 
                1             1             0             0             0 
                0             2             1             0             0 
                0             0             3             1             0 
                0             0             0             4             1 

Perhatikan bahwa kita tidak mengubah matriks A. Kita mendapatkan
sebuah matriks baru sebagai hasil dari setdiag().


Berikut adalah sebuah fungsi yang mengembalikan sebuah matriks
tri-diagonal.


\>function tridiag (n,a,b,c) := setdiag(setdiag(b\*id(n),1,c),-1,a); ...  
\>   tridiag(5,1,2,3)


                2             3             0             0             0 
                1             2             3             0             0 
                0             1             2             3             0 
                0             0             1             2             3 
                0             0             0             1             2 

Diagonal sebuah matriks juga dapat diekstrak dari matriks. Untuk
mendemonstrasikan hal ini, kami merestrukturisasi vektor 1:9 menjadi
matriks 3x3.


\>A=redim(1:9,3,3)


                1             2             3 
                4             5             6 
                7             8             9 

Sekarang kita bisa mengekstrak diagonal.


\>d=getdiag(A,0)


    [1,  5,  9]

Contoh: Kita dapat membagi matriks dengan diagonalnya. Bahasa matriks
memperhatikan bahwa vektor kolom d diterapkan ke matriks baris demi
baris.


\>fraction A/d'


            1         2         3 
          4/5         1       6/5 
          7/9       8/9         1 

# Vektorisasi

Hampir semua fungsi di Euler juga dapat digunakan untuk input matriks
dan vektor, jika hal ini masuk akal.


Sebagai contoh, fungsi sqrt() menghitung akar kuadrat dari semua
elemen vektor atau matriks.


\>sqrt(1:3)


    [1,  1.41421,  1.73205]

Jadi, Anda dapat dengan mudah membuat tabel nilai. Ini adalah salah
satu cara untuk memplot sebuah fungsi (alternatif lainnya menggunakan
ekspresi).


\>x=1:0.01:5; y=log(x)/x^2; // terlalu panjang untuk ditampikan


Dengan ini dan operator titik dua a:delta:b, vektor nilai fungsi dapat
dihasilkan dengan mudah.


Pada contoh berikut, kita membuat vektor nilai t[i] dengan jarak 0.1
dari -1 hingga 1. Kemudian kita membuat vektor nilai dari fungsi


\>t=-1:0.1:1; s=t^3-t


    [0,  0.171,  0.288,  0.357,  0.384,  0.375,  0.336,  0.273,  0.192,
    0.099,  0,  -0.099,  -0.192,  -0.273,  -0.336,  -0.375,  -0.384,
    -0.357,  -0.288,  -0.171,  0]

EMT memperluas operator untuk skalar, vektor, dan matriks dengan cara
yang jelas.


Misalnya, vektor kolom dikalikan vektor baris diperluas menjadi
matriks, jika operator diterapkan. Berikut ini, v' adalah vektor yang
ditransposisikan (vektor kolom).


\>shortest (1:5)\*(1:5)'


         1      2      3      4      5 
         2      4      6      8     10 
         3      6      9     12     15 
         4      8     12     16     20 
         5     10     15     20     25 

Perhatikan, bahwa ini sangat berbeda dengan hasil kali matriks. Hasil
kali matriks dilambangkan dengan sebuah titik "." dalam EMT.


\>(1:5).(1:5)'


    55

Secara default, vektor baris dicetak dalam format ringkas.


\>[1,2,3,4]


    [1,  2,  3,  4]

Untuk matriks, operator khusus . menyatakan perkalian matriks, dan A'
menyatakan transposisi. Matriks 1x1 dapat digunakan seperti halnya
bilangan real.


\>v:=[1,2]; v.v', %^2


    5
    25

Untuk mentransposisikan matriks, kita menggunakan apostrof.


\>v=1:4; v'


                1 
                2 
                3 
                4 

Jadi kita dapat menghitung matriks A dikali vektor b.


\>A=[1,2,3,4;5,6,7,8]; A, A.v'


                1             2             3             4 
                5             6             7             8 
               30 
               70 

Perhatikan bahwa v masih merupakan vektor baris. Jadi v'.v berbeda
dengan v.v'.


\>v'.v


                1             2             3             4 
                2             4             6             8 
                3             6             9            12 
                4             8            12            16 

v.v' menghitung norma v kuadrat untuk vektor baris v. Hasilnya adalah
vektor 1x1, yang berfungsi seperti bilangan real.


\>v.v'


    30

Ada juga normal fungsi (bersama dengan banyak fungsi Aljabar Linier
lainnya).


\>norm(v)^2


    30

Operator dan fungsi mematuhi bahasa matriks Euler.


Berikut ini adalah ringkasan aturannya.


* 
Sebuah fungsi yang diterapkan pada vektor atau matriks diterapkan
* pada setiap elemen.


* 
Operator yang beroperasi pada dua matriks dengan ukuran yang sama
* diterapkan secara berpasangan pada elemen-elemen matriks.


* 
Jika dua matriks memiliki dimensi yang berbeda, keduanya diperluas
* dengan cara yang masuk akal, sehingga memiliki ukuran yang sama.


Misalnya, nilai skalar dikalikan vektor mengalikan nilai dengan setiap
elemen vektor. Atau matriks dikali vektor (dengan *, bukan .)
memperluas vektor ke ukuran matriks dengan menduplikasinya.


Berikut ini adalah kasus sederhana dengan operator ^.


\>[1,2,3]^2


    [1,  4,  9]

Ini adalah kasus yang lebih rumit. Vektor baris dikalikan vektor kolom
memperluas keduanya dengan menduplikasi.


\>v:=[1,2,3]; v\*v'


                1             2             3 
                2             4             6 
                3             6             9 

Perhatikan bahwa hasil kali skalar menggunakan hasil kali matriks,
bukan tanda *!


\>v.v'


    14

Ada banyak fungsi untuk matriks. Kami memberikan daftar singkat. Anda
harus membaca dokumentasi untuk informasi lebih lanjut mengenai
perintah-perintah ini.


  sum,prod menghitung jumlah dan hasil kali dari baris-baris  
  cumsum,cumprod melakukan hal yang sama secara kumulatif  
  menghitung nilai ekstrem dari setiap baris  
  extrema mengembalikan vektor dengan informasi ekstrem  
  diag(A,i) mengembalikan diagonal ke-i  
  setdiag(A,i,v) menetapkan diagonal ke-i  
  id(n) matriks identitas  
  det(A) determinan  
  charpoly(A) polinomial karakteristik  
  eigenvalues(A) nilai eigen  

\>v\*v, sum(v\*v), cumsum(v\*v)


    [1,  4,  9]
    14
    [1,  5,  14]

Operator : menghasilkan vektor baris dengan spasi yang sama, opsional
dengan ukuran langkah.


\>1:4, 1:2:10


    [1,  2,  3,  4]
    [1,  3,  5,  7,  9]

Untuk menggabungkan matriks dan vektor, terdapat operator "|" dan "_".


\>[1,2,3]|[4,5], [1,2,3]\_1 //|menggabung di sebelahnya, \_menggabung di bawahnya


    [1,  2,  3,  4,  5]
                1             2             3 
                1             1             1 

Elemen-elemen dari sebuah matriks disebut dengan "A[i,j]".


\>A:=[1,2,3;4,5,6;7,8,9]; A[2,3]


    6

Untuk vektor baris atau kolom, v[i] adalah elemen ke-i dari vektor
tersebut. Untuk matriks, ini mengembalikan baris ke-i dari matriks.


\>v:=[2,4,6,8]; v[3], A[3]


    6
    [7,  8,  9]

Indeks juga dapat berupa vektor baris dari indeks. : menunjukkan semua
indeks.


\>v[1:2], A[:,2]


    [2,  4]
                2 
                5 
                8 

Bentuk singkat untuk : adalah menghilangkan indeks sepenuhnya.


\>A[,2:3]


                2             3 
                5             6 
                8             9 

Untuk tujuan vektorisasi, elemen-elemen matriks dapat diakses
seolah-olah mereka adalah vektor.


\>A{4}


    4

Sebuah matriks juga dapat diratakan, dengan menggunakan fungsi
redim(). Hal ini diimplementasikan dalam fungsi flatten().


\>redim(A,1,prod(size(A))), flatten(A)


    [1,  2,  3,  4,  5,  6,  7,  8,  9]
    [1,  2,  3,  4,  5,  6,  7,  8,  9]

Untuk menggunakan matriks untuk tabel, mari kita atur ulang ke format
default, dan menghitung tabel nilai sinus dan kosinus. Perhatikan
bahwa sudut dalam radian secara default.


\>defformat; w=0°:45°:360°; w=w'; deg(w)


                0 
               45 
               90 
              135 
              180 
              225 
              270 
              315 
              360 

Sekarang kita menambahkan kolom ke matriks.


\>M = deg(w)|w|cos(w)|sin(w)


                0             0             1             0 
               45      0.785398      0.707107      0.707107 
               90        1.5708             0             1 
              135       2.35619     -0.707107      0.707107 
              180       3.14159            -1             0 
              225       3.92699     -0.707107     -0.707107 
              270       4.71239             0            -1 
              315       5.49779      0.707107     -0.707107 
              360       6.28319             1             0 

Dengan menggunakan bahasa matriks, kita dapat membuat beberapa tabel
dari beberapa fungsi sekaligus.


Pada contoh berikut, kita menghitung t[j]^i untuk i dari 1 hingga n.
Kita mendapatkan sebuah matriks, di mana setiap baris adalah tabel t^i
untuk satu i. Dengan kata lain, matriks tersebut memiliki
elemen-elemen


$$a_{i, j}=t_j^i, \quad 1 \le j \le 101, \quad 1 \le i \le n$$Sebuah fungsi yang tidak berfungsi untuk input vektor harus
"vectorized". Hal ini dapat dicapai dengan kata kunci "map" dalam
definisi fungsi. Kemudian fungsi akan dievaluasi untuk setiap elemen
parameter vektor.


Integrasi numerik integrate() hanya bekerja untuk batas interval
skalar. Jadi kita perlu membuat vektornya.


\>function map f(x) := integrate("x^x",1,x)


Kata kunci "map" membuat vektor fungsi. Fungsi ini sekarang akan
bekerja untuk vektor angka.


\>f([1:5])


    [0,  2.05045,  13.7251,  113.336,  1241.03]

# Sub-Matriks dan Elemen Matriks

Untuk mengakses elemen matriks, gunakan notasi kurung.


\>A=[1,2,3;4,5,6;7,8,9], A[2,2]


                1             2             3 
                4             5             6 
                7             8             9 
    5

Kita dapat mengakses baris lengkap dari sebuah matriks.


\>A[2]


    [4,  5,  6]

Untuk vektor baris atau kolom, ini mengembalikan elemen vektor.


\>v=1:3; v[2]


    2

Untuk memastikan, Anda mendapatkan baris pertama untuk matriks 1xn dan
mxn, tentukan semua kolom menggunakan indeks kedua yang kosong.


\>A[2,]


    [4,  5,  6]

Jika indeks adalah vektor indeks, Euler akan mengembalikan baris-baris
yang sesuai dari matriks.


Di sini kita menginginkan baris pertama dan kedua dari A.


\>A[[1,2]], A[1,2], A[,1:2]


                1             2             3 
                4             5             6 
    2
                1             2 
                4             5 
                7             8 

Kita bahkan dapat menyusun ulang A menggunakan vektor indeks.
Tepatnya, kita tidak mengubah A di sini, tetapi menghitung versi
susunan ulang dari A.


\>A[[3,2,1]]


                7             8             9 
                4             5             6 
                1             2             3 

Trik indeks juga bekerja dengan kolom.


Contoh ini memilih semua baris A dan kolom kedua dan ketiga.


\>A[1:3,2:3]


                2             3 
                5             6 
                8             9 

Untuk singkatan ":" menunjukkan semua indeks baris atau kolom.


\>A[:,3]


                3 
                6 
                9 

Sebagai alternatif, biarkan indeks pertama kosong.


\>A[,2:3]


                2             3 
                5             6 
                8             9 

Kita juga bisa mendapatkan baris terakhir A.


\>A[-1]


    [7,  8,  9]

Sekarang mari kita ubah elemen-elemen dari A dengan memberikan sebuah
submatriks dari A ke suatu nilai. Hal ini sebenarnya mengubah matriks
A yang tersimpan.


\>A[1,1]=4


                4             2             3 
                4             5             6 
                7             8             9 

Kita juga dapat menetapkan nilai pada baris A.


\>A[1]=[-1,-1,-1]


               -1            -1            -1 
                4             5             6 
                7             8             9 

Kami bahkan dapat menetapkan ke sub-matriks jika memiliki ukuran yang
tepat.


\>A[1:2,1:2]=[5,6;7,8]


                5             6            -1 
                7             8             6 
                7             8             9 

Selain itu, beberapa jalan pintas diperbolehkan.


\>A[1:2,1:2]=0


                0             0            -1 
                0             0             6 
                7             8             9 

Peringatan: Indeks di luar batas akan mengembalikan matriks kosong,
atau error message, tergantung pada pengaturan sistem. Standarnya
adalah error message. Namun, ingatlah bahwa indeks negatif dapat
digunakan untuk mengakses elemen-elemen matriks yang dihitung dari
akhir.


\>A[4]


    Row index 4 out of bounds!
    Error in:
    A[4] ...
        ^

# Pengurutan dan Pengocokan

Fungsi sort() mengurutkan vektor baris.


\>sort([5,6,4,8,1,9])


    [1,  4,  5,  6,  8,  9]

Sering kali diperlukan untuk mengetahui indeks vektor yang diurutkan
dalam vektor aslinya. Hal ini dapat digunakan untuk menyusun ulang
vektor lain dengan cara yang sama.


Mari kita mengacak sebuah vektor.


\>v=shuffle(1:10)


    [4,  5,  10,  6,  8,  9,  1,  7,  2,  3]

Indeks berisi urutan v yang tepat.


\>{vs,ind}=sort(v); v[ind]


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

Hal ini juga berlaku untuk vektor string.


\>s=["a","d","e","a","aa","e"]


    a
    d
    e
    a
    aa
    e

\>{ss,ind}=sort(s); ss


    a
    a
    aa
    d
    e
    e

Seperti yang Anda lihat, posisi entri ganda agak acak.


\>ind


    [4,  1,  5,  2,  6,  3]

Fungsi unique mengembalikan daftar terurut dari elemen unik sebuah
vektor.


\>intrandom(1,10,10), unique(%)


    [4,  4,  9,  2,  6,  5,  10,  6,  5,  1]
    [1,  2,  4,  5,  6,  9,  10]

Hal ini juga berlaku untuk vektor string.


\>unique(s)


    a
    aa
    d
    e

# Aljabar Linier

EMT memiliki banyak fungsi untuk menyelesaikan sistem linier, sparse
systems, atau masalah regresi.


Untuk sistem linier Ax=b, Anda dapat menggunakan algoritma Gauss,
matriks invers, atau kecocokan linier. Operator A\b menggunakan versi
algoritma Gauss.


\>A=[1,2;3,4]; b=[5;6]; A\\b


               -4 
              4.5 

Sebagai contoh lain, kita membuat matriks 200x200 dan jumlah barisnya.
Kemudian kita selesaikan Ax = b dengan menggunakan matriks inversnya.
Kita mengukur kesalahan sebagai deviasi maksimal dari semua elemen
dari 1, yang tentu saja merupakan solusi yang benar.


\>A=normal(200,200); b=sum(A); longest totalmax(abs(inv(A).b-1))


      8.790745908981989e-13 

Jika sistem tidak memiliki solusi, kecocokan linier meminimalkan
normal error Ax-b.


\>A=[1,2,3;4,5,6;7,8,9]


                1             2             3 
                4             5             6 
                7             8             9 

Determinan dari matriks ini adalah 0.


\>det(A)


    0

# Matriks Simbolik

Maxima memiliki matriks simbolik. Tentu saja, Maxima dapat digunakan
untuk masalah aljabar linier sederhana. Kita bisa mendefinisikan
matriks untuk Euler dan Maxima dengan &amp;:=, dan kemudian menggunakannya
dalam ekspresi simbolik. Bentuk [...] yang biasa untuk mendefinisikan
matriks dapat digunakan dalam Euler untuk mendefinisikan matriks
simbolik.


\>A &= [a,1,1;1,a,1;1,1,a]; $A


$$\begin{pmatrix}a & 1 & 1 \\ 1 & a & 1 \\ 1 & 1 & a \\ \end{pmatrix}$$\>$&det(A), $&factor(%)


$$\left(a-1\right)^2\,\left(a+2\right)$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-103.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-103.png)

\>$&invert(A) with a=0


$$\begin{pmatrix}-\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\ \frac{1  }{2} & -\frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} & -  \frac{1}{2} \\ \end{pmatrix}$$\>A &= [1,a;b,2]; $A


$$\begin{pmatrix}1 & a \\ b & 2 \\ \end{pmatrix}$$Seperti semua variabel simbolik, matriks ini dapat digunakan dalam
ekspresi simbolik lainnya.


\>$&det(A-x\*ident(2)), $&solve(%,x)


$$\left[ x=\frac{3-\sqrt{4\,a\,b+1}}{2} , x=\frac{\sqrt{4\,a\,b+1}+3  }{2} \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-107.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-107.png)

Nilai eigen juga dapat dihitung secara otomatis. Hasilnya adalah
sebuah vektor dengan dua vektor nilai eigen dan kelipatannya.


\>$&eigenvalues([a,1;1,a])


$$\left[ \left[ a-1 , a+1 \right]  , \left[ 1 , 1 \right]  \right] $$Untuk mengekstrak vektor eigen tertentu, diperlukan pengindeksan yang
cermat.


\>$&eigenvectors([a,1;1,a]), &%[2][1][1]


$$\left[ \left[ \left[ a-1 , a+1 \right]  , \left[ 1 , 1 \right]    \right]  , \left[ \left[ \left[ 1 , -1 \right]  \right]  , \left[   \left[ 1 , 1 \right]  \right]  \right]  \right] $$    
                                   [1, - 1]
    

Matriks simbolik dapat dievaluasi dalam Euler secara numerik seperti
halnya ekspresi simbolik lainnya.


\>A(a=4,b=5)


                1             4 
                5             2 

Dalam ekspresi simbolis, gunakan with.


\>$&A with [a=4,b=5]


$$\begin{pmatrix}1 & 4 \\ 5 & 2 \\ \end{pmatrix}$$Akses ke barisan matriks simbolik bekerja seperti halnya matriks
numerik.


\>$&A[1]


$$\left[ 1 , a \right] $$Ekspresi simbolik dapat berisi sebuah assignment. Dan itu mengubah
matriks A.


\>&A[1,1]:=t+1; $&A


$$\begin{pmatrix}t+1 & a \\ b & 2 \\ \end{pmatrix}$$Terdapat fungsi-fungsi simbolik dalam Maxima untuk membuat vektor dan
matriks. Untuk hal ini, lihat dokumentasi Maxima atau tutorial tentang
Maxima di EMT.


\>v &= makelist(1/(i+j),i,1,3); $v


$$\left[ \frac{1}{j+1} , \frac{1}{j+2} , \frac{1}{j+3} \right] $$\>B &:= [1,2;3,4]; $B, $&invert(B)


$$\begin{pmatrix}-2 & 1 \\ \frac{3}{2} & -\frac{1}{2} \\   \end{pmatrix}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-115.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-115.png)

Hasilnya dapat dievaluasi secara numerik dalam Euler. Untuk informasi
lebih lanjut tentang Maxima, lihat pengantar Maxima.


\>$&invert(B)()


               -2             1 
              1.5          -0.5 

Euler juga memiliki sebuah fungsi yang kuat xinv(), yang melakukan
usaha yang lebih besar dan mendapatkan hasil yang lebih tepat.


Perhatikan, bahwa dengan &amp;:= matriks B telah didefinisikan sebagai
simbolik dalam ekspresi simbolik dan sebagai numerik dalam ekspresi
numerik. Jadi kita dapat menggunakannya di sini.


\>longest B.xinv(B)


                          1                       0 
                          0                       1 

Misalnya, nilai eigen dari A dapat dihitung secara numerik.


\>A=[1,2,3;4,5,6;7,8,9]; real(eigenvalues(A))


    [16.1168,  -1.11684,  0]

Atau secara simbolis. Lihat tutorial tentang Maxima untuk mengetahui
detailnya.


\>$&eigenvalues(@A)


$$\left[ \left[ \frac{15-3\,\sqrt{33}}{2} , \frac{3\,\sqrt{33}+15}{2}   , 0 \right]  , \left[ 1 , 1 , 1 \right]  \right] $$# Nilai Numerik dalam Ekspresi simbolik

Ekspresi simbolik hanyalah sebuah string yang berisi ekspresi. Jika
kita ingin mendefinisikan nilai baik untuk ekspresi simbolik maupun
ekspresi numerik, kita harus menggunakan "&amp;:=".


\>A &:= [1,pi;4,5]


                1       3.14159 
                4             5 

Masih ada perbedaan antara bentuk numerik dan bentuk simbolik. Ketika
mentransfer matriks ke bentuk simbolik, perkiraan pecahan untuk
bilangan real akan digunakan.


\>$&A


$$\begin{pmatrix}1 & \frac{1146408}{364913} \\ 4 & 5 \\ \end{pmatrix}$$Untuk menghindari hal ini, ada fungsi "mxmset(variable)".


\>mxmset(A); $&A


$$\begin{pmatrix}1 & 3.141592653589793 \\ 4 & 5 \\ \end{pmatrix}$$Maxima juga dapat menghitung dengan angka floating point, dan bahkan
dengan floating number yang besar dengan 32 digit. Namun, evaluasinya
jauh lebih lambat.


\>$&bfloat(sqrt(2)), $&float(sqrt(2))


$$1.414213562373095$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-120.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-120.png)

Ketepatan angka floating point yang besar dapat diubah.


\>&fpprec:=100; &bfloat(pi)


    
            3.14159265358979323846264338327950288419716939937510582097494\
    4592307816406286208998628034825342117068b0
    

Variabel numerik dapat digunakan dalam ekspresi simbolik apa pun
dengan menggunakan "@var".


Perhatikan bahwa ini hanya diperlukan, jika variabel telah
didefinisikan dengan ":=" atau "=" sebagai variabel numerik.


\>B:=[1,pi;3,4]; $&det(@B)


$$-5.424777960769379$$# Demo - Suku Bunga

Di bawah ini, kami menggunakan Euler Math Toolbox (EMT) untuk
menghitung suku bunga. Kami melakukannya secara numerik dan simbolis
untuk menunjukkan kepada Anda bagaimana Euler dapat digunakan untuk
memecahkan masalah kehidupan nyata.


Asumsikan Anda memiliki modal awal sebesar 5000 (katakanlah dalam
dolar).


\>K=5000


    5000

Sekarang kita asumsikan suku bunga 3% per tahun. Mari kita tambahkan
satu suku bunga sederhana dan hitung hasilnya.


\>K\*1.03


    5150

Euler juga akan memahami sintaks berikut ini.


\>K+K\*3%


    5150

Tetapi lebih mudah untuk menggunakan faktor


\>q=1+3%, K\*q


    1.03
    5150

Untuk 10 tahun, kita cukup mengalikan faktor-faktor tersebut dan
mendapatkan nilai akhir dengan suku bunga majemuk.


\>K\*q^10


    6719.58189672

Untuk tujuan kita, kita bisa menetapkan formatnya menjadi 2 digit
setelah titik desimal.


\>format(12,2); K\*q^10


        6719.58 

Mari kita cetak angka yang dibulatkan menjadi 2 digit dalam kalimat
lengkap.


\>"Starting from " + K + "$ you get " + round(K\*q^10,2) + "$."


    Starting from 5000$ you get 6719.58$.

Bagaimana jika kita ingin mengetahui hasil antara dari tahun ke-1
hingga tahun ke-9? Untuk hal ini, bahasa matriks Euler sangat
membantu. Anda tidak perlu menulis perulangan, tetapi cukup masukkan


\>K\*q^(0:10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

Bagaimana keajaiban ini bekerja? Pertama, ekspresi 0:10 mengembalikan
sebuah vektor bilangan bulat.


\>short 0:10


    [0,  1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

Kemudian semua operator dan fungsi dalam Euler dapat diterapkan pada
vektor elemen demi elemen. Jadi


\>short q^(0:10)


    [1,  1.03,  1.0609,  1.0927,  1.1255,  1.1593,  1.1941,  1.2299,
    1.2668,  1.3048,  1.3439]

adalah vektor faktor q^0 hingga q^10. Ini dikalikan dengan K, dan kita
mendapatkan vektor nilai.


\>VK=K\*q^(0:10);


Tentu saja, cara yang realistis untuk menghitung suku bunga ini adalah
dengan membulatkan ke sen terdekat setelah setiap tahun. Mari kita
tambahkan fungsi untuk ini.


\>function oneyear (K) := round(K\*q,2)


Mari kita bandingkan kedua hasil tersebut, dengan dan tanpa
pembulatan.


\>longest oneyear(1234.57), longest 1234.57\*q


                    1271.61 
                  1271.6071 

Sekarang tidak ada rumus sederhana untuk tahun ke-n, dan kita harus
mengulang selama bertahun-tahun. Euler menyediakan banyak solusi untuk
ini.


Cara termudah adalah iterasi fungsi, yang mengulang fungsi yang
diberikan beberapa kali.


\>VKr=iterate("oneyear",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

Kita bisa mencetaknya dengan cara yang bersahabat, menggunakan format
kami dengan angka desimal yang tetap.


\>VKr'


        5000.00 
        5150.00 
        5304.50 
        5463.64 
        5627.55 
        5796.38 
        5970.27 
        6149.38 
        6333.86 
        6523.88 
        6719.60 

Untuk mendapatkan elemen tertentu dari vektor, kita menggunakan indeks
dalam tanda kurung siku.


\>VKr[2], VKr[1:3]


        5150.00 
        5000.00     5150.00     5304.50 

Yang mengejutkan, kita juga dapat menggunakan vektor indeks. Ingatlah
bahwa 1:3 menghasilkan vektor [1,2,3].


Mari kita bandingkan elemen terakhir dari nilai yang dibulatkan dengan
nilai penuh.


\>VKr[-1], VK[-1]


        6719.60 
        6719.58 

Perbedaannya sangat kecil.


# Menyelesaikan Persamaan

Sekarang kita ambil fungsi yang lebih maju, yang menambahkan tingkat
uang tertentu setiap tahun.


\>function onepay (K) := K\*q+R


Kita tidak perlu menentukan q atau R untuk definisi fungsi. Hanya jika
kita menjalankan perintah, kita harus mendefinisikan nilai-nilai ini.
Kami memilih R = 200.


\>R=200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5350.00     5710.50     6081.82     ...

Bagaimana jika kita menghapus jumlah yang sama setiap tahun?


\>R=-200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

Kami melihat bahwa uangnya berkurang. Jelas, jika kita hanya
mendapatkan 150 bunga di tahun pertama, tetapi menghapus 200, kita
kehilangan uang setiap tahun.


Bagaimana kita dapat menentukan berapa tahun uang itu akan bertahan?
Kita harus menulis perulangan untuk ini. Cara termudah adalah dengan
melakukan perulangan yang cukup lama.


\>VKR=iterate("onepay",5000,50)


    Real 1 x 51 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

Dengan menggunakan bahasa matriks, kita dapat menentukan nilai negatif
pertama dengan cara berikut.


\>min(nonzeros(VKR<0))


          48.00 

Alasannya adalah karena nonzeros(VKR&lt;0) mengembalikan vektor dengan
indeks i, di mana VKR[i]&lt;0, dan min menghitung indeks minimal.


Karena vektor selalu dimulai dengan indeks 1, maka jawabannya adalah
47 tahun.


Fungsi iterate() memiliki satu trik lagi. Fungsi ini dapat menerima
kondisi akhir sebagai argumen. Kemudian fungsi ini akan mengembalikan
nilai dan jumlah iterasi.


\>{x,n}=iterate("onepay",5000,till="x<0"); x, n,


         -19.83 
          47.00 

Mari kita coba menjawab pertanyaan yang lebih ambigu. Anggaplah kita
tahu bahwa nilainya adalah 0 setelah 50 tahun. Berapakah tingkat suku
bunganya?


Ini adalah pertanyaan yang hanya bisa dijawab secara numerik. Di bawah
ini, kami akan menurunkan rumus yang diperlukan. Kemudian Anda akan
melihat bahwa tidak ada rumus yang mudah untuk suku bunga. Namun untuk
saat ini, kita akan mencari solusi numerik.


Langkah pertama adalah mendefinisikan sebuah fungsi yang melakukan
iterasi sebanyak n kali. Kita tambahkan semua parameter ke fungsi ini.


\>function f(K,R,P,n) := iterate("x\*(1+P/100)+R",K,n;P,R)[-1]


Perulangannya sama seperti di atas


$$x_{n+1}=x_n\cdot\left(1+\frac{P}{100}\right) + R$$Tetapi kita tidak lagi menggunakan nilai global R dalam ekspresi kita.
Fungsi-fungsi seperti iterate() memiliki trik khusus dalam Euler. Anda
bisa mengoper nilai variabel dalam ekspresi sebagai parameter titik
koma. Dalam hal ini P dan R.


Selain itu, kita hanya tertarik pada nilai terakhir. Jadi kita
mengambil indeks [-1].


Mari kita coba sebuah tes.


\>f(5000,-200,3,47)


         -19.83 

Sekarang kita bisa menyelesaikan masalah kita.


\>solve("f(5000,-200,x,50)",3)


           3.15 

Rutin penyelesaian menyelesaikan ekspresi = 0 untuk variabel x.
Jawabannya adalah 3,15% per tahun. Kita mengambil nilai awal 3% untuk
algoritma ini. Fungsi solve() selalu membutuhkan nilai awal.


Kita dapat menggunakan fungsi yang sama untuk menyelesaikan pertanyaan
berikut: Berapa banyak yang dapat kita hapus per tahun sehingga modal
awal habis setelah 20 tahun dengan asumsi tingkat bunga 3% per tahun.


\>solve("f(5000,x,3,20)",-200)


        -336.08 

Perhatikan bahwa Anda tidak dapat menyelesaikan jumlah tahun, karena
fungsi kita mengasumsikan n sebagai nilai bilangan bulat.


## Solusi Simbolik untuk Masalah Suku Bunga

Kita dapat menggunakan bagian simbolik dari Euler untuk mempelajari
masalah ini. Pertama, kita mendefinisikan fungsi onepay() secara
simbolik.


\>function op(K) &= K\*q+R; $&op(K)


$$R+q\,K$$Sekarang kita bisa mengulangi hal ini.


\>$&op(op(op(op(K)))), $&expand(%)


$$q^3\,R+q^2\,R+q\,R+R+q^4\,K$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-125.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-125.png)

Kita melihat sebuah pola. Setelah n periode, kita memiliki


$$K_n=q^n K + R (1+q+\ldots+q^{n-1})=q^n K + \frac{q^n-1}{q-1} R$$Rumus tersebut adalah rumus untuk jumlah geometris, yang dikenal
dengan Maxima.


\>&sum(q^k,k,0,n-1); $& % = ev(%,simpsum)


$$\sum_{k=0}^{n-1}{q^{k}}=\frac{q^{n}-1}{q-1}$$Ini sedikit rumit. Penjumlahan dievaluasi dengan flag "simpsum" untuk
menguranginya menjadi hasil bagi.


Mari kita buat sebuah fungsi untuk ini.


\>function fs(K,R,P,n) &= (1+P/100)^n\*K + ((1+P/100)^n-1)/(P/100)\*R; $&fs(K,R,P,n)


$$\frac{100\,\left(\left(\frac{P}{100}+1\right)^{n}-1\right)\,R}{P}+K  \,\left(\frac{P}{100}+1\right)^{n}$$Fungsi ini melakukan hal yang sama seperti fungsi f kita sebelumnya.
Tetapi fungsi ini lebih efektif.


\>longest f(5000,-200,3,47), longest fs(5000,-200,3,47)


         -19.82504734650985 
         -19.82504734652684 

Sekarang kita dapat menggunakannya untuk menanyakan waktu n. Kapan
modal kita habis? Perkiraan awal kita adalah 30 tahun.


\>solve("fs(5000,-330,3,x)",30)


          20.51 

Jawaban ini mengatakan bahwa nilai tersebut akan menjadi negatif
setelah 21 tahun.


Kita juga bisa menggunakan sisi simbolis dari Euler untuk menghitung
rumus pembayaran.


Asumsikan kita mendapatkan pinjaman sebesar K, dan membayar n kali
pembayaran sebesar R (dimulai setelah tahun pertama) sehingga
menyisakan sisa utang sebesar Kn (pada saat pembayaran terakhir).
Rumus untuk hal ini adalah sebagai berikut


\>equ &= fs(K,R,P,n)=Kn; $&equ


$$\frac{100\,\left(\left(\frac{P}{100}+1\right)^{n}-1\right)\,R}{P}+K  \,\left(\frac{P}{100}+1\right)^{n}={\it Kn}$$Biasanya rumus ini diberikan dalam bentuk


$$i=\frac{P}{100}$$\>equ &= (equ with P=100\*i); $&equ


$$\frac{\left(\left(i+1\right)^{n}-1\right)\,R}{i}+\left(i+1\right)^{  n}\,K={\it Kn}$$Kita dapat menyelesaikan laju R secara simbolis.


\>$&solve(equ,R)


$$\left[ R=\frac{i\,{\it Kn}-i\,\left(i+1\right)^{n}\,K}{\left(i+1  \right)^{n}-1} \right] $$Seperti yang dapat Anda lihat dari rumusnya, fungsi ini mengembalikan
kesalahan floating point untuk i = 0. Euler tetap memplotnya.


Tentu saja, kita memiliki batas berikut.


\>$&limit(R(5000,0,x,10),x,0)


$$\lim_{x\rightarrow 0}{R\left(5000 , 0 , x , 10\right)}$$Jelasnya, tanpa bunga kita harus membayar kembali 10 suku bunga 500.


Persamaan ini juga dapat diselesaikan untuk n. Akan terlihat lebih
baik jika kita menerapkan beberapa penyederhanaan.


\>fn &= solve(equ,n) | ratsimp; $&fn


$$\left[ n=\frac{\log \left(\frac{R+i\,{\it Kn}}{R+i\,K}\right)}{  \log \left(i+1\right)} \right] $$---



Excercise


## R.2 Integer Exponents

~&gt; Menyederhanakan


Soal 49


$$\left(\frac{24a^{10}b^{-8}c^7}{12a^6b^{-3}c^5}\right)^{-5}$$\>"Jawaban Soal 49", $&((24\*a^10\*b^-8\*c^7)/(12\*a^6\*b^-3\*c^5))^-5


    Jawaban Soal 49

$$\frac{b^{25}}{32\,a^{20}\,c^{10}}$$Soal 50


$$\left(\frac{125p^{12}q^{-14}r^{22}}{25p^8q^6r^{-15}}\right)^{-4}$$\>"Jawaban Soal 50", $&((125\*p^12\*q^-14\*r^22)/(25\*p^8\*q^6\*r^-15))^-4


    Jawaban Soal 50

$$\frac{q^{80}}{625\,p^{16}\,r^{148}}$$~&gt; Menghitung


Soal 87


$$5\cdot3+8\cdot3^2+4(6-2)$$\>"Jawaban Soal 87", $&5\*3+8\*3^2+4\*(6-2)


    Jawaban Soal 87

$$103$$Soal 91


$$\frac{4(8-6)^2-4\cdot3+2\cdot8}{3^1+19^0}$$\>"Jawaban Soal 91", $&(4\*(8-6)^2-4\*3+2\*8)/(3^1+19^0)


    Jawaban Soal 91

$$5$$Soal 92


$$\frac{[4(8-6)^2+4](3-2\cdot8)}{2^2(2^3+5)}$$\>"Jawaban Soal 92", $&((4\*(8-6)^2+4)\*(3-2\*8))/(2^2\*(2^3+5))


    Jawaban Soal 92

$$-5$$## R.3 Addition, Subtraction, and Multiplication of Polynomials

Soal 8


$$(2x^2+12xy-11)+(6x^2-2x+4)+(-x^2-y-2)$$\>"Jawaban Soal 8", $&(2\*x^2+12\*x\*y-11)+(6\*x^2-2\*x+4)+(-x^2-y-2)


    Jawaban Soal 8

$$12\,x\,y-y+7\,x^2-2\,x-9$$Soal 10


$$(5x^2+4xy-3y^2+2)-(9x^2-4xy+2y^2-1)$$\>"Jawaban Soal 10", $&(5\*x^2+4\*x\*y-3\*y^2+2)-(9\*x^2-4\*x\*y+2\*y^2-1)


    Jawaban Soal 10

$$-5\,y^2+8\,x\,y-4\,x^2+3$$Soal 13


$$(3a^2)(-7a^4)$$\>"Jawaban Soal 13", $&(3\*a^2)\*(-7\*a^4)


    Jawaban Soal 13

$$-21\,a^6$$Soal 44


$$(5x+2y+3)(5x+2y-3)$$\>"Jawaban Soal 44", $&ratsimp((5\*x+2\*y+3)\*(5\*x+2\*y-3))


    Jawaban Soal 44

$$4\,y^2+20\,x\,y+25\,x^2-9$$Soal 45


$$(x+1)(x-1)(x^2+1)$$\>"Jawaban Soal 45", $&ratsimp((x+1)\*(x-1)\*(x^2+1))


    Jawaban Soal 45

$$x^4-1$$## R.4 Factoring

~&gt; Memfaktorkan


Soal 56


$$25ab^4-25az^4$$\>"Jawaban Soal 56", $&factor(25\*a\*b^4-25\*a\*z^4)


    Jawaban Soal 56

$$-25\,a\,\left(z-b\right)\,\left(z+b\right)\,\left(z^2+b^2\right)$$Soal 66


$$5a^2-10ab+5b^2$$\>"Jawaban Soal 66", $&factor(5\*a^2-10\*a\*b+5\*b^2)


    Jawaban Soal 66

$$5\,\left(b-a\right)^2$$Soal 69


$$m^3-216$$\>"Jawaban Soal 69", $&factor(m^3-216)


    Jawaban Soal 69

$$\left(m-6\right)\,\left(m^2+6\,m+36\right)$$Soal 101


$$4ax^2+20ax-56a$$\>"Jawaban Soal 101", $&factor(4\*a\*x^2+20\*a\*x-56\*a)


    Jawaban Soal 101

$$4\,a\,\left(x-2\right)\,\left(x+7\right)$$Soal 126


$$x^2-5x+\frac{25}{4}$$\>"Jawaban Soal 126", $&factor(x^2-5\*x+(25/4))


    Jawaban Soal 126

$$\frac{\left(2\,x-5\right)^2}{4}$$## R.5 The Basic of Equation Solving

~&gt; Mencari Solusi


Soal 32


$$9(2x+8)=20-(x+5)$$\>"Jawaban Soal 32", $&solve(9\*(2\*x+8)=20-(x+5), x)


    Jawaban Soal 32

$$\left[ x=-3 \right] $$Soal 33


$$4(3y-1)-6=5(y+2)$$\>"Jawaban Soal 33", $&solve(4\*(3\*y-1)-6=5\*(y+2), y)


    Jawaban Soal 33

$$\left[ y=\frac{20}{7} \right] $$Soal 56


$$t^2=25$$\>"Jawaban Soal 56", $&solve(t^2=25, t)


    Jawaban Soal 56

$$\left[ t=-5 , t=5 \right] $$Soal 82


$$6[4(8-y)-5(9+3y)]-21=-7[3(7+4y)-4]$$\>"Jawaban Soal 82", $&solve(6\*(4\*(8-y)-5\*(9+3\*y))-21=-7\*(3\*(7+4\*y)-4), y)


    Jawaban Soal 82

$$\left[ y=\frac{2}{3} \right] $$Soal 85


$$(5x^2+6x)(12x^2-5x-2)=0$$\>"Jawaban Soal 85", $&solve((5\*x^2+6\*x)\*(12\*x^2-5\*x-2)=0, x)


    Jawaban Soal 85

$$\left[ x=-\frac{1}{4} , x=\frac{2}{3} , x=-\frac{6}{5} , x=0   \right] $$## R.6 Rational Expression

~&gt; Menyederhanakan


Soal 12


$$\frac{y^5-5y^4+4y^3}{y^3-6y^2+8y}$$\>"Jawaban Soal 12", $&ratsimp((y^5-5\*y^4+4\*y^3)/(y^3-6\*y^2+8\*y))


    Jawaban Soal 12

$$\frac{y^3-y^2}{y-2}$$Soal 29


$$\frac{(x-y)^2-z^2}{(x+y)^2-z^2}/\frac{x-y+z}{x+y-z}$$\>"Jawaban Soal 29", $&ratsimp((((x-y)^2-z^2)/((x+y)^2-z^2))/((x-y+z)/(x+y-z)))


    Jawaban Soal 29

$$\frac{-z-y+x}{z+y+x}$$Soal 39


$$\frac{y}{y^2-y-20}-\frac{2}{y+4}$$\>"Jawaban Soal 39", $&ratsimp((y/(y^2-y-20))-(2/(y+4)))


    Jawaban Soal 39

$$\frac{10-y}{y^2-y-20}$$Soal 59


$$\frac{c+\frac{8}{c^2}}{1+\frac2c}$$\>"Jawaban Soal 59", $&ratsimp((c+8/c^2)/(1+2/c))


    Jawaban Soal 59

$$\frac{c^2-2\,c+4}{c}$$Soal 71


$$\frac{(x+h)^2-x^2}{h}$$\>"Jawaban Soal 71", $&ratsimp(((x+h)^2-x^2)/h)


    Jawaban Soal 71

$$2\,x+h$$## R.7 Rational Notation and Rational Exponents

~&gt; Menyederhanakan


Soal 9


$$\sqrt[4]{81x^8}$$\>"Jawaban Soal 9", $&(81\*x^8)^(1/4)


    Jawaban Soal 9

$$3\,x^2$$Soal 34


$$\sqrt[3]{4(x+1)^2}\sqrt[3]{18(x+1)^2}$$\>"Jawaban Soal 34", $&((4\*(x+1)^2)^(1/3))\*((18\*(x+1)^2)^(1/3))


    Jawaban Soal 34

$$4^{\frac{1}{3}}\,18^{\frac{1}{3}}\,\left(x+1\right)^{\frac{4}{3}}$$Soal 44


$$\sqrt[3]{\frac{2yz}{250z^4}}$$\>"Jawaban Soal 44", $&((2\*y\*z)/(250\*z^4))^(1/3)


    Jawaban Soal 44

$$\frac{y^{\frac{1}{3}}}{5\,z}$$Soal 54


$$(\sqrt{6}-4\sqrt{7})(3\sqrt{6}+2\sqrt{7})$$\>"Jawaban Soal 54", $&ratsimp((6^(1/2)-4\*7^(1/2))\*(3\*6^(1/2)+2\*7^(1/2)))


    Jawaban Soal 54

$$-10\,\sqrt{6}\,\sqrt{7}-38$$Soal 125


$$\sqrt{1+x^2}+\frac{1}{\sqrt{1+x^2}}$$\>"Jawaban Soal 125", $&ratsimp((1+x^2)^(1/2)+(1/(1+x^2)^(1/2)))


    Jawaban Soal 125

$$\frac{x^2+2}{\sqrt{x^2+1}}$$## Chapter R Test

~&gt; Menyederhanakan


Soal 12


$$(2y^2)^3(3y^4)^2$$\>"Jawaban Soal 12", $&((2\*y^2)^3)\*(3\*y^4)^2


    Jawaban Soal 12

$$72\,y^{14}$$Soal 17


$$\frac{\frac{x}{y}-\frac{y}{x}}{x+y}$$\>"Jawaban Soal 17", $&ratsimp((x/y)-(y/x))/(x+y)


    Jawaban Soal 17

$$\frac{x^2-y^2}{x\,y\,\left(y+x\right)}$$~&gt; Memfaktorkan


Soal 26


$$x^3+10x^2+25x$$\>"Jawaban Soal 26", $&factor(x^3+10\*x^2+25\*x)


    Jawaban Soal 26

$$x\,\left(x+5\right)^2$$~&gt; Mencari Solusi


Soal 29


$$3(y-5)+6=8-(y+2)$$\>"Jawaban Soal 29", $&solve(3\*(y-5)+6=8-(y+2))


    Jawaban Soal 29

$$\left[ y=\frac{15}{4} \right] $$~&gt; Menghitung dan Menyedehanakan


Soal 32


$$\frac{x^2+x-6}{x^2+8x+15}\cdot\frac{x^2-25}{x^2-4x+4}$$\>"Jawaban Soal 32",  ...  
\>   $&((x^2+x-6)/(x^2+8\*x+15))\*((x^2-25)/(x^2-4\*x+4)), $&ratsimp(%)


    Jawaban Soal 32

$$\frac{x-5}{x-2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-205.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-205.png)

## 2.3 The Composition of Function

~&gt;Diberikan fungsi sebagai berikut:


$$f(x)=3x+1,\ g(x)=x^2-2x-6,\ h(x)=x^3$$\>function f(x)&=3\*x+1; function g(x)&=x^2-2\*x-6; function h(x)&=x^3;


Soal 1


$$(f\circ g)(-1)$$\>"Jawaban Soal 1", $f(x) with x=g(x), $&ratsimp(%), $% with x=-1


    Jawaban Soal 1

$$-8$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-209.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-209.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-210.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-210.png)

Soal 4


$$(g\circ h)\left(\frac12\right)$$\>"Jawaban Soal 4", $g(x) with x=h(x), $% with x=1/2


    Jawaban Soal 4

$$-\frac{399}{64}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-213.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-213.png)

Soal 10


$$(g\circ g)(3)$$\>"Jawaban Soal 10", $g(x) with x=g(x), $&ratsimp(%), $% with x=3


    Jawaban Soal 10

$$9$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-216.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-216.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-217.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-217.png)

~&gt; Cari nilai serta domain dari


$$(f\circ g)(x)\ dan\ (g\circ f)(x)$$Soal 17


$$f(x)=x+3,\ g(x)=x-3$$\>function g(x)&=x-3; function f(x)&=x+3; 

\>"Jawaban Soal 17"


    Jawaban Soal 17

$$(f\circ g)(x)=$$\>$f(x) with x=g(x)


$$x$$Domainnya adalah


$$D_{f\circ g}=\left\{x\in\mathbb{R}\right\}$$$$(g\circ f)(x)=$$\>$g(x) with x=f(x)


$$x$$Domainnya adalah


$$D_{g\circ f}=\left\{x\in\mathbb{R}\right\}$$Soal 35


$$f(x)=\frac{1-x}{x},\ g(x)=\frac{1}{1+x}$$\>function f(x)&=(1-x)/x; function g(x)&=1/(1+x);

\>"Jawaban Soal 35"


    Jawaban Soal 35

$$(f\circ g)(x)=$$\>$f(x) with x=g(x), $&ratsimp(%)


$$x$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-229.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-229.png)

Domainnya adalah


$$D_{f\circ g}=\left\{x\in\mathbb{R}\right\}$$$$(g\circ f)(x)=$$\>$g(x) with x=f(x), $&ratsimp(%)


$$x$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-233.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-233.png)

Doaminnya adalah


$$D_{g\circ f}=\left\{x\in\mathbb{R}\right\}$$## 3.1 Quadratic Functions and Equations; Inequalities

~&gt; Menyederhanakan


Soal 15


$$(12+3i)+(-8+5i)$$\>"Jawaban Soal 15", $&(12+3\*I)+(-8+5\*I)


    Jawaban Soal 15

$$8\,i+4$$Soal 20


$$(7-\sqrt{-36})+(2+\sqrt{-9})$$\>"Jawaban Soal 20", $&(7-(-36)^(1/2))+(2+(-9)^(1/2))


    Jawaban Soal 20

$$9-3\,i$$Soal 32


$$\sqrt{-49}\cdot\sqrt{-9}$$\>"Jawaban Soal 32", $&(-49)^(1/2)\*(-9)^(1/2)


    Jawaban Soal 32

$$-21$$Soal 35


$$7i(2-5i)$$\>"Jawaban Soal 35", $&ratsimp(7\*I\*(2-5\*I))


    Jawaban Soal 35

$$14\,i+35$$Soal 87


$$(5i)^4$$\>"Jawaban Soal 87", $&(5\*I)^4


    Jawaban Soal 87

$$625$$## 3.2 Quadratic Equations, Functions, Zeros, and Models

~&gt;Mencari Solusi


Soal 48


$$2t^2-5t=1$$\>"Jawaban Soal 48", $&solve(2\*t^2-5\*t=1, t)


    Jawaban Soal 48

$$\left[ t=\frac{5-\sqrt{33}}{4} , t=\frac{\sqrt{33}+5}{4} \right] $$Soal 79


$$x^4-3x^2+2=0$$\>"Jawaban Soal 79", $&solve(x^4-3\*x^2+2, x)


    Jawaban Soal 79

$$\left[ x=-\sqrt{2} , x=\sqrt{2} , x=-1 , x=1 \right] $$Soal 86


$$2x-9\sqrt x+4=0$$\>"Jawaban Soal 86", $&solve(2\*x-9\*x^(1/2)+4=0, x)


    Jawaban Soal 86

$$\left[ x=\frac{9\,\sqrt{x}-4}{2} \right] $$Soal 93


$$(2t^2+t)^2-4(t^2+t)+3=0$$\>"Jawaban Soal 93", $&solve((2\*t^2+t)^2-4\*(2\*t^2+t)+3=0, t)


    Jawaban Soal 93

$$\left[ t=\frac{1}{2} , t=-1 , t=1 , t=-\frac{3}{2} \right] $$Soal 128


$$\left(x-\frac15\right)\left(x^2-\frac14\right)+\left(x-\frac15\right)\left(x^2-\frac18\right)=0$$\>"Jawaban Soal 128", $&solve((x-1/5)\*(x^2-1/4)+(x-1/5)\*(x^2-1/8)=0, x)


    Jawaban Soal 128

$$\left[ x=-\frac{\sqrt{3}}{4} , x=\frac{\sqrt{3}}{4} , x=\frac{1}{5}   \right] $$## 3.4 Solving Rational Equations and Radical Equations

~&gt; Mencari Solusi


Soal 10


$$x-\frac{12}{x}=1$$\>"Jawaban Soal 10", $&solve(x-12/x=1, x)


    Jawaban Soal 10

$$\left[ x=-3 , x=4 \right] $$Soal 16


$$\frac{2}{x^2-9}+\frac{5}{x-3}=\frac{3}{x+3}$$\>"Jawaban Soal 16", $&solve(2/(x^2-9)+5/(x-3)=3/(x+3), x)


    Jawaban Soal 16

$$\left[ x=-13 \right] $$Soal 34


$$\sqrt{5-x}=1$$\>"Jawaban Soal 34", $&solve((5-x)^(1/2)=1, x)


    Jawaban Soal 34

$$\left[ x=4 \right] $$Soal 94


$$\frac{x+3}{x+2}-\frac{x+4}{x+3}=\frac{x+5}{x+4}-\frac{x+6}{x+5}$$\>"Jawaban Soal 94", $&solve((x+3)/(x+2)-(x+4)/(x+3)=(x+5)/(x+4)-(x+6)/(x+5), x)


    Jawaban Soal 94

$$\left[ x=-\frac{7}{2} \right] $$Soal 96


$$\sqrt{15+\sqrt{2x+80}}=5$$\>"Jawaban Soal 96", $&solve((15+(2\*x+80)^(1/2))^(1/2)=5, x)


    Jawaban Soal 96

$$\left[ x=10 \right] $$## 3.5 Solving Equations and Inequalities with Absolute Value

\>&load(fourier\_elim)


    
            C:/Program Files/Euler x64/maxima/share/maxima/5.35.1/share/f\
    ourier_elim/fourier_elim.lisp
    

~&gt; Mencari Solusi


Soal 25


$$|3x+1|-4=-1$$\>"Jawaban Soal 25", $&solve(abs(3\*x+1)-4=-1, x)  ...  
\>   //belum tahu cara menampilkan solusi x di EMT


    Jawaban Soal 25

$$\left[ \left| 3\,x+1\right| =3 \right] $$'


\>"Jawaban Soal 30", $&solve(9-abs(x-2)=7) ...  
\>   //belum tahu cara menampilkan solusi x di EMT


    Jawaban Soal 30

$$\left[ \left| x-2\right| =2 \right] $$Soal 43


$$|2x|\ge 6$$\>"Jawaban Soal 43", $&fourier\_elim(abs(2\*x)\>=6, [x])


    Jawaban Soal 43

$$\left[ x=3 \right] \lor \left[ x=-3 \right] \lor \left[ 3<x   \right] \lor \left[ x<-3 \right] $$Soal 60


$$\left|\frac{2x-1}{3}\right|\ge \frac56$$\>"Jawaban Soal 60", $&fourier\_elim(abs((2\*x-1)/3)\>=5/6, [x])


    Jawaban Soal 60

$$\left[ x=-\frac{3}{4} \right] \lor \left[ x=\frac{7}{4} \right]   \lor \left[ x<-\frac{3}{4} \right] \lor \left[ \frac{7}{4}<x   \right] $$Soal 71


$$|3x-1|>5x-2$$\>"Jawaban Soal 71", $&fourier\_elim(abs(3\*x-1)\>5\*x-2, [x])


    Jawaban Soal 71

$$\left[ x=\frac{2}{5} \right] \lor \left[ \frac{2}{5}<x , x<\frac{1  }{2} \right] \lor \left[ x<\frac{2}{5} \right] $$## 4.1 Polynomial Functions and Models

~&gt; Mencari Nilai 0


Soal 36


$$f(x)=(x^2-5x+6)^2$$\>"Jawaban Soal 36", $&solve((x^2-5\*x+6)^2, x)


    Jawaban Soal 36

$$\left[ x=3 , x=2 \right] $$~&gt; Mencari Solusi


Soal 61


$$2y-3\ge 1-y+5$$\>"Jawaban Soal 61", $&fourier\_elim(2\*y-3\>=1-y+5, [y])


    Jawaban Soal 61

$$\left[ y=3 \right] \lor \left[ 3<y \right] $$Soal 62


$$(x-2)(x+5)>x(x-3)$$\>"Jawaban Soal 62", $&fourier\_elim((x-2)\*(x+5)\>x\*(x-3), [x])


    Jawaban Soal 62

$$\left[ \frac{5}{3}<x \right] $$Soal 63


$$|x+6|\ge 7$$\>"Jawaban Soal 63", $&fourier\_elim(abs(x+6)\>=7, [x])


    Jawaban Soal 63

$$\left[ x=1 \right] \lor \left[ x=-13 \right] \lor \left[ x<-13   \right] \lor \left[ 1<x \right] $$Soal 64


$$\left|x+\frac14\right|\le \frac23$$\>"Jawaban Soal 64", $&fourier\_elim(abs(x+1/4)<=2/3, [x])


    Jawaban Soal 64

$$\left[ x=-\frac{11}{12} \right] \lor \left[ x=\frac{5}{12} \right]   \lor \left[ -\frac{11}{12}<x , x<\frac{5}{12} \right] $$## 4.3 Polynomial Division

~&gt; Memfaktorkan dan Mencari Solusi


Soal 40


$$f(x)=x^3+5x^2-2x-24$$\>"Jawaban Soal 40", $&factor(x^3+5\*x^2-2\*x-24), $&solve(%, x)


    Jawaban Soal 40

$$\left[ x=-4 , x=-3 , x=2 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-286.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-286.png)

Soal 45


$$f(x)=x^4-7x^3+9x^2+27x-54$$\>"Jawaban Soal 45", $&factor(x^4-7\*x^3+9\*x^2+27\*x-54), $&solve(%, x)


    Jawaban Soal 45

$$\left[ x=-2 , x=3 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-289.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-289.png)

Soal 48


$$f(x)=x^4+11x^3+41x^2+61x+30$$\>"Jawaban Soal 48", $&factor(x^4+11\*x^3+41\*x^2+61\*x+30), $&solve(%, x)


    Jawaban Soal 48

$$\left[ x=-5 , x=-3 , x=-2 , x=-1 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-292.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-292.png)

~&gt; Mencari Solusi


Soal 67


$$\frac{2x^2}{x^2-1}+\frac{4}{x+3}=\frac{12x-4}{x^3+3x^2-x-3}$$\>"Jawaban Soal 67",  ...  
\>   $&solve(2\*x^2/(x^2-1)+4/(x+3)=(12\*x-4)/(x^3+3\*x^2-x-3))


    Jawaban Soal 67

$$\left[ x=-6 , x=0 \right] $$Soal 68


$$\frac{6x^2}{x^2+11}+\frac{60}{x^3-7x^2+11x-77}=\frac{1}{x-7}$$\>"Jawaban Soal 68",  ...  
\>   $&solve(6\*x^2/(x^2+11)+60/(x^3-7\*x^2+11\*x-77)=1/(x-7))


    Jawaban Soal 68

$$\left[ x=\frac{7}{6} , x=-1 \right] $$---

---

---

# Menggambar Grafik 2D dengan EMT

Notebook ini menjelaskan tentang cara menggambar berbagaikurva dan
grafik 2D dengan software EMT. EMT menyediakan fungsi plot2d() untuk
menggambar berbagai kurva dan grafik dua dimensi (2D).


## Plot Dasar

Ada fungsi plot yang sangat mendasar. Ada koordinat layar, yang selalu
berkisar dari 0 hingga 1024 di setiap sumbu, tidak peduli apakah
layarnya persegi atau tidak. Terdapat koordinat plot, yang dapat
diatur dengan setplot(). Pemetaan antara koordinat tergantung pada
jendela plot saat ini. Sebagai contoh, default shrinkwindow()
menyisakan ruang untuk label sumbu dan judul plot.


Pada contoh, kita hanya menggambar beberapa garis acak dalam berbagai
warna. Untuk detail mengenai fungsi-fungsi ini, pelajari fungsi-fungsi
inti dari EMT.


\>clg; // clear screen

\>window(0,0,1024,1024); // use all of the window

\>setplot(0,1,0,1); // set plot coordinates

\>hold on; // start overwrite mode

\>n=100; X=random(n,2); Y=random(n,2);  // get random points

\>colors=rgb(random(n),random(n),random(n)); // get random colors

\>loop 1 to n; color(colors[#]); plot(X[#],Y[#]); end; // plot

\>hold off; // end overwrite mode

\>insimg; // insert to notebook


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-297.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-297.png)

\>reset;


Anda harus menahan grafik, karena perintah plot() akan menghapus
jendela plot.


Untuk menghapus semua yang telah kita lakukan, kita gunakan reset().


Untuk menampilkan gambar hasil plot di layar notebook, perintah
plot2d() dapat diakhiri dengan titik dua (:). Cara lain adalah
perintah plot2d() diakhiri dengan titik koma (;), kemudian gunakan
perintah insimg() untuk menampilkan gambar hasil plot.


Sebagai contoh lain, kita menggambar sebuah plot sebagai inset pada
plot yang lain. Hal ini dilakukan dengan mendefinisikan jendela plot
yang lebih kecil. Perhatikan bahwa jendela ini tidak menyediakan ruang
untuk label sumbu di luar jendela plot. Kita harus menambahkan
beberapa margin untuk hal ini sesuai kebutuhan. Perhatikan bahwa kita
menyimpan dan mengembalikan jendela penuh, dan menahan plot saat ini
ketika kita membuat inset.


\>plot2d("x^3-x");

\>xw=200; yw=100; ww=300; hw=300;

\>ow=window();

\>window(xw,yw,xw+ww,yw+hw);

\>hold on;

\>barclear(xw-50,yw-10,ww+60,ww+60);

\>plot2d("x^4-x",grid=6):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-298.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-298.png)

\>hold off;

\>window(ow);


Plot dengan beberapa angka dicapai dengan cara yang sama. Ada fungsi
utility figure() untuk ini.


## Aspek Plot

Plot default menggunakan jendela plot persegi. Anda dapat mengubahnya
dengan fungsi aspect(). Jangan lupa untuk mengatur ulang aspeknya
nanti. Anda juga dapat mengubah default ini di menu dengan "Set
Aspect" ke rasio aspek tertentu atau ke ukuran jendela grafik saat
ini.


Tetapi Anda juga dapat mengubahnya untuk satu plot. Untuk ini, ukuran
area plot saat ini diubah, dan jendela diatur sedemikian rupa sehingga
label memiliki ruang yang cukup.


\>aspect(2); // rasio panjang dan lebar 2:1

\>plot2d(["sin(x)","cos(x)"],0,2pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-299.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-299.png)

\>aspect();

\>reset;


Fungsi reset () mengembalikan default plot, termasuk rasio aspek.


Plot 2D di Euler


EMT Math Toolbox memiliki plot dalam bentuk 2D, baik untuk data maupun
fungsi. EMT menggunakan fungsi plot2d. Fungsi ini dapat memplot fungsi
dan data.


Dimungkinkan untuk memplot di Maxima menggunakan Gnuplot atau di
Python menggunakan Math Plot Lib.


Euler dapat memplot plot 2D dari


* 
ekspresi

* 
fungsi, variabel, atau kurva berparameter,

* 
vektor nilai x-y,

* 
awan titik-titik di bidang,

* 
kurva implisit dengan level atau wilayah level.

* 
Fungsi yang kompleks


Gaya plot mencakup berbagai gaya untuk garis dan titik, plot batang,
dan plot berbayang.


Plot Ekspresi atau Variabel


Ekspresi tunggal dalam "x" (misalnya "4*x^2") atau nama fungsi
(misalnya "f") menghasilkan grafik fungsi.


Berikut ini adalah contoh paling dasar, yang menggunakan rentang
default dan menetapkan rentang y yang tepat agar sesuai dengan plot
fungsi.


Catatan: Jika Anda mengakhiri baris perintah dengan tanda titik dua
":", plot akan disisipkan ke dalam jendela teks. Jika tidak, tekan TAB
untuk melihat plot jika jendela plot tertutup.


\>plot2d("x^2"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-300.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-300.png)

\>aspect(1.5); plot2d("x^3-x"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-301.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-301.png)

\>a:=5.6; plot2d("exp(-a\*x^2)/a"); insimg(30); // menampilkan gambar hasil plot setinggi 25 baris


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-302.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-302.png)

Dari beberapa contoh sebelumnya Anda dapat melihat bahwa aslinya
gambar plot menggunakan sumbu X dengan rentang nilai dari -2 sampai
dengan 2. Untuk mengubah rentang nilai X dan Y, Anda dapat menambahkan
nilai-nilai batas X (dan Y) di belakang ekspresi yang digambar.


Rentang plot ditetapkan dengan parameter yang ditetapkan berikut ini


* 
a,b: rentang x (default -2,2)

* 
c, d: rentang y (default: skala dengan nilai)

* 
r: sebagai alternatif, radius di sekitar pusat plot

* 
cx, cy: koordinat pusat plot (default 0,0)


\>plot2d("x^3-x",-1,2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-303.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-303.png)

\>plot2d("sin(x)",-2\*pi,2\*pi): // plot sin(x) pada interval [-2pi, 2pi]


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-304.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-304.png)

\>plot2d("cos(x)","sin(3\*x)",xmin=0,xmax=2pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-305.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-305.png)

Alternatif untuk tanda titik dua adalah perintah insimg(lines), yang
menyisipkan plot yang menempati sejumlah baris teks tertentu.


Dalam opsi, plot dapat diatur untuk muncul


* 
di jendela terpisah yang dapat diubah ukurannya,

* 
di jendela buku catatan.


Lebih banyak gaya yang dapat dicapai dengan perintah plot tertentu.


Dalam hal apa pun, tekan tombol tabulator untuk melihat plot, jika
disembunyikan.


Untuk membagi jendela menjadi beberapa plot, gunakan perintah
figure(). Pada contoh, kita memplot x^1 sampai x^4 ke dalam 4 bagian
jendela. figure(0) akan mereset jendela default.


\>reset;

\>figure(2,2); ...  
\>   for n=1 to 4; figure(n); plot2d("x^"+n); end; ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-306.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-306.png)

Pada plot2d(), terdapat beberapa gaya alternatif yang tersedia dengan
grid=x. Sebagai gambaran umum, kami menampilkan berbagai gaya grid
dalam satu gambar (lihat di bawah ini untuk perintah figure()). Gaya
grid=0 tidak disertakan. Gaya ini tidak menampilkan grid dan frame.


\>figure(3,3); ...  
\>   for k=1:9; figure(k); plot2d("x^3-x",-2,1,grid=k); end; ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-307.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-307.png)

Jika argumen untuk plot2d() adalah sebuah ekspresi yang diikuti oleh
empat angka, angka-angka ini adalah rentang x dan y untuk plot.


Atau, a, b, c, d dapat ditentukan sebagai parameter yang ditetapkan
sebagai a=... dst.


Pada contoh berikut, kita mengubah gaya grid, menambahkan label, dan
menggunakan label vertikal untuk sumbu y.


\>aspect(1.5); plot2d("sin(x)",0,2pi,-1.2,1.2,grid=3,xl="x",yl="sin(x)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-308.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-308.png)

\>plot2d("sin(x)+cos(2\*x)",0,4pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-309.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-309.png)

Gambar yang dihasilkan dengan menyisipkan plot ke dalam jendela teks
disimpan dalam direktori yang sama dengan notebook, secara default
dalam subdirektori bernama "images". Gambar-gambar tersebut juga
digunakan oleh ekspor HTML.


Anda cukup menandai gambar mana saja dan menyalinnya ke clipboard
dengan Ctrl-C. Tentu saja, Anda juga dapat mengekspor grafik saat ini
dengan fungsi-fungsi pada menu File.


Fungsi atau ekspresi dalam plot2d dievaluasi secara adaptif. Untuk
kecepatan yang lebih tinggi, matikan plot adaptif dengan &lt;adaptive dan
tentukan jumlah subinterval dengan n=... Hal ini hanya diperlukan pada
kasus-kasus yang jarang terjadi.


\>plot2d("sign(x)\*exp(-x^2)",-1,1,<adaptive,n=10000):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-310.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-310.png)

\>plot2d("x^x",r=1.2,cx=1,cy=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-311.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-311.png)

Perhatikan bahwa x^x tidak didefinisikan untuk x&lt;=0. Fungsi plot2d
menangkap kesalahan ini, dan mulai memplot segera setelah fungsi
didefinisikan. Hal ini berlaku untuk semua fungsi yang mengembalikan
NAN di luar jangkauan definisinya.


\>plot2d("log(x)",-0.1,2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-312.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-312.png)

Parameter square=true (or &gt;square) memilih rentang y secara otomatis
sehingga hasilnya adalah jendela plot persegi. Perhatikan bahwa secara
default, Euler menggunakan ruang persegi di dalam jendela plot.


\>plot2d("x^3-x",\>square):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-313.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-313.png)

\>plot2d(''integrate("sin(x)\*exp(-x^2)",0,x)'',0,2): // plot integral


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-314.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-314.png)

Jika Anda membutuhkan lebih banyak ruang untuk label-y, panggil
shrinkwindow() dengan parameter lebih kecil, atau tetapkan nilai
positif untuk "smaller" pada plot2d().


\>plot2d("gamma(x)",1,10,yl="y-values",smaller=6,<vertical):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-315.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-315.png)

Ekspresi simbolik juga dapat digunakan, karena disimpan sebagai
ekspresi string sederhana.


\>x=linspace(0,2pi,1000); plot2d(sin(5x),cos(7x)):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-316.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-316.png)

\>a:=5.6; expr &= exp(-a\*x^2)/a; // define expression

\>plot2d(expr,-2,2): // plot from -2 to 2


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-317.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-317.png)

\>plot2d(expr,r=1,thickness=2): // plot in a square around (0,0)


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-318.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-318.png)

\>plot2d(&diff(expr,x),\>add,style="--",color=red): // add another plot


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-319.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-319.png)

\>plot2d(&diff(expr,x,2),a=-2,b=2,c=-2,d=1): // plot in rectangle


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-320.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-320.png)

\>plot2d(&diff(expr,x),a=-2,b=2,\>square): // keep plot square


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-321.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-321.png)

\>plot2d("x^2",0,1,steps=1,color=red,n=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-322.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-322.png)

\>plot2d("x^2",\>add,steps=2,color=blue,n=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-323.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-323.png)

# Fungsi dalam satu Parameter

Fungsi plot yang paling penting untuk plot planar adalah plot2d().
Fungsi ini diimplementasikan dalam bahasa Euler dalam file "plot.e",
yang dimuat pada awal program.


Berikut adalah beberapa contoh penggunaan fungsi. Seperti biasa dalam
EMT, fungsi yang bekerja untuk fungsi atau ekspresi lain, Anda dapat
mengoper parameter tambahan (selain x) yang bukan variabel global ke
fungsi dengan parameter titik koma atau dengan koleksi panggilan.


\>function f(x,a) := x^2/a+a\*x^2-x; // define a function

\>a=0.3; plot2d("f",0,1;a): // plot with a=0.3


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-324.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-324.png)

\>plot2d("f",0,1;0.4): // plot with a=0.4


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-325.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-325.png)

\>plot2d({{"f",0.2}},0,1): // plot with a=0.2


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-326.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-326.png)

\>plot2d({{"f(x,b)",b=0.1}},0,1): // plot with 0.1


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-327.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-327.png)

\>function f(x) := x^3-x; ...  
\>   plot2d("f",r=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-328.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-328.png)

Berikut ini adalah ringkasan dari fungsi yang diterima


* 
ekspresi atau ekspresi simbolik dalam x

* 
fungsi atau fungsi simbolik dengan nama sebagai "f"

* 
fungsi-fungsi simbolik hanya dengan nama f


Fungsi plot2d() juga menerima fungsi simbolik. Untuk fungsi simbolik,
nama saja sudah cukup.


\>function f(x) &= diff(x^x,x)


    
                                x
                               x  (log(x) + 1)
    

\>plot2d(f,0,2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-329.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-329.png)

Tentu saja, untuk ekspresi atau ungkapan simbolik, nama variabel sudah
cukup untuk memplotnya.


\>expr &= sin(x)\*exp(-x)


    
                                  - x
                                 E    sin(x)
    

\>plot2d(expr,0,3pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-330.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-330.png)

\>function f(x) &= x^x;

\>plot2d(f,r=1,cx=1,cy=1,color=blue,thickness=2);

\>plot2d(&diff(f(x),x),\>add,color=red,style="-.-"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-331.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-331.png)

Untuk gaya garis, ada berbagai pilihan.


* 
style = "...". Pilih dari "-", "--", "-.", ".", ".-.", "-.-".

* 
color: Lihat di bawah untuk warna.

* 
thickness (Ketebalan): Default adalah 1.


Warna dapat dipilih sebagai salah satu warna default, atau sebagai
warna RGB.


* 
0..15: indeks warna default.

* 
color constant: white, black, red, green, blue, cyan, olive,
* lightgray, gray, darkgray, orange, lightgreen, turquoise, lightblue,
* lightorange, yellow

* 
rgb ( red, green, blue ): parameter adalah real dalam [0,1].


\>plot2d("exp(-x^2)",r=2,color=red,thickness=3,style="--"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-332.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-332.png)

Berikut ini adalah pemandangan warna EMT yang sudah ditetapkan
sebelumnya.


\>aspect(2); columnsplot(ones(1,16),lab=0:15,grid=0,color=0:15):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-333.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-333.png)

Tetapi Anda bisa menggunakan warna apa pun.


\>columnsplot(ones(1,16),grid=0,color=rgb(0,0,linspace(0,1,15))):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-334.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-334.png)

# Menggambar beberapa kurva pada bidang koordinat yang sama

Memplot lebih dari satu fungsi (multiple function) ke dalam satu
jendela dapat dilakukan dengan berbagai cara. Salah satu caranya
adalah dengan menggunakan &gt;add untuk beberapa pemanggilan ke plot2d
secara bersamaan, kecuali pemanggilan pertama. Kita telah menggunakan
fitur ini pada contoh di atas.


\>aspect(); plot2d("cos(x)",r=2,grid=6); plot2d("x",style=".",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-335.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-335.png)

\>aspect(1.5); plot2d("sin(x)",0,2pi); plot2d("cos(x)",color=blue,style="--",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-336.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-336.png)

Salah satu kegunaan &gt;add adalah untuk menambahkan titik pada kurva.


\>plot2d("sin(x)",0,pi); plot2d(2,sin(2),\>points,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-337.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-337.png)

Kami menambahkan titik perpotongan dengan label (pada posisi "cl"
untuk kiri tengah), dan menyisipkan hasilnya ke dalam buku catatan.
Kami juga menambahkan judul ke plot.


\>plot2d(["cos(x)","x"],r=1.1,cx=0.5,cy=0.5, ...  
\>     color=[black,blue],style=["-","."], ...  
\>     grid=1);

\>x0=solve("cos(x)-x",1);  ...  
\>     plot2d(x0,x0,\>points,\>add,title="Intersection Demo");  ...  
\>     label("cos(x) = x",x0,x0,pos="cl",offset=20):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-338.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-338.png)

Dalam demo berikut ini, kami memplot fungsi sinc(x)=sin(x)/x dan
ekspansi Taylor ke-8 dan ke-16. Kami menghitung ekspansi ini
menggunakan Maxima melalui ekspresi simbolik.


Plot ini dilakukan dalam perintah multi-baris berikut dengan tiga
pemanggilan plot2d(). Perintah kedua dan ketiga memiliki set flag
&gt;add, yang membuat plot menggunakan rentang sebelumnya.


Kami menambahkan sebuah kotak label yang menjelaskan fungsi-fungsi
tersebut.


\>$taylor(sin(x)/x,x,0,4)


$$\frac{x^4}{120}-\frac{x^2}{6}+1$$\>plot2d("sinc(x)",0,4pi,color=green,thickness=2); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,8),\>add,color=blue,style="--"); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,16),\>add,color=red,style="-.-"); ...  
\>     labelbox(["sinc","T8","T16"],styles=["-","--","-.-"], ...  
\>       colors=[black,blue,red]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-340.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-340.png)

Pada contoh berikut, kami menghasilkan Polinomial Bernstein.


$$B_i(x) = \binom{n}{i} x^i (1-x)^{n-i}$$\>plot2d("(1-x)^10",0,1); // plot first function

\>for i=1 to 10; plot2d("bin(10,i)\*x^i\*(1-x)^(10-i)",\>add); end;

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-342.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-342.png)

Metode kedua menggunakan sepasang matriks nilai x dan matriks nilai y
dengan ukuran yang sama.


Kita membuat sebuah matriks nilai dengan satu Polinomial Bernstein di
setiap baris. Untuk ini, kita cukup menggunakan vektor kolom i.
Lihatlah pengantar tentang bahasa matriks untuk mempelajari lebih
lanjut.


\>x=linspace(0,1,500)  ...  
\>   //(a,b,c)=dari a sampe b, ditambah (b-a)/c, di sini 0 ditambah 0,002 sampe 1


    [0,  0.002,  0.004,  0.006,  0.008,  0.01,  0.012,  0.014,  0.016,
    0.018,  0.02,  0.022,  0.024,  0.026,  0.028,  0.03,  0.032,  0.034,
    0.036,  0.038,  0.04,  0.042,  0.044,  0.046,  0.048,  0.05,  0.052,
    0.054,  0.056,  0.058,  0.06,  0.062,  0.064,  0.066,  0.068,  0.07,
    0.072,  0.074,  0.076,  0.078,  0.08,  0.082,  0.084,  0.086,  0.088,
    0.09,  0.092,  0.094,  0.096,  0.098,  0.1,  0.102,  0.104,  0.106,
    0.108,  0.11,  0.112,  0.114,  0.116,  0.118,  0.12,  0.122,  0.124,
    0.126,  0.128,  0.13,  0.132,  0.134,  0.136,  0.138,  0.14,  0.142,
    0.144,  0.146,  0.148,  0.15,  0.152,  0.154,  0.156,  0.158,  0.16,
    0.162,  0.164,  0.166,  0.168,  0.17,  0.172,  0.174,  0.176,  0.178,
    0.18,  0.182,  0.184,  0.186,  0.188,  0.19,  0.192,  0.194,  0.196,
    0.198,  0.2,  0.202,  0.204,  0.206,  0.208,  0.21,  0.212,  0.214,
    0.216,  0.218,  0.22,  0.222,  0.224,  0.226,  0.228,  0.23,  0.232,
    0.234,  0.236,  0.238,  0.24,  0.242,  0.244,  0.246,  0.248,  0.25,
    0.252,  0.254,  0.256,  0.258,  0.26,  0.262,  0.264,  0.266,  0.268,
    0.27,  0.272,  0.274,  0.276,  0.278,  0.28,  0.282,  0.284,  0.286,
    0.288,  0.29,  0.292,  0.294,  0.296,  0.298,  0.3,  0.302,  0.304,
    0.306,  0.308,  0.31,  0.312,  0.314,  0.316,  0.318,  0.32,  0.322,
    0.324,  0.326,  0.328,  0.33,  0.332,  0.334,  0.336,  0.338,  0.34,
    0.342,  0.344,  0.346,  0.348,  0.35,  0.352,  0.354,  0.356,  0.358,
     ... ]

\>n=10; k=(0:n)' // n is row vector, k is column vector


                0 
                1 
                2 
                3 
                4 
                5 
                6 
                7 
                8 
                9 
               10 

\>y=bin(n,k)\*x^k\*(1-x)^(n-k); // y is a matrix then

\>plot2d(x,y):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-343.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-343.png)

Perhatikan bahwa parameter warna dapat berupa vektor. Kemudian setiap
warna digunakan untuk setiap baris matriks.


\>x=linspace(0,1,200); y=x^(1:10)'; plot2d(x,y,color=1:10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-344.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-344.png)

Metode lainnya adalah menggunakan vektor ekspresi (string). Anda
kemudian dapat menggunakan larik warna, larik gaya, dan larik
ketebalan dengan panjang yang sama.


\>plot2d(["sin(x)","cos(x)"],0,2pi,color=4:5): 


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-345.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-345.png)

\>plot2d(["sin(x)","cos(x)"],0,2pi): // plot vector of expressions


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-346.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-346.png)

Kita bisa mendapatkan vektor seperti itu dari Maxima dengan
menggunakan makelist() dan mxm2str().


\>v &= makelist(binomial(10,i)\*x^i\*(1-x)^(10-i),i,0,10) // make list


    
                    10            9              8  2             7  3
            [(1 - x)  , 10 (1 - x)  x, 45 (1 - x)  x , 120 (1 - x)  x , 
               6  4             5  5             4  6             3  7
    210 (1 - x)  x , 252 (1 - x)  x , 210 (1 - x)  x , 120 (1 - x)  x , 
              2  8              9   10
    45 (1 - x)  x , 10 (1 - x) x , x  ]
    

\>mxm2str(v) // get a vector of strings from the symbolic vector


    (1-x)^10
    10*(1-x)^9*x
    45*(1-x)^8*x^2
    120*(1-x)^7*x^3
    210*(1-x)^6*x^4
    252*(1-x)^5*x^5
    210*(1-x)^4*x^6
    120*(1-x)^3*x^7
    45*(1-x)^2*x^8
    10*(1-x)*x^9
    x^10

\>plot2d(mxm2str(v),0,1): // plot functions


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-347.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-347.png)

Alternatif lain adalah dengan menggunakan bahasa matriks Euler.


Jika sebuah ekspresi menghasilkan sebuah matriks fungsi, dengan satu
fungsi di setiap baris, semua fungsi ini akan diplot ke dalam satu
plot.


Untuk ini, gunakan vektor parameter dalam bentuk vektor kolom. Jika
sebuah larik warna ditambahkan, maka akan digunakan untuk setiap baris
plot.


\>n=(1:10)'; plot2d("x^n",0,1,color=1:10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-348.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-348.png)

Ekspresi dan fungsi satu baris dapat melihat variabel global.


Jika Anda tidak dapat menggunakan variabel global, Anda perlu
menggunakan fungsi dengan parameter tambahan, dan memberikan parameter
ini sebagai parameter titik koma.


Berhati-hatilah untuk meletakkan semua parameter yang diberikan di
akhir perintah plot2d. Pada contoh ini kita mengoper a=5 ke fungsi f,
yang kita plot dari -10 ke 10.


\>function f(x,a) := 1/a\*exp(-x^2/a); ...  
\>   plot2d("f",-10,10;5,thickness=2,title="a=5"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-349.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-349.png)

Atau, gunakan koleksi dengan nama fungsi dan semua parameter tambahan.
Daftar khusus ini disebut koleksi panggilan, dan itu adalah cara yang
lebih disukai untuk mengoper argumen ke fungsi yang dengan sendirinya
dioper sebagai argumen ke fungsi lain.


Pada contoh berikut, kita menggunakan perulangan untuk memplot
beberapa fungsi (lihat tutorial tentang pemrograman perulangan).


\>plot2d({{"f",1}},-10,10); ...  
\>   for a=2:10; plot2d({{"f",a}},\>add); end:


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-350.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-350.png)

Kita dapat mencapai hasil yang sama dengan cara berikut menggunakan
bahasa matriks EMT. Setiap baris dari matriks f(x,a) adalah satu
fungsi. Selain itu, kita dapat mengatur warna untuk setiap baris
matriks. Klik dua kali pada fungsi getspectral() untuk penjelasannya.


\>x=-10:0.01:10; a=(1:10)'; plot2d(x,f(x,a),color=getspectral(a/10)):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-351.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-351.png)

## Label Teks

Dekorasi sederhana dapat berupa


* 
sebuah judul dengan title="..."

* 
label x dan y dengan xl="...", yl="..."

* 
label teks lain dengan label("...",x,y)


Perintah label akan memplotkan ke dalam plot saat ini pada koordinat
plot (x,y). Perintah ini dapat menerima sebuah argumen posisi.


\>plot2d("x^3-x",-1,2,title="y=x^3-x",yl="y",xl="x"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-352.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-352.png)

\>expr := "log(x)/x"; ...  
\>     plot2d(expr,0.5,5,title="y="+expr,xl="x",yl="y"); ...  
\>     label("(1,0)",1,0); label("Max",E,expr(E),pos="lc"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-353.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-353.png)

Ada juga fungsi labelbox(), yang dapat menampilkan fungsi dan teks.
Fungsi ini membutuhkan vektor string dan warna, satu item untuk setiap
fungsi.


\>function f(x) &= x^2\*exp(-x^2);  ...  
\>   plot2d(&f(x),a=-3,b=3,c=-1,d=1);  ...  
\>   plot2d(&diff(f(x),x),\>add,color=blue,style="--"); ...  
\>   labelbox(["function","derivative"],styles=["-","--"], ...  
\>      colors=[black,blue],w=0.4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-354.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-354.png)

Kotak tersebut ditempatkan di kanan atas secara default, tetapi &gt;left
menempatkannya di kiri atas. Anda dapat memindahkannya ke tempat mana
pun yang Anda suka. Posisi jangkar adalah sudut kanan atas kotak, dan
angkanya adalah pecahan dari ukuran jendela grafik. Lebarnya otomatis.


Untuk plot titik, kotak label juga dapat digunakan. Tambahkan
parameter &gt;points, atau vektor bendera, satu untuk setiap label.


Pada contoh berikut, hanya ada satu fungsi. Jadi kita dapat
menggunakan string sebagai pengganti vektor string. Kita mengatur
warna teks menjadi hitam untuk contoh ini.


\>n=10; plot2d(0:n,bin(n,0:n),\>addpoints); ...  
\>   labelbox("Binomials",styles="[]",\>points,x=0.1,y=0.1, ...  
\>   tcolor=black,\>left):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-355.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-355.png)

Gaya plot ini juga tersedia di statplot(). Seperti pada plot2d() warna
dapat diatur untuk setiap baris plot. Terdapat lebih banyak plot
khusus untuk keperluan statistik (lihat tutorial tentang statistik).


\>statplot(1:10,random(2,10),color=[red,blue]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-356.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-356.png)

Fitur yang serupa adalah fungsi textbox().


Lebarnya secara default adalah lebar maksimal baris teks. Tetapi bisa
juga diatur oleh pengguna.


\>function f(x) &= exp(-x)\*sin(2\*pi\*x); ...  
\>   plot2d("f(x)",0,2pi); ...  
\>   textbox(latex("\\text{Example of a damped oscillation}\\ f(x)=e^{-x}sin(2\\pi x)"),w=1.125):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-357.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-357.png)

Label teks, judul, kotak label, dan teks lainnya dapat berisi string
Unicode (lihat sintaks EMT untuk mengetahui lebih lanjut tentang
string Unicode).


\>plot2d("x^3-x",title=u"x &rarr; x&sup3; - x"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-358.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-358.png)

Label pada sumbu x dan y bisa vertikal, begitu juga dengan sumbu.


\>plot2d("sinc(x)",0,2pi,xl="x",yl=u"x &rarr; sinc(x)",\>vertical):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-359.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-359.png)

## LaTeX

Anda juga dapat memplot formula LaTeX jika Anda telah menginstal
sistem LaTeX. Saya merekomendasikan MiKTeX. Jalur ke binari " latex "
dan " dvipng " harus berada di jalur sistem, atau Anda harus mengatur
LaTeX pada menu opsi.


Perhatikan, bahwa penguraian LaTeX berjalan lambat. Jika Anda ingin
menggunakan LaTeX dalam plot animasi, Anda harus memanggil latex()
sebelum perulangan satu kali dan menggunakan hasilnya (gambar dalam
matriks RGB).


Pada plot berikut ini, kita menggunakan LaTeX untuk label x dan y,
sebuah label, kotak label dan judul plot.


\>plot2d("exp(-x)\*sin(x)/x",a=0,b=2pi,c=0,d=1,grid=6,color=blue, ...  
\>     title=latex("\\text{Function $\\Phi$}"), ...  
\>     xl=latex("\\phi"),yl=latex("\\Phi(\\phi)")); ...  
\>   textbox( ...  
\>     latex("\\Phi(\\phi) = e^{-\\phi} \\frac{\\sin(\\phi)}{\\phi}"),x=0.8,y=0.5); ...  
\>   label(latex("\\Phi",color=blue),1,0.4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-360.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-360.png)

Seringkali, kita menginginkan spasi dan label teks yang tidak sesuai
pada sumbu x. Kita dapat menggunakan xaxis() dan yaxis() seperti yang
akan kita tunjukkan nanti.


Cara termudah adalah dengan membuat plot kosong dengan sebuah frame
menggunakan grid=4, dan kemudian menambahkan grid dengan ygrid() dan
xgrid(). Pada contoh berikut, kita menggunakan tiga buah string LaTeX
untuk label pada sumbu x dengan xtick().


\>plot2d("sinc(x)",0,2pi,grid=4,<ticks); ...  
\>   ygrid(-2:0.5:2,grid=6); ...  
\>   xgrid([0:2]\*pi,<ticks,grid=6);  ...  
\>   xtick([0,pi,2pi],["0","\\pi","2\\pi"],\>latex):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-361.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-361.png)

Tentu saja, fungsi juga dapat digunakan.


\>function map f(x) ...


    if x>0 then return x^4
    else return x^2
    endi
    endfunction
</pre>
Parameter "map" membantu menggunakan fungsi untuk vektor. Untuk


plot, hal ini tidak diperlukan. Tetapi untuk mendemonstrasikan bahwa
vektorisasi


berguna, kami menambahkan beberapa titik kunci pada plot pada x=-1,
x=0 dan x=1.


Pada plot berikut, kita juga memasukkan beberapa kode LaTeX. Kita
menggunakannya untuk


dua label dan sebuah kotak teks. Tentu saja, Anda hanya dapat
menggunakan


LaTeX jika Anda telah menginstal LaTeX dengan benar.


\>plot2d("f",-1,1,xl="x",yl="f(x)",grid=6);  ...  
\>   plot2d([-1,0,1],f([-1,0,1]),\>points,\>add); ...  
\>   label(latex("x^3"),0.72,f(0.72)); ...  
\>   label(latex("x^2"),-0.52,f(-0.52),pos="ll"); ...  
\>   textbox( ...  
\>     latex("f(x)=\\begin{cases} x^3 & x\>0 \\\\ x^2 & x \\le 0\\end{cases}"), ...  
\>     x=0.7,y=0.2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-362.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-362.png)

## Interaksi Pengguna

Ketika memplot fungsi atau ekspresi, parameter &gt;user memungkinkan
pengguna untuk memperbesar dan menggeser plot dengan tombol kursor
atau mouse. Pengguna dapat


* 
memperbesar dengan + atau -

* 
memindahkan plot dengan tombol kursor

* 
memilih jendela plot dengan mouse

* 
mereset tampilan dengan spasi

* 
keluar dengan return


Tombol spasi akan mengatur ulang plot ke jendela plot semula.


Ketika memplot data, bendera &gt;user hanya akan menunggu penekanan
tombol.


\>plot2d({{"x^3-a\*x",a=1}},\>user,title="Press any key!"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-363.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-363.png)

\>plot2d("exp(x)\*sin(x)",user=true, ...  
\>     title="+/- or cursor keys (return to exit)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-364.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-364.png)

Berikut ini menunjukkan cara interaksi pengguna tingkat lanjut (lihat
tutorial tentang pemrograman untuk detailnya).


Fungsi bawaan mousedrag() menunggu peristiwa mouse atau keyboard.
Fungsi ini melaporkan mouse ke bawah, mouse bergerak atau mouse ke
atas, dan penekanan tombol. Fungsi dragpoints() memanfaatkan hal ini,
dan mengizinkan pengguna untuk menyeret titik manapun di dalam plot.


Kita membutuhkan fungsi plot terlebih dahulu. Sebagai contoh, kita
melakukan interpolasi pada 5 titik dengan sebuah polinomial. Fungsi
ini harus memplot ke dalam area plot yang tetap.


\>function plotf(xp,yp,select) ...


      d=interp(xp,yp);
      plot2d("interpval(xp,d,x)";d,xp,r=2);
      plot2d(xp,yp,>points,>add);
      if select>0 then
        plot2d(xp[select],yp[select],color=red,>points,>add);
      endif;
      title("Drag one point, or press space or return!");
    endfunction
</pre>
Perhatikan parameter titik koma pada plot2d (d dan xp), yang
diteruskan ke evaluasi fungsi interp(). Tanpa ini, kita harus menulis
fungsi plotinterp() terlebih dahulu, untuk mengakses nilai secara
global.


Sekarang kita menghasilkan beberapa nilai acak, dan membiarkan
pengguna menyeret titik-titiknya.


\>t=-1:0.5:1; dragpoints("plotf",t,random(size(t))-0.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-365.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-365.png)

Ada juga fungsi yang memplot fungsi lain tergantung pada vektor
parameter, dan memungkinkan pengguna menyesuaikan parameter ini.


Pertama, kita memerlukan fungsi plot.


\>function plotf([a,b]) := plot2d("exp(a\*x)\*cos(2pi\*b\*x)",0,2pi;a,b);


Kemudian kita membutuhkan nama untuk parameter, nilai awal dan matriks
rentang nx2, dan secara opsional, sebuah garis judul.


Terdapat slider interaktif, yang dapat mengatur nilai oleh pengguna.
Fungsi dragvalues() menyediakan ini.


\>dragvalues("plotf",["a","b"],[-1,2],[[-2,2];[1,10]], ...  
\>     heading="Drag these values:",hcolor=black):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-366.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-366.png)

Anda dapat membatasi nilai yang diseret menjadi bilangan bulat.
Sebagai contoh, kita menulis fungsi plot, yang memplot polinomial
Taylor dengan derajat n ke fungsi kosinus.


\>function plotf(n) ...


    plot2d("cos(x)",0,2pi,>square,grid=6);
    plot2d(&"taylor(cos(x),x,0,@n)",color=blue,>add);
    textbox("Taylor polynomial of degree "+n,0.1,0.02,style="t",>left);
    endfunction
</pre>
Sekarang kita membiarkan derajat n bervariasi dari 0 sampai 20 dalam
20 stop. Hasil dari dragvalues() digunakan untuk memplot sketsa dengan
n ini, dan untuk menyisipkan plot ke dalam buku catatan.


\>nd=dragvalues("plotf","degree",2,[0,20],20,y=0.8, ...  
\>      heading="Drag the value:"); ...  
\>   plotf(nd):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-367.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-367.png)

Berikut ini adalah peragaan sederhana dari fungsi ini. Pengguna dapat
menggambar di atas jendela plot, meninggalkan jejak titik.


\>function dragtest ...


      plot2d(none,r=1,title="Drag with the mouse, or press any key!");
      start=0;
      repeat
        {flag,m,time}=mousedrag();
        if flag==0 then return; endif;
        if flag==2 then
          hold on; mark(m[1],m[2]); hold off;
        endif;
      end
    endfunction
</pre>
\>dragtest // lihat hasilnya dan cobalah lakukan!


## Gaya Plot 2D

Secara default, EMT menghitung tanda sumbu otomatis dan menambahkan
label pada setiap tanda. Hal ini dapat diubah dengan parameter grid.
Gaya default sumbu dan label dapat dimodifikasi. Selain itu, label dan
judul dapat ditambahkan secara manual. Untuk mengatur ulang ke gaya
default, gunakan reset().


\>aspect();

\>figure(3,4); ...  
\>    figure(1); plot2d("x^3-x",grid=0); ... // no grid, frame or axis

\> figure(2); plot2d("x^3-x",grid=1); ... // x-y-axis

\> figure(3); plot2d("x^3-x",grid=2); ... // default ticks

\> figure(4); plot2d("x^3-x",grid=3); ... // x-y- axis with labels inside

\> figure(5); plot2d("x^3-x",grid=4); ... // no ticks, only labels

\> figure(6); plot2d("x^3-x",grid=5); ... // default, but no margin

\> figure(7); plot2d("x^3-x",grid=6); ... // axes only

\> figure(8); plot2d("x^3-x",grid=7); ... // axes only, ticks at axis

\> figure(9); plot2d("x^3-x",grid=8); ... // axes only, finer ticks at axis

\> figure(10); plot2d("x^3-x",grid=9); ... // default, small ticks inside

\> figure(11); plot2d("x^3-x",grid=10); ...// no ticks, axes only

\> figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-368.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-368.png)

Parameter &lt;frame mematikan bingkai, dan framecolor=blue menetapkan
bingkai ke warna biru.


Jika Anda menginginkan tanda centang Anda sendiri, Anda dapat
menggunakan style=0, dan menambahkan semuanya nanti.


\>aspect(1.5); 

\>plot2d("x^3-x",grid=0); // plot

\>frame; xgrid([-1,0,1]); ygrid(0): // add frame and grid


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-369.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-369.png)

Untuk judul plot dan label sumbu, lihat contoh berikut.


\>plot2d("exp(x)",-1,1);

\>textcolor(black); // set the text color to black

\>title(latex("y=e^x")); // title above the plot

\>xlabel(latex("x")); // "x" for x-axis

\>ylabel(latex("y"),\>vertical); // vertical "y" for y-axis

\>label(latex("(0,1)"),0,1,color=blue): // label a point


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-370.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-370.png)

Sumbu dapat digambar secara terpisah dengan sumbu x() dan sumbu y().


\>plot2d("x^3-x",<grid,<frame);

\>xaxis(0,xx=-2:1,style="-\>"); yaxis(0,yy=-5:5,style="-\>"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-371.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-371.png)

Teks pada plot dapat diatur dengan label(). Pada contoh berikut ini,
"lc" berarti lower center. Ini mengatur posisi label relatif terhadap
koordinat plot.


\>function f(x) &= x^3-x


    
                                     3
                                    x  - x
    

\>plot2d(f,-1,1,\>square);

\>x0=fmin(f,0,1); // compute point of minimum

\>label("Rel. Min.",x0,f(x0),pos="lc"): // add a label there


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-372.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-372.png)

Terdapat juga kotak teks.


\>plot2d(&f(x),-1,1,-2,2); // function

\>plot2d(&diff(f(x),x),\>add,style="--",color=red); // derivative

\>labelbox(["f","f'"],["-","--"],[black,red]): // label box


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-373.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-373.png)

\>plot2d(["exp(x)","1+x"],color=[black,blue],style=["-","-.-"]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-374.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-374.png)

\>gridstyle("-\>",color=gray,textcolor=gray,framecolor=gray);  ...  
\>    plot2d("x^3-x",grid=1);   ...  
\>    settitle("y=x^3-x",color=black); ...  
\>    label("x",2,0,pos="bc",color=gray);  ...  
\>    label("y",0,6,pos="cl",color=gray); ...  
\>    reset():


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-375.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-375.png)

Untuk kontrol yang lebih besar lagi, sumbu x dan sumbu y dapat
dilakukan secara manual.


Perintah fullwindow() akan memperluas jendela plot karena kita tidak
lagi membutuhkan tempat untuk label di luar jendela plot. Gunakan
shrinkwindow() atau reset() untuk mengatur ulang ke default.


\>fullwindow; ...  
\>    gridstyle(color=darkgray,textcolor=darkgray); ...  
\>    plot2d(["2^x","1","2^(-x)"],a=-2,b=2,c=0,d=4,<grid,color=4:6,<frame); ...  
\>    xaxis(0,-2:1,style="-\>"); xaxis(0,2,"x",<axis); ...  
\>    yaxis(0,4,"y",style="-\>"); ...  
\>    yaxis(-2,1:4,\>left); ...  
\>    yaxis(2,2^(-2:2),style=".",<left); ...  
\>    labelbox(["2^x","1","2^-x"],colors=4:6,x=0.8,y=0.2); ...  
\>    reset:


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-376.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-376.png)

Berikut ini adalah contoh lain, di mana string Unicode digunakan dan
sumbu di luar area plot.


\>aspect(1.5); 

\>plot2d(["sin(x)","cos(x)"],0,2pi,color=[red,green],<grid,<frame); ...  
\>    xaxis(-1.1,(0:2)\*pi,xt=["0",u"&pi;",u"2&pi;"],style="-",\>ticks,\>zero);  ...  
\>    xgrid((0:0.5:2)\*pi,<ticks); ...  
\>    yaxis(-0.1\*pi,-1:0.2:1,style="-",\>zero,\>grid); ...  
\>    labelbox(["sin","cos"],colors=[red,green],x=0.5,y=0.2,\>left); ...  
\>    xlabel(u"&phi;"); ylabel(u"f(&phi;)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-377.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-377.png)

# Memplot Data 2D

Jika x dan y adalah vektor data, data ini akan digunakan sebagai
koordinat x dan y dari sebuah kurva. Dalam hal ini, a, b, c, dan d,
atau radius r dapat ditentukan, atau jendela plot akan menyesuaikan
secara otomatis dengan data. Sebagai alternatif, &gt;square dapat diatur
untuk mempertahankan rasio aspek persegi.


Memplot ekspresi hanyalah singkatan untuk plot data. Untuk plot data,
Anda memerlukan satu atau beberapa baris nilai x, dan satu atau
beberapa baris nilai y. Dari rentang dan nilai x, fungsi plot2d akan
menghitung data untuk diplot, secara default dengan evaluasi adaptif
dari fungsi tersebut. Untuk plot titik, gunakan "&gt;points", untuk garis
dan titik campuran gunakan "&gt;addpoints".


Namun Anda dapat memasukkan data secara langsung.


* 
Gunakan vektor baris untuk x dan y untuk satu fungsi.

* 
Matriks untuk x dan y diplot baris demi baris.


Berikut adalah contoh dengan satu baris untuk x dan y.


\>x=-10:0.1:10; y=exp(-x^2)\*x; plot2d(x,y):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-378.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-378.png)

Data juga dapat diplot sebagai titik. Gunakan points = true untuk ini.
Plot ini bekerja seperti poligon, namun hanya menggambar
sudut-sudutnya saja.


* 
style = "...": Pilih dari "[]", "&lt;&gt;", "o", ".", "..", "+", "*", "[]
* #", "&lt;&gt;#", "o#", "..#", "#", "|".


Untuk memplot kumpulan titik, gunakan &gt;points. Jika warna adalah
sebuah vektor warna, setiap titik


mendapatkan warna yang berbeda. Untuk sebuah matriks koordinat dan
vektor kolom, warna berlaku pada baris-baris matriks.


Parameter &gt;addpoints menambahkan titik-titik pada segmen garis untuk
plot data.


\>xdata=[1,1.5,2.5,3,4]; ydata=[3,3.1,2.8,2.9,2.7]; // data

\>plot2d(xdata,ydata,a=0.5,b=4.5,c=2.5,d=3.5,style="."); // lines

\>plot2d(xdata,ydata,\>points,\>add,style="o"): // add points


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-379.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-379.png)

\>p=polyfit(xdata,ydata,1); // get regression line

\>plot2d("polyval(p,x)",\>add,color=red): // add plot of line


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-380.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-380.png)

# Menggambar Daerah Yang Dibatasi Kurva

Plot data sebenarnya adalah poligon. Kita juga dapat memplot kurva
atau kurva yang terisi.


* 
filled=true mengisi plot.

* 
style = "...": Pilih dari "#", "/", "\", "\/".

* 
fillcolor: Lihat di atas untuk warna yang tersedia.


Warna isian ditentukan oleh argumen "fillcolor", dan pada pilihan
&lt;outline mencegah menggambar batas untuk semua gaya kecuali gaya
default.


\>t=linspace(0,2pi,1000); // parameter for curve

\>x=sin(t)\*exp(t/pi); y=cos(t)\*exp(t/pi); // x(t) and y(t)

\>figure(1,2); aspect(16/9)

\>figure(1); plot2d(x,y,r=10); // plot curve

\>figure(2); plot2d(x,y,r=10,\>filled,style="/",fillcolor=red); // fill curve

\>figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-381.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-381.png)

Pada contoh berikut ini, kami memplot elips terisi dan dua segi enam
terisi menggunakan kurva tertutup dengan 6 titik dengan gaya isian
yang berbeda.


\>x=linspace(0,2pi,1000); plot2d(sin(x),cos(x)\*0.5,r=1,\>filled,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-382.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-382.png)

\>t=linspace(0,2pi,6); ...  
\>   plot2d(cos(t),sin(t),\>filled,style="/",fillcolor=red,r=1.2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-383.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-383.png)

\>t=linspace(0,2pi,6); plot2d(cos(t),sin(t),\>filled,style="#"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-384.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-384.png)

Contoh lainnya adalah septagon, yang kita buat dengan 7 titik pada
lingkaran satuan.


\>t=linspace(0,2pi,7);  ...  
\>    plot2d(cos(t),sin(t),r=1,\>filled,style="/",fillcolor=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-385.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-385.png)

Berikut ini adalah himpunan nilai maksimal dari empat kondisi linier
yang kurang dari atau sama dengan 3. Ini adalah A[k].v&lt;=3 untuk semua
barisan A. Untuk mendapatkan sudut-sudut yang bagus, kita menggunakan
n yang relatif besar.


\>A=[2,1;1,2;-1,0;0,-1];

\>function f(x,y) := max([x,y].A');

\>plot2d("f",r=4,level=[0;3],color=green,n=111):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-386.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-386.png)

Poin utama dari bahasa matriks adalah bahwa bahasa ini memungkinkan
untuk menghasilkan tabel fungsi dengan mudah.


\>t=linspace(0,2pi,1000); x=cos(3\*t); y=sin(4\*t);


Kita sekarang memiliki vektor nilai x dan y. plot2d() dapat memplot
nilai-nilai ini sebagai sebuah kurva yang menghubungkan titik-titik.
Plot dapat diisi. Dalam kasus ini ini memberikan hasil yang bagus
karena aturan penggulungan, yang digunakan untuk pengisian.


\>plot2d(x,y,<grid,<frame,\>filled):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-387.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-387.png)

Vektor interval diplot terhadap nilai x sebagai wilayah yang terisi
antara nilai bawah dan atas interval.


Hal ini dapat berguna untuk memplot kesalahan perhitungan. Tapi itu
bisa juga dapat digunakan untuk memplot kesalahan statistik.


\>t=0:0.1:1; ...  
\>    plot2d(t,interval(t-random(size(t)),t+random(size(t))),style="|");  ...  
\>    plot2d(t,t,add=true):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-388.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-388.png)

Jika x adalah vektor yang diurutkan, dan y adalah vektor interval,
maka plot2d akan memplot rentang interval yang terisi pada bidang,
gaya isian sama dengan gaya poligon.


\>t=-1:0.01:1; x=~t-0.01,t+0.01~; y=x^3-x;

\>plot2d(t,y):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-389.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-389.png)

Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Untuk
ini, level harus berupa matriks 2xn. Baris pertama adalah batas bawah
dan baris kedua berisi batas atas.


\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-390.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-390.png)

Kita juga dapat mengisi rentang nilai seperti


$$-1 \le (x^2+y^2)^2-x^2+y^2 \le 0.$$\>plot2d("(x^2+y^2)^2-x^2+y^2",r=1.2,level=[-1;0],style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-392.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-392.png)

\>plot2d("cos(x)","sin(x)^3",xmin=0,xmax=2pi,\>filled,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-393.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-393.png)

# Grafik Fungsi Parametrik

Nilai x tidak perlu diurutkan. (x,y) hanya menggambarkan sebuah kurva.
Jika x diurutkan, kurva tersebut adalah grafik fungsi.


Pada contoh berikut, kita memplot spiral


$$\gamma(t) = t \cdot (\cos(2\pi t),\sin(2\pi t))$$Kita mungkin perlu menggunakan sangat banyak titik untuk tampilan yang
halus atau fungsi adaptive() untuk mengevaluasi ekspresi (lihat fungsi
adaptive() untuk lebih jelasnya).


\>t=linspace(0,1,1000); ...  
\>   plot2d(t\*cos(2\*pi\*t),t\*sin(2\*pi\*t),r=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-395.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-395.png)

Sebagai alternatif, Anda dapat menggunakan dua ekspresi untuk kurva.
Berikut ini memplot kurva yang sama seperti di atas.


\>plot2d("x\*cos(2\*pi\*x)","x\*sin(2\*pi\*x)",xmin=0,xmax=1,r=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-396.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-396.png)

\>t=linspace(0,1,1000); r=exp(-t); x=r\*cos(2pi\*t); y=r\*sin(2pi\*t);

\>plot2d(x,y,r=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-397.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-397.png)

Dalam contoh berikut, kami memplot kurva


$$\gamma(t) = (r(t) \cos(t), r(t) \sin(t))$$dengan


$$r(t) = 1 + \dfrac{\sin(3t)}{2}.$$\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t); ...  
\>   plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-400.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-400.png)

# Menggambar Grafik Bilangan Kompleks

Sebuah deretan bilangan kompleks juga dapat diplot. Kemudian
titik-titik kisi akan dihubungkan. Jika sejumlah garis kisi ditentukan
(atau vektor 1x2 garis kisi) pada argumen cgrid, hanya garis-garis
kisi tersebut yang akan terlihat.


Matriks bilangan kompleks akan secara otomatis diplot sebagai sebuah
grid pada bidang kompleks.


Pada contoh berikut, kita memplot gambar lingkaran satuan di bawah
fungsi eksponensial. Parameter cgrid menyembunyikan beberapa kurva
grid.


\>aspect(); r=linspace(0,1,50); a=linspace(0,2pi,80)'; z=r\*exp(I\*a);...  
\>   plot2d(z,a=-1.25,b=1.25,c=-1.25,d=1.25,cgrid=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-401.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-401.png)

\>aspect(1.25); r=linspace(0,1,50); a=linspace(0,2pi,200)'; z=r\*exp(I\*a);

\>plot2d(exp(z),cgrid=[40,10]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-402.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-402.png)

\>r=linspace(0,1,10); a=linspace(0,2pi,40)'; z=r\*exp(I\*a);

\>plot2d(exp(z),\>points,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-403.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-403.png)

Vektor bilangan kompleks secara otomatis diplot sebagai kurva pada
bidang kompleks dengan bagian nyata dan bagian imajiner.


Pada contoh, kami memplot lingkaran satuan dengan


$$\gamma(t) = e^{it}$$\>t=linspace(0,2pi,1000); ...  
\>   plot2d(exp(I\*t)+exp(4\*I\*t),r=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-405.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-405.png)

# Plot Statistik

Terdapat banyak fungsi yang dikhususkan untuk plot statistik. Salah
satu plot yang sering digunakan adalah plot kolom.


Jumlah kumulatif dari nilai berdistribusi normal 0-1 menghasilkan
jalan acak.


\>plot2d(cumsum(randnormal(1,1000))):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-406.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-406.png)

Dengan menggunakan dua baris, ini menunjukkan jalan di dua dimensi.


\>X=cumsum(randnormal(2,1000)); plot2d(X[1],X[2]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-407.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-407.png)

\>columnsplot(cumsum(random(10)),style="/",color=blue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-408.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-408.png)

Ini juga dapat menampilkan string sebagai label.


\>months=["Jan","Feb","Mar","Apr","May","Jun", ...  
\>     "Jul","Aug","Sep","Oct","Nov","Dec"];

\>values=[10,12,12,18,22,28,30,26,22,18,12,8];

\>columnsplot(values,lab=months,color=red,style="-");

\>title("Temperature"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-409.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-409.png)

\>k=0:10;

\>plot2d(k,bin(10,k),\>bar):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-410.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-410.png)

\>plot2d(k,bin(10,k)); plot2d(k,bin(10,k),\>points,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-411.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-411.png)

\>plot2d(normal(1000),normal(1000),\>points,grid=6,style=".."):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-412.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-412.png)

\>plot2d(normal(1,1000),\>distribution,style="O"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-413.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-413.png)

\>plot2d("qnormal",0,5;2.5,0.5,\>filled):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-414.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-414.png)

Untuk memplot distribusi statistik eksperimental, Anda dapat
menggunakan distribution=n dengan plot2d.


\>w=randexponential(1,1000); // exponential distribution

\>plot2d(w,\>distribution): // or distribution=n with n intervals


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-415.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-415.png)

Atau Anda dapat menghitung distribusi dari data dan memplot hasilnya
dengan &gt;bar di plot3d, atau dengan plot kolom.


\>w=normal(1000); // 0-1-normal distribution

\>{x,y}=histo(w,10,v=[-6,-4,-2,-1,0,1,2,4,6]); // interval bounds v

\>plot2d(x,y,\>bar):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-416.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-416.png)

Fungsi statplot() menetapkan gaya dengan string sederhana.


\>statplot(1:10,cumsum(random(10)),"b"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-417.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-417.png)

\>n=10; i=0:n; ...  
\>   plot2d(i,bin(n,i)/2^n,a=0,b=10,c=0,d=0.3); ...  
\>   plot2d(i,bin(n,i)/2^n,points=true,style="ow",add=true,color=blue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-418.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-418.png)

Selain itu, data dapat diplot sebagai batang. Dalam hal ini, x harus
diurutkan dan satu elemen lebih panjang dari y. Batang akan memanjang
dari x[i] ke x[i+1] dengan nilai y[i]. Jika x memiliki ukuran yang
sama dengan y, maka x akan diperpanjang satu elemen dengan jarak
terakhir.


Gaya isian dapat digunakan seperti di atas.


\>n=10; k=bin(n,0:n); ...  
\>   plot2d(-0.5:n+0.5,k,bar=true,fillcolor=lightgray):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-419.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-419.png)

Data untuk plot batang ( bar = 1) dan histogram (histogram = 1) dapat
diberikan secara eksplisit dalam xv dan yv, atau dapat dihitung dari
distribusi empiris dalam xv dengan &gt;distribution (atau distribution =
n). Histogram dari nilai xv akan dihitung secara otomatis dengan
&gt;histogram. Jika &gt;even ditentukan, nilai xv akan dihitung dalam
interval bilangan bulat.


\>plot2d(normal(10000),distribution=50):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-420.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-420.png)

\>k=0:10; m=bin(10,k); x=(0:11)-0.5; plot2d(x,m,\>bar):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-421.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-421.png)

\>columnsplot(m,k):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-422.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-422.png)

\>plot2d(random(600)\*6,histogram=6):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-423.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-423.png)

Untuk distribusi, ada parameter distribution=n, yang menghitung nilai
secara otomatis dan mencetak distribusi relatif dengan n sub-interval.


\>plot2d(normal(1,1000),distribution=10,style="\\/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-424.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-424.png)

Dengan parameter even=true, ini akan menggunakan interval bilangan
bulat.


\>plot2d(intrandom(1,1000,10),distribution=10,even=true):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-425.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-425.png)

Perhatikan bahwa ada banyak plot statistik yang mungkin berguna.
Lihatlah tutorial tentang statistik.


\>columnsplot(getmultiplicities(1:6,intrandom(1,6000,6))):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-426.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-426.png)

\>plot2d(normal(1,1000),\>distribution); ...  
\>     plot2d("qnormal(x)",color=red,thickness=2,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-427.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-427.png)

Ada juga banyak plot khusus untuk statistik. Boxplot menunjukkan
kuartil dari distribusi ini dan banyak outlier. Menurut definisi,
outlier dalam boxplot adalah data yang melebihi 1,5 kali kisaran 50%
tengah plot.


\>M=normal(5,1000); boxplot(quartiles(M)):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-428.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-428.png)

# Fungsi Implisit

Plot implisit menunjukkan garis level yang menyelesaikan f(x,y)=level,
di mana "level" dapat berupa nilai tunggal atau vektor nilai. Jika
level = "auto", akan ada nc garis level, yang akan menyebar di antara
minimum dan maksimum fungsi secara merata. Warna yang lebih gelap atau
lebih terang dapat ditambahkan dengan &gt;hue untuk mengindikasikan nilai
fungsi. Untuk fungsi implisit, xv haruslah sebuah fungsi atau ekspresi
dari parameter x dan y, atau, sebagai alternatif, xv dapat berupa
matriks nilai.


Euler dapat menandai garis level


$$f(x,y) = c$$dari fungsi apa pun.


Untuk menggambar himpunan f(x,y) = c untuk satu atau lebih konstanta
c, Anda bisa menggunakan plot2d() dengan plot implisitnya pada bidang.
Parameter untuk c adalah level = c, di mana c dapat berupa vektor
garis level. Sebagai tambahan, sebuah skema warna dapat digambar pada
latar belakang untuk mengindikasikan nilai fungsi untuk setiap titik
pada plot. Parameter "n" menentukan kehalusan plot.


\>aspect(1.5); 

\>plot2d("x^2+y^2-x\*y-x",r=1.5,level=0,contourcolor=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-430.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-430.png)

\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=0): // Solutions of f(x,y)=0


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-431.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-431.png)

\>plot2d(expr,level=0:0.5:20,\>hue,contourcolor=white,n=200): // nice


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-432.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-432.png)

\>plot2d(expr,level=0:0.5:20,\>hue,\>spectral,n=200,grid=4): // nicer


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-433.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-433.png)

Hal ini juga berlaku untuk plot data. Tetapi Anda harus menentukan
rentang untuk label sumbu.


\>x=-2:0.05:1; y=x'; z=expr(x,y);

\>plot2d(z,level=0,a=-1,b=2,c=-2,d=1,\>hue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-434.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-434.png)

\>plot2d("x^3-y^2",\>contour,\>hue,\>spectral):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-435.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-435.png)

\>plot2d("x^3-y^2",level=0,contourwidth=3,\>add,contourcolor=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-436.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-436.png)

\>z=z+normal(size(z))\*0.2;

\>plot2d(z,level=0.5,a=-1,b=2,c=-2,d=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-437.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-437.png)

\>plot2d(expr,level=[0:0.2:5;0.05:0.2:5.05],color=lightgray):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-438.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-438.png)

\>plot2d("x^2+y^3+x\*y",level=1,r=4,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-439.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-439.png)

\>plot2d("x^2+2\*y^2-x\*y",level=0:0.1:10,n=100,contourcolor=white,\>hue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-440.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-440.png)

Dimungkinkan juga untuk mengisi set


$$a \le f(x,y) \le b$$dengan rentang level.


Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Untuk
ini, level harus berupa matriks 2xn. Baris pertama adalah batas bawah
dan baris kedua berisi batas atas.


\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-442.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-442.png)

Plot implisit juga dapat menunjukkan rentang level. Maka level harus
berupa matriks 2xn interval level, di mana baris pertama berisi awal
dan baris kedua adalah akhir dari setiap interval. Sebagai alternatif,
vektor baris sederhana dapat digunakan untuk level, dan parameter dl
memperluas nilai level ke interval.


\>plot2d("x^4+y^4",r=1.5,level=[0;1],color=blue,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-443.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-443.png)

\>plot2d("x^2+y^3+x\*y",level=[0,2,4;1,3,5],style="/",r=2,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-444.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-444.png)

\>plot2d("x^2+y^3+x\*y",level=-10:20,r=2,style="-",dl=0.1,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-445.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-445.png)

\>plot2d("sin(x)\*cos(y)",r=pi,\>hue,\>levels,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-446.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-446.png)

Anda juga dapat menandai suatu wilayah


$$a \le f(x,y) \le b.$$Hal ini dilakukan dengan menambahkan level dengan dua baris.


\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>     style="#",color=red,<outline, ...  
\>     level=[-2;0],n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-448.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-448.png)

Dimungkinkan untuk menentukan level tertentu. Sebagai contoh, kita
dapat memplot solusi dari persamaan seperti


$$x^3-xy+x^2y^2=6$$\>plot2d("x^3-x\*y+x^2\*y^2",r=6,level=1,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-450.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-450.png)

\>function starplot1 (v, style="/", color=green, lab=none) ...


      if !holding() then clg; endif;
      w=window(); window(0,0,1024,1024);
      h=holding(1);
      r=max(abs(v))*1.2;
      setplot(-r,r,-r,r);
      n=cols(v); t=linspace(0,2pi,n);
      v=v|v[1]; c=v*cos(t); s=v*sin(t);
      cl=barcolor(color); st=barstyle(style);
      loop 1 to n
        polygon([0,c[#],c[#+1]],[0,s[#],s[#+1]],1);
        if lab!=none then
          rlab=v[#]+r*0.1;
          {col,row}=toscreen(cos(t[#])*rlab,sin(t[#])*rlab);
          ctext(""+lab[#],col,row-textheight()/2);
        endif;
      end;
      barcolor(cl); barstyle(st);
      holding(h);
      window(w);
    endfunction
</pre>
Tidak ada kisi-kisi atau tanda panah sumbu di sini. Selain itu, kami
menggunakan jendela penuh untuk plot.


Kami memanggil reset sebelum kami menguji plot ini untuk mengembalikan
default grafis. Hal ini tidak perlu dilakukan, jika Anda yakin bahwa
plot Anda berfungsi.


\>reset; starplot1(normal(1,10)+5,color=red,lab=1:10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-451.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-451.png)

Terkadang, Anda mungkin ingin memplot sesuatu yang tidak dapat
dilakukan oleh plot2d, tetapi hampir.


Pada fungsi berikut ini, kita akan membuat plot impuls logaritmik.
plot2d dapat membuat plot logaritmik, tetapi tidak untuk batang
impuls.


\>function logimpulseplot1 (x,y) ...


      {x0,y0}=makeimpulse(x,log(y)/log(10));
      plot2d(x0,y0,>bar,grid=0);
      h=holding(1);
      frame();
      xgrid(ticks(x));
      p=plot();
      for i=-10 to 10;
        if i<=p[4] and i>=p[3] then
           ygrid(i,yt="10^"+i);
        endif;
      end;
      holding(h);
    endfunction
</pre>
Mari kita uji dengan nilai yang terdistribusi secara eksponensial.


\>aspect(1.5); x=1:10; y=-log(random(size(x)))\*200; ...  
\>   logimpulseplot1(x,y):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-452.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-452.png)

Mari kita menghidupkan kurva 2D dengan menggunakan plot langsung.
Perintah plot(x,y) hanya memplot kurva ke dalam jendela plot.
setplot(a,b,c,d) mengatur jendela ini.


Fungsi wait(0) memaksa plot untuk muncul pada jendela grafik. Jika
tidak, penggambaran ulang akan dilakukan dalam interval waktu yang
jarang.


\>function animliss (n,m) ...


    t=linspace(0,2pi,500);
    f=0;
    c=framecolor(0);
    l=linewidth(2);
    setplot(-1,1,-1,1);
    repeat
      clg;
      plot(sin(n*t),cos(m*t+f));
      wait(0);
      if testkey() then break; endif;
      f=f+0.02;
    end;
    framecolor(c);
    linewidth(l);
    endfunction
</pre>
Tekan sembarang tombol untuk menghentikan animasi ini.


\>animliss(2,3); // lihat hasilnya, jika sudah puas, tekan ENTER


# Plot Logaritmik

EMT menggunakan parameter "logplot" untuk skala logaritmik.


Plot logaritmik dapat diplot menggunakan skala logaritmik dalam y
dengan logplot = 1, atau menggunakan skala logaritmik dalam x dan y
dengan logplot = 2, atau dalam x dengan logplot = 3.


 - logplot=1: y-logaritmik  
 - logplot=2: x-y-logaritmik  
 - logplot=3: x-logaritmik  

\>plot2d("exp(x^3-x)\*x^2",1,5,logplot=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-453.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-453.png)

\>plot2d("exp(x+sin(x))",0,100,logplot=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-454.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-454.png)

\>plot2d("exp(x+sin(x))",10,100,logplot=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-455.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-455.png)

\>plot2d("gamma(x)",1,10,logplot=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-456.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-456.png)

\>plot2d("log(x\*(2+sin(x/100)))",10,1000,logplot=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-457.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-457.png)

Hal ini juga bisa dilakukan dengan plot data.


\>x=10^(1:20); y=x^2-x;

\>plot2d(x,y,logplot=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-458.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-458.png)

# Rujukan Lengkap Fungsi plot2d()

  function plot2d (xv, yv, btest, a, b, c, d, xmin, xmax, r, n,  ..  
  logplot, grid, frame, framecolor, square, color, thickness, style,  

..


  auto, add, user, delta, points, addpoints, pointstyle, bar,
histogram,  ..


  distribution, even, steps, own, adaptive, hue, level, contour,  ..


  nc, filled, fillcolor, outline, title, xl, yl, maps, contourcolor,
..


  contourwidth, ticks, margin, clipping, cx, cy, insimg, spectral,  ..


  cgrid, vertical, smaller, dl, niveau, levels)


Multipurpose plot function for plots in the plane (2D plots). This
function can do plots of functions of one variables, data plots,
curves in the plane, bar plots, grids of complex numbers, and implicit
plots of functions of two variables.


Parameters


x,y       : equations, functions or data vectors


a,b,c,d   : Plot area (default a=-2,b=2)


r         : if r is set, then a=cx-r, b=cx+r, c=cy-r, d=cy+r


            r can be a vector [rx,ry] or a vector [rx1,rx2,ry1,ry2].


xmin,xmax : range of the parameter for curves


auto      : Determine y-range automatically (default)


square    : if true, try to keep square x-y-ranges


n         : number of intervals (default is adaptive)


grid      : 0 = no grid and labels,


            1 = axis only,


            2 = normal grid (see below for the number of grid lines)


            3 = inside axis


            4 = no grid


            5 = full grid including margin


            6 = ticks at the frame


            7 = axis only


            8 = axis only, sub-ticks


frame     : 0 = no frame


framecolor: color of the frame and the grid


margin    : number between 0 and 0.4 for the margin around the plot


color     : Color of curves. If this is a vector of colors,


            it will be used for each row of a matrix of plots. In the
case of


            point plots, it should be a column vector. If a row vector
or a


            full matrix of colors is used for point plots, it will be
used for


            each data point.


thickness : line thickness for curves


            This value can be smaller than 1 for very thin lines.


style     : Plot style for lines, markers, and fills.


            For points use


            "[]", "&lt;&gt;", ".", "..", "...",


            "*", "+", "|", "-", "o"


            "[]#", "&lt;&gt;#", "o#" (filled shapes)


            "[]w", "&lt;&gt;w", "ow" (non-transparent)


            For lines use


            "-", "--", "-.", ".", ".-.", "-.-", "-&gt;"


            For filled polygons or bar plots use


            "#", "#O", "O", "/", "\", "\/",


            "+", "|", "-", "t"


points    : plot single points instead of line segments


addpoints : if true, plots line segments and points


add       : add the plot to the existing plot


user      : enable user interaction for functions


delta     : step size for user interaction


bar       : bar plot (x are the interval bounds, y the interval
values)


histogram : plots the frequencies of x in n subintervals


distribution=n : plots the distribution of x with n subintervals


even      : use inter values for automatic histograms.


steps     : plots the function as a step function (steps=1,2)


adaptive  : use adaptive plots (n is the minimal number of steps)


level     : plot level lines of an implicit function of two variables


outline   : draws boundary of level ranges.


If the level value is a 2xn matrix, ranges of levels will be drawn


in the color using the given fill style. If outline is true, it


will be drawn in the contour color. Using this feature, regions of


f(x,y) between limits can be marked.


hue       : add hue color to the level plot to indicate the function


            value


contour   : Use level plot with automatic levels


nc        : number of automatic level lines


title     : plot title (default "")


xl, yl    : labels for the x- and y-axis


smaller   : if &gt;0, there will be more space to the left for labels.


vertical  :


  Turns vertical labels on or off. This changes the global variable


  verticallabels locally for one plot. The value 1 sets only vertical


  text, the value 2 uses vertical numerical labels on the y axis.


filled    : fill the plot of a curve


fillcolor : fill color for bar and filled curves


outline   : boundary for filled polygons


logplot   : set logarithmic plots


            1 = logplot in y,


            2 = logplot in xy,


            3 = logplot in x


own       :


  A string, which points to an own plot routine. With &gt;user, you get


  the same user interaction as in plot2d. The range will be set


  before each call to your function.


maps      : map expressions (0 is faster), functions are always
mapped.


contourcolor : color of contour lines


contourwidth : width of contour lines


clipping  : toggles the clipping (default is true)


title     :


  This can be used to describe the plot. The title will appear above


  the plot. Moreover, a label for the x and y axis can be added with


  xl="string" or yl="string". Other labels can be added with the


  functions label() or labelbox(). The title can be a unicode


  string or an image of a Latex formula.


cgrid     :


  Determines the number of grid lines for plots of complex grids.


  Should be a divisor of the the matrix size minus 1 (number of


  subintervals). cgrid can be a vector [cx,cy].


Overview


The function can plot


* 
expressions, call collections or functions of one variable,

* 
parametric curves,

* 
x data against y data,

* 
implicit functions,

* 
bar plots,

* 
complex grids,

* 
polygons.


If a function or expression for xv is given, plot2d() will compute


values in the given range using the function or expression. The


expression must be an expression in the variable x. The range must


be defined in the parameters a and b unless the default range


[-2,2] should be used. The y-range will be computed automatically,


unless c and d are specified, or a radius r, which yields the range


[-r,r] for x and y. For plots of functions, plot2d will use an


adaptive evaluation of the function by default. To speed up the


plot for complicated functions, switch this off with &lt;adaptive, and


optionally decrease the number of intervals n. Moreover, plot2d()


will by default use mapping. I.e., it will compute the plot element


for element. If your expression or your functions can handle a


vector x, you can switch that off with &lt;maps for faster evaluation.


Note that adaptive plots are always computed element for element.


If functions or expressions for both xv and for yv are specified,


plot2d() will compute a curve with the xv values as x-coordinates


and the yv values as y-coordinates. In this case, a range should be


defined for the parameter using xmin, xmax. Expressions contained


---

---

---

# Menggambar Plot 3D dengan EMT

Ini adalah pengenalan plot 3D di Euler. Kita memerlukan plot 3D untuk
memvisualisasikan fungsi dua variabel.


Euler menggambar fungsi tersebut menggunakan algoritma pengurutan
untuk menyembunyikan bagian-bagian di latar belakang. Secara umum,
Euler menggunakan proyeksi pusat. Standarnya adalah dari kuadran x-y
positif ke arah titik asal x=y=z=0, tetapi sudut=0° terlihat dari arah
sumbu y. Sudut pandang dan ketinggian dapat diubah.


Euler dapat memetakan


* 
permukaan dengan bayangan dan garis level atau rentang level,

* 
awan titik-titik,

* 
kurva parametrik,

* 
permukaan implisit.


Plot 3D dari sebuah fungsi menggunakan plot3d. Cara termudah adalah
memplot ekspresi dalam x dan y. Parameter r mengatur rentang plot di
sekitar (0,0).


\>aspect(1.5); plot3d("x^2+sin(y)",-5,5,0,6\*pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-459.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-459.png)

\>plot3d("x^2+x\*sin(y)",-5,5,0,6\*pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-460.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-460.png)

Silakan lakukan modifikasi agar gambar "talang bergelombang" tersebut
tidak lurus melainkan melengkung/melingkar, baik melingkar secara
mendatar maupun melingkar turun/naik (seperti papan peluncur pada
kolam renang. Temukan rumusnya.


# Fungsi dari dua Variabel

Untuk grafik sebuah fungsi, gunakan


* 
ekspresi sederhana dalam x dan y,

* 
nama fungsi dari dua variabell

* 
atau matriks data.


Standarnya adalah kisi-kisi kawat yang terisi dengan warna yang
berbeda di kedua sisi. Perhatikan bahwa jumlah default interval grid
adalah 10, namun plot menggunakan jumlah default 40x40 persegi panjang
untuk membangun permukaan. Hal ini dapat diubah.


* 
n=40, n=[40,40]: jumlah garis kisi di setiap arah

* 
grid=10, grid=[10,10]: jumlah garis grid di setiap arah.


Kami menggunakan default n=40 dan grid=10.


\>plot3d("x^2+y^2"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-461.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-461.png)

Interaksi pengguna dapat dilakukan dengan parameter &gt;user. Pengguna
dapat menekan tombol berikut ini.


* 
left,right,up,down: memutar sudut pandang

* 
+,-: memperbesar atau memperkecil

* 
a: menghasilkan anaglyph (lihat di bawah)

* 
l: beralih memutar sumber cahaya (lihat di bawah)

* 
space: mengatur ulang ke default

* 
return: mengakhiri interaksi


\>plot3d("exp(-x^2+y^2)",\>user, ...  
\>     title="Turn with the vector keys (press return to finish)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-462.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-462.png)

Rentang plot untuk fungsi dapat ditentukan dengan


* 
a, b: rentang x

* 
c, d: rentang y

* 
r: bujur sangkar simetris di sekitar (0,0).

* 
n: jumlah subinterval untuk plot.


Terdapat beberapa parameter untuk menskalakan fungsi atau mengubah
tampilan grafik.


fscale: skala untuk nilai fungsi (standarnya adalah &lt;fscale).


scale: angka atau vektor 1x2 untuk menskalakan ke arah x dan y.


frame: jenis bingkai (default 1).


\>plot3d("exp(-(x^2+y^2)/5)",r=10,n=80,fscale=4,scale=1.2,frame=3,\>user):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-463.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-463.png)

Tampilan dapat diubah dengan berbagai cara.


* 
distance: jarak tampilan ke plot.

* 
zoom: nilai zoom.

* 
angle: sudut ke sumbu y negatif dalam radian.

* 
height: ketinggian tampilan dalam radian.


Nilai default dapat diperiksa atau diubah dengan fungsi view(). Fungsi
ini mengembalikan parameter dalam urutan di atas.


\>view


    [5,  2.6,  2,  0.4]

Jarak yang lebih dekat membutuhkan zoom yang lebih sedikit. Efeknya
lebih seperti lensa sudut lebar.


Dalam contoh berikut ini, angle=0 dan height=0 terlihat dari sumbu y
negatif. Label sumbu untuk y disembunyikan dalam kasus ini.


\>plot3d("x^2+y",distance=3,zoom=1,angle=pi/2,height=0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-464.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-464.png)

Plot terlihat selalu ke bagian tengah kubus plot. Anda dapat
memindahkan bagian tengah dengan parameter center.


\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>     center=[0.4,0,0],zoom=5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-465.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-465.png)

Plot diskalakan agar sesuai dengan kubus satuan untuk dilihat. Jadi,
tidak perlu mengubah jarak atau melakukan zoom, tergantung pada ukuran
plot. Namun demikian, label mengacu ke ukuran yang sesungguhnya.


Jika Anda menonaktifkannya dengan scale=false, Anda harus berhati-hati
agar plot tetap muat di dalam jendela plotting, dengan mengubah jarak
tampilan atau zoom, dan memindahkan bagian tengahnya.


\>plot3d("5\*exp(-x^2-y^2)",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>     center=[0,0,-2],frame=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-466.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-466.png)

Plot polar juga tersedia. Parameter polar=true menggambar plot polar.
Fungsi harus tetap merupakan fungsi dari x dan y. Parameter "fscale"
menskalakan fungsi dengan skala sendiri. Jika tidak, fungsi akan
diskalakan agar sesuai dengan kubus.


\>plot3d("1/(x^2+y^2+1)",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=blue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-467.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-467.png)

\>function f(r) := exp(-r/2)\*cos(r); ...  
\>   plot3d("f(x^2+y^2)",\>polar,scale=[1,1,0.4],r=pi,frame=3,zoom=4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-468.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-468.png)

Parameter rotate memutar fungsi dalam x di sekitar sumbu x.


* 
rotate=1: Menggunakan sumbu x

* 
rotate=2: Menggunakan sumbu z


\>plot3d("x^2+1",a=-1,b=1,rotate=true,grid=5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-469.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-469.png)

\>plot3d("x^2+1",a=-1,b=1,rotate=2,grid=5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-470.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-470.png)

\>plot3d("sqrt(25-x^2)",a=0,b=5,rotate=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-471.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-471.png)

\>plot3d("x\*sin(x)",a=0,b=6pi,rotate=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-472.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-472.png)

Berikut ini adalah plot dengan tiga fungsi.


\>plot3d("x","x^2+y^2","y",r=2,zoom=3.5,frame=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-473.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-473.png)

# Plot Kontur

Untuk plot, Euler menambahkan garis kisi-kisi. Sebagai gantinya,
dimungkinkan untuk menggunakan garis level dan rona satu warna atau
rona berwarna spektral. Euler dapat menggambar ketinggian fungsi pada
plot dengan bayangan. Pada semua plot 3D, Euler dapat menghasilkan
anaglyph merah/cyan.


* 
&gt;hue: Mengaktifkan bayangan cahaya, bukan kabel.

* 
&gt;contour: Memplot garis kontur otomatis pada plot.

* 
level=... (atau levels): Vektor nilai untuk garis kontur.


Defaultnya adalah level="auto", yang menghitung beberapa garis level
secara otomatis. Seperti yang Anda lihat di plot, level sebenarnya
adalah rentang level.


Gaya default dapat diubah. Untuk plot kontur berikut ini, kami
menggunakan grid yang lebih halus untuk titik 100x100, skala fungsi
dan plot, dan menggunakan sudut pandang yang berbeda.


\>plot3d("exp(-x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=45°,height=20°):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-474.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-474.png)

\>plot3d("exp(x\*y)",angle=100°,\>contour,color=green):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-475.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-475.png)

Bayangan default menggunakan warna abu-abu. Tetapi, kisaran warna
spektral juga tersedia.


* 
&gt;spectral: Menggunakan skema spektral default

* 
color =...: Menggunakan warna khusus atau skema spektral


Untuk plot berikut ini, kami menggunakan skema spektral default dan
menambah jumlah titik untuk mendapatkan tampilan yang sangat mulus.


\>plot3d("x^2+y^2",\>spectral,\>contour,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-476.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-476.png)

Alih-alih garis level otomatis, kita juga dapat menetapkan nilai garis
level. Hal ini akan menghasilkan garis level yang tipis, alih-alih
rentang level.


\>plot3d("x^2-y^2",0,5,0,5,level=-1:0.1:1,color=redgreen):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-477.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-477.png)

Pada plot berikut ini, kami menggunakan dua pita level yang sangat
luas dari -0,1 hingga 1, dan dari 0,9 hingga 1. Ini dimasukkan sebagai
matriks dengan batas-batas level sebagai kolom.


Selain itu, kami menghamparkan grid dengan 10 interval di setiap arah.


\>plot3d("x^2+y^3",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=30°,grid=10,contourcolor=gray):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-478.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-478.png)

Pada contoh berikut, kami memplot himpunan, di mana


$$f(x,y) = x^y-y^x = 0$$Kita menggunakan satu garis tipis untuk garis level.


\>plot3d("x^y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=red,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-480.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-480.png)

Dimungkinkan untuk menampilkan bidang kontur di bawah plot. Warna dan
jarak ke plot dapat ditentukan.


\>plot3d("x^2+y^4",\>cp,cpcolor=green,cpdelta=0.2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-481.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-481.png)

Berikut ini beberapa gaya lainnya. Kami selalu mematikan bingkai, dan
menggunakan berbagai skema warna untuk plot dan kisi-kisi.


\>figure(2,2); ...  
\>   expr="y^3-x^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-482.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-482.png)

Ada beberapa skema spektral lainnya, yang diberi nomor dari 1 hingga
9. Tetapi Anda juga dapat menggunakan color=value, di mana value


* 
spectral: untuk rentang dari biru ke merah

* 
white: untuk rentang yang lebih redup

* 
yellowblue (kuning), purplegreen (ungu), blueyellow (biru), greenred
* (hijau)

* 
blueyellow, greenpurple, yellowblue, redgreen


\>figure(3,3); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^2+y^2",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-483.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-483.png)

Sumber cahaya dapat diubah dengan l dan tombol kursor selama interaksi
pengguna. Ini juga dapat ditetapkan dengan parameter.


* 
light: arah cahaya

* 
amb: cahaya sekitar antara 0 dan 1


Perhatikan, bahwa program ini tidak membuat perbedaan di antara
sisi-sisi plot. Tidak ada bayangan. Untuk ini Anda akan membutuhkan
Povray.


\>plot3d("-x^2-y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-484.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-484.png)

Parameter warna mengubah warna permukaan. Warna garis level juga dapat
diubah.


\>plot3d("-x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=red,level=-2:0.1:1,dl=0.01):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-485.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-485.png)

Warna 0 memberikan efek pelangi yang istimewa.


\>plot3d("x^2/(x^2+y^2+1)",color=0,hue=true,grid=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-486.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-486.png)

Permukaannya juga bisa transparan.


\>plot3d("x^2+y^2",\>transparent,grid=10,wirecolor=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-487.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-487.png)

# Plot Implisit

Ada juga plot implisit dalam tiga dimensi. Euler menghasilkan potongan
melalui objek. Fitur plot3d termasuk plot implisit. Plot-plot ini
menunjukkan himpunan nol dari sebuah fungsi dalam tiga variabel.


Solusi dari


$$f(x,y,z) = 0$$dapat divisualisasikan dalam potongan yang sejajar dengan bidang x-y,
bidang x-z, dan bidang y-z.


* 
implicit=1: potong sejajar dengan bidang-y-z

* 
implicit=2: memotong sejajar dengan bidang x-z

* 
implicit=4: memotong sejajar dengan bidang x-y


Tambahkan nilai-nilai ini, jika Anda mau. Pada contoh, kami memplot


$$M = \{ (x,y,z) : x^2+y^3+zy=1 \}$$\>plot3d("x^2+y^3+z\*y-1",r=5,implicit=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-490.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-490.png)

\>c=1; d=1;

\>plot3d("((x^2+y^2-c^2)^2+(z^2-1)^2)\*((y^2+z^2-c^2)^2+(x^2-1)^2)\*((z^2+x^2-c^2)^2+(y^2-1)^2)-d",r=2,<frame,\>implicit,\>user): 


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-491.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-491.png)

\>plot3d("x^2+y^2+4\*x\*z+z^3",\>implicit,r=2,zoom=2.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-492.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-492.png)

# Memplot Data 3D

Sama seperti plot2d, plot3d menerima data. Untuk objek 3D, Anda perlu
menyediakan matriks nilai x, y, dan z, atau tiga fungsi atau ekspresi
fx(x,y), fy(x,y), fz(x,y).


$$\gamma(t,s) = (x(t,s),y(t,s),z(t,s))$$Karena x,y,z adalah matriks, kita mengasumsikan bahwa (t,s) berjalan
melalui kotak persegi. Hasilnya, Anda dapat memplot gambar persegi
panjang dalam ruang.


Anda dapat menggunakan bahasa matriks Euler untuk menghasilkan
koordinat secara efektif.


Pada contoh berikut, kita menggunakan vektor nilai t dan vektor kolom
nilai s untuk memparameterkan permukaan bola. Pada gambar kita dapat
menandai daerah, dalam kasus kita daerah kutub.


\>t=linspace(0,2pi,180); s=linspace(-pi/2,pi/2,90)'; ...  
\>   x=cos(s)\*cos(t); y=cos(s)\*sin(t); z=sin(s); ...  
\>   plot3d(x,y,z,\>hue, ...  
\>   color=blue,<frame,grid=[10,20], ...  
\>   values=s,contourcolor=red,level=[90°-24°;90°-22°], ...  
\>   scale=1.4,height=50°):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-494.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-494.png)

Berikut ini adalah contoh, yang merupakan grafik suatu fungsi.


\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s,grid=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-495.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-495.png)

Namun demikian, kita bisa membuat segala macam permukaan. Berikut ini
adalah permukaan yang sama dengan fungsi


$$x = y \, z$$\>plot3d(t\*s,t,s,angle=180°,grid=10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-497.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-497.png)

Dengan lebih banyak upaya, kita bisa menghasilkan banyak permukaan.


Dalam contoh berikut ini, kami membuat tampilan berbayang dari bola
yang terdistorsi. Koordinat yang biasa digunakan untuk bola adalah


$$\gamma(t,s) = (\cos(t)\cos(s),\sin(t)\sin(s),\cos(s))$$dengan


$$0 \le t \le 2\pi, \quad \frac{-\pi}{2} \le s \le \frac{\pi}{2}.$$Kami mengubahnya dengan sebuah faktor


$$d(t,s) = \frac{\cos(4t)+\cos(8s)}{4}.$$\>t=linspace(0,2pi,320); s=linspace(-pi/2,pi/2,160)'; ...  
\>   d=1+0.2\*(cos(4\*t)+cos(8\*s)); ...  
\>   plot3d(cos(t)\*cos(s)\*d,sin(t)\*cos(s)\*d,sin(s)\*d,hue=1, ...  
\>     light=[1,0,1],frame=0,zoom=5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-501.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-501.png)

Tentu saja, point cloud juga dimungkinkan. Untuk memplot data titik
dalam ruang, kita membutuhkan tiga vektor untuk koordinat titik.


Gaya-gayanya sama seperti pada plot2d dengan points=true;


\>n=500;  ...  
\>     plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="."):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-502.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-502.png)

Anda juga dapat memplot kurva dalam bentuk 3D. Dalam hal ini, akan
lebih mudah untuk menghitung titik-titik kurva. Untuk kurva pada
bidang, kami menggunakan urutan koordinat dan parameter wire=true.


\>t=linspace(0,8pi,500); ...  
\>   plot3d(sin(t),cos(t),t/10,\>wire,zoom=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-503.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-503.png)

\>t=linspace(0,4pi,1000); plot3d(cos(t),sin(t),t/2pi,\>wire, ...  
\>   linewidth=3,wirecolor=blue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-504.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-504.png)

\>X=cumsum(normal(3,100)); ...  
\>    plot3d(X[1],X[2],X[3],\>anaglyph,\>wire):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-505.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-505.png)

EMT juga dapat membuat plot dalam mode anaglyph. Untuk melihat plot
semacam itu, Anda memerlukan kacamata merah/cyan. 


\> plot3d("x^2+y^3",\>anaglyph,\>contour,angle=30°):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-506.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-506.png)

Sering kali, skema warna spektral digunakan untuk plot. Hal ini
menekankan ketinggian fungsi.


\>plot3d("x^2\*y^3-y",\>spectral,\>contour,zoom=3.2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-507.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-507.png)

Euler juga dapat memplot permukaan yang diparameterkan, ketika
parameternya adalah nilai x, y, dan z dari gambar kisi-kisi persegi
panjang di dalam ruang.


Untuk demo berikut ini, kami menyiapkan parameter u dan v, dan
menghasilkan koordinat ruang dari parameter ini.


\>u=linspace(-1,1,10); v=linspace(0,2\*pi,50)'; ...  
\>   X=(3+u\*cos(v/2))\*cos(v); Y=(3+u\*cos(v/2))\*sin(v); Z=u\*sin(v/2); ...  
\>   plot3d(X,Y,Z,\>anaglyph,<frame,\>wire,scale=2.3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-508.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-508.png)

Berikut ini contoh yang lebih rumit, yang tampak megah dengan kacamata
merah/cyan.


\>u:=linspace(-pi,pi,160); v:=linspace(-pi,pi,400)';  ...  
\>   x:=(4\*(1+.25\*sin(3\*v))+cos(u))\*cos(2\*v); ...  
\>   y:=(4\*(1+.25\*sin(3\*v))+cos(u))\*sin(2\*v); ...  
\>    z=sin(u)+2\*cos(3\*v); ...  
\>   plot3d(x,y,z,frame=0,scale=1.5,hue=1,light=[1,0,-1],zoom=2.8,\>anaglyph):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-509.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-509.png)

# Plot Statistik

Plot batang juga dapat digunakan. Untuk ini, kita harus menyediakan


* 
x: vektor baris dengan n+1 elemen

* 
y: vektor kolom dengan n+1 elemen

* 
z: matriks nilai berukuran nxn.


z dapat lebih besar, tetapi hanya nilai nxn yang akan digunakan.


Pada contoh, pertama-tama kita menghitung nilainya. Kemudian kita
sesuaikan x dan y, sehingga vektor berada di tengah-tengah nilai yang
digunakan.


\>x=-1:0.1:1; y=x'; z=x^2+y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-510.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-510.png)

Dimungkinkan untuk membagi plot permukaan menjadi dua bagian atau
lebih.


\>x=-1:0.1:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-511.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-511.png)

Jika memuat atau menghasilkan matriks data M dari file dan perlu
memplotnya dalam 3D, Anda dapat menskalakan matriks ke [-1,1] dengan
scale(M), atau menskalakan matriks dengan &gt;zscale. Hal ini dapat
dikombinasikan dengan faktor penskalaan individual yang diterapkan
sebagai tambahan.


\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,1.5],angle=-40°,zoom=1.8):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-512.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-512.png)

\>Z=intrandom(5,100,6); v=zeros(5,6); ...  
\>   loop 1 to 5; v[#]=getmultiplicities(1:6,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:5,ccols=[1:5]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-513.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-513.png)

# Permukaan Benda Putar

\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=red,<outline, ...  
\>   level=[-2;0],n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-514.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-514.png)

\>ekspresi &= (x^2+y^2-1)^3-x^2\*y^3; $ekspresi


$$\left(y^2+x^2-1\right)^3-x^2\,y^3$$Kami ingin memutar kurva jantung di sekitar sumbu y. Berikut ini
adalah ekspresi yang mendefinisikan jantung:


$$f(x,y)=(x^2+y^2-1)^3-x^2.y^3.$$Selanjutnya kita atur


$$x=r.cos(a),\quad y=r.sin(a).$$\>function fr(r,a) &= ekspresi with [x=r\*cos(a),y=r\*sin(a)] | trigreduce; $fr(r,a)


$$\left(r^2-1\right)^3+\frac{\left(\sin \left(5\,a\right)-\sin \left(  3\,a\right)-2\,\sin a\right)\,r^5}{16}$$Hal ini memungkinkan untuk mendefinisikan fungsi numerik, yang
menyelesaikan untuk r, jika a diberikan. Dengan fungsi tersebut kita
dapat memplotkan jantung yang diputar sebagai permukaan parametrik.


\>function map f(a) := bisect("fr",0,2;a); ...  
\>   t=linspace(-pi/2,pi/2,100); r=f(t);  ...  
\>   s=linspace(pi,2pi,100)'; ...  
\>   plot3d(r\*cos(t)\*sin(s),r\*cos(t)\*cos(s),r\*sin(t), ...  
\>   \>hue,<frame,color=red,zoom=4,amb=0,max=0.7,grid=12,height=50°):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-519.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-519.png)

Berikut ini adalah plot 3D dari gambar di atas yang diputar
mengelilingi sumbu-z. Kami mendefinisikan fungsi, yang menggambarkan
objek.


\>function f(x,y,z) ...


    r=x^2+y^2;
    return (r+z^2-1)^3-r*z^3;
     endfunction
</pre>
\>plot3d("f(x,y,z)", ...  
\>   xmin=0,xmax=1.2,ymin=-1.2,ymax=1.2,zmin=-1.2,zmax=1.4, ...  
\>   implicit=1,angle=-30°,zoom=2.5,n=[10,100,60],\>anaglyph):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-520.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-520.png)

# Plot 3D Khusus

Fungsi plot3d memang bagus untuk dimiliki, tetapi tidak memenuhi semua
kebutuhan. Selain rutinitas yang lebih mendasar, Anda juga bisa
mendapatkan plot berbingkai dari objek apa pun yang Anda sukai.


Meskipun Euler bukan program 3D, namun dapat menggabungkan beberapa
objek dasar. Kami mencoba memvisualisasikan parabola dan garis
singgungnya.


\>function myplot ...


      y=-1:0.01:1; x=(-1:0.01:1)';
      plot3d(x,y,0.2*(x-0.1)/2,<scale,<frame,>hue, ..
        hues=0.5,>contour,color=orange);
      h=holding(1);
      plot3d(x,y,(x^2+y^2)/2,<scale,<frame,>contour,>hue);
      holding(h);
    endfunction
</pre>
Sekarang framedplot() menyediakan frame, dan mengatur tampilan.


\>framedplot("myplot",[-1,1,-1,1,0,1],height=0,angle=-30°, ...  
\>     center=[0,0,-0.7],zoom=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-521.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-521.png)

Dengan cara yang sama, Anda dapat memplot bidang kontur secara manual.
Perhatikan bahwa plot3d() mengatur jendela ke fullwindow() secara
default, namun plotcontourplane() mengasumsikannya.


\>x=-1:0.02:1.1; y=x'; z=x^2-y^4;

\>function myplot (x,y,z) ...  
\>  
<pre class="udf">      zoom(2);
      wi=fullwindow();
      plotcontourplane(x,y,z,level="auto",<scale);
      plot3d(x,y,z,>hue,<scale,>add,color=white,level="thin");
      window(wi);
      reset();
    endfunction
</pre>
\>myplot(x,y,z):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-522.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-522.png)

# Animasi

Euler dapat menggunakan frame untuk melakukan pra-komputasi animasi.


Salah satu fungsi yang memanfaatkan teknik ini adalah rotate. Fungsi
ini dapat mengubah sudut pandang dan menggambar ulang plot 3D. Fungsi
ini memanggil addpage() untuk setiap plot baru. Akhirnya fungsi ini
menganimasikan plot tersebut.


Silakan pelajari sumber dari rotate untuk melihat lebih detail.


\>function testplot () := plot3d("x^2+y^3"); ...  
\>   rotate("testplot"); testplot():


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-523.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-523.png)

# Menggambar Povray

Dengan bantuan file Euler povray.e, Euler dapat menghasilkan file
Povray. Hasilnya sangat bagus untuk dilihat.


Anda perlu menginstal Povray (32bit atau 64bit) dari
  <a href="http://www.povray.org/, dan meletakkan sub-direktori "bin" dari Povray ke dalam environment path, atau mengatur variabel "defaultpovray" dengan full path yang mengarah ke "pvengine.exe".">http://www.povray.org/, dan meletakkan sub-direktori "bin" dari Povray ke dalam environment path, atau mengatur variabel "defaultpovray" dengan full path yang mengarah ke "pvengine.exe".</a>


Interface Povray dari Euler menghasilkan file Povray di home direktori
pengguna, dan memanggil Povray untuk mem-parsing file-file ini. Nama
file default adalah current.pov, dan direktori defaultnya adalah
eulerhome(), biasanya c:\Users\Username\Euler. Povray menghasilkan
sebuah file PNG, yang dapat dimuat oleh Euler ke dalam notebook. Untuk
membersihkan berkas-berkas ini, gunakan povclear().


Fungsi pov3d memiliki semangat yang sama dengan plot3d. Fungsi ini
dapat menghasilkan grafik dari sebuah fungsi f(x,y), atau sebuah
permukaan dengan koordinat X,Y,Z dalam bentuk matriks, termasuk
garis-garis level yang bersifat opsional. Fungsi ini memulai raytracer
secara otomatis, dan memuat adegan ke dalam notebook Euler.


Selain pov3d(), ada banyak fungsi yang menghasilkan objek Povray.
Fungsi-fungsi ini mengembalikan string, yang berisi kode Povray untuk
objek. Untuk menggunakan fungsi-fungsi ini, mulai file Povray dengan
povstart(). Kemudian gunakan writeln(...) untuk menulis objek ke scene
file. Terakhir, akhiri file dengan povend(). Secara default, raytracer
akan dimulai, dan PNG akan dimasukkan ke dalam buku catatan Euler.


Fungsi objek memiliki parameter yang disebut "look", yang membutuhkan
string dengan kode povray untuk tekstur dan hasil akhir objek. Fungsi
povlook() dapat digunakan untuk menghasilkan string ini. Fungsi ini
memiliki parameter untuk warna, transparansi, Phong Shading, dll.


Perhatikan bahwa Povray universe memiliki sistem koordinat lain.
Interface ini menerjemahkan semua koordinat ke sistem Povray. Jadi
Anda dapat tetap berpikir dalam sistem koordinat Euler dengan z yang
mengarah vertikal ke atas, dan sumbu x, y, z di tangan kanan.


Anda perlu memuat file povray.


\>load povray;


Pastikan Povray bin directory berada di dalam path. Jika tidak, edit
variabel berikut sehingga berisi jalur ke povray yang dapat
dieksekusi.


\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Untuk kesan pertama, kita plot sebuah fungsi sederhana. Perintah
berikut ini menghasilkan file povray di user directory anda, dan
menjalankan Povray untuk melacak sinar pada file ini.


Jika Anda memulai perintah berikut, GUI Povray akan terbuka,
menjalankan file, dan menutup secara otomatis. Karena alasan keamanan,
Anda akan ditanya, apakah Anda ingin mengizinkan file exe dijalankan.
Anda dapat menekan cancel untuk menghentikan pertanyaan lebih lanjut.
Anda mungkin harus menekan OK pada jendela Povray untuk mengetahui
dialog awal Povray.


\>plot3d("x^2+y^2",zoom=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-524.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-524.png)

\>pov3d("x^2+y^2",zoom=3);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-525.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-525.png)

Kita dapat membuat fungsi menjadi transparan dan menambahkan hasil
akhir lainnya. Kita juga dapat menambahkan garis level ke plot fungsi.


\>pov3d("x^2+y^3",axiscolor=red,angle=-45°,\>anaglyph, ...  
\>     look=povlook(cyan,0.2),level=-1:0.5:1,zoom=3.8);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-526.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-526.png)

Kadang-kadang perlu untuk mencegah penskalaan fungsi, dan menskalakan
fungsi dengan tangan.


Kami memplot kumpulan titik pada bidang kompleks, di mana hasil kali
jarak ke 1 dan -1 sama dengan 1.


\>pov3d("((x-1)^2+y^2)\*((x+1)^2+y^2)/40",r=2, ...  
\>     angle=-120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=10°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-527.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-527.png)

# Merencanakan dengan Koordinat

Sebagai pengganti fungsi, kita dapat membuat plot dengan koordinat.
Seperti pada plot3d, kita membutuhkan tiga matriks untuk
mendefinisikan objek.


Pada contoh, kita memutar sebuah fungsi pada sumbu z.


\>function f(x) := x^3-x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,50)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,look=povlook(red,0.1),height=50°,axis=0,zoom=4,light=[10,5,15]);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-528.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-528.png)

Pada contoh berikut, kita memplot damped wave (gelombang teredam).
Kami menghasilkan gelombang dengan bahasa matriks Euler.


Kami juga menunjukkan, bagaimana objek tambahan dapat ditambahkan ke
adegan pov3d. Untuk pembuatan objek, lihat contoh berikut. Perhatikan
bahwa plot3d menskalakan plot, sehingga sesuai dengan kubus satuan.


\>r=linspace(0,1,80); phi=linspace(0,2pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=6,axis=0,height=30°,add=povsphere([0.5,0,0.25],0.15,povlook(red)), ...  
\>     w=500,h=300);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-529.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-529.png)

Dengan metode bayangan canggih Povray, hanya sedikit titik yang bisa
menghasilkan permukaan yang sangat halus. Hanya pada batas-batas dan
bayangan, trik ini bisa terlihat jelas.


Untuk itu, kita perlu menambahkan vektor normal di setiap titik
matriks.


\>Z &= x^2\*y^3


    
                                     2  3
                                    x  y
    

Persamaan permukaannya adalah [x,y,Z]. Kami menghitung dua turunan
terhadap x dan y dari persamaan ini dan mengambil hasil perkalian
silang sebagai normal.


\>dx &= diff([x,y,Z],x); dy &= diff([x,y,Z],y);


Kami mendefinisikan normal sebagai hasil kali silang dari turunan ini,
dan mendefinisikan fungsi koordinat.


\>N &= crossproduct(dx,dy); NX &= N[1]; NY &= N[2]; NZ &= N[3]; N,


    
                                   3       2  2
                           [- 2 x y , - 3 x  y , 1]
    

Kami hanya menggunakan 25 titik.


\>x=-1:0.5:1; y=x';

\>pov3d(x,y,Z(x,y),angle=10°, ...  
\>     xv=NX(x,y),yv=NY(x,y),zv=NZ(x,y),<shadow);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-530.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-530.png)

Berikut ini adalah simpul Trefoil yang dibuat oleh A. Busser di
Povray. Ada versi yang lebih baik dari ini dalam contoh.


  <a href="Examples\Trefoil Knot.html">Trefoil Knot</a>  

Untuk tampilan yang bagus dengan tidak terlalu banyak titik, kita
tambahkan vektor normal di sini. Kita menggunakan Maxima untuk
menghitung normal untuk kita. Pertama, tiga fungsi untuk koordinat
sebagai ekspresi simbolik.


\>X &= ((4+sin(3\*y))+cos(x))\*cos(2\*y); ...  
\>   Y &= ((4+sin(3\*y))+cos(x))\*sin(2\*y); ...  
\>   Z &= sin(x)+2\*cos(3\*y);


Kemudian dua vektor turunan terhadap x dan y.


\>dx &= diff([X,Y,Z],x); dy &= diff([X,Y,Z],y);


Sekarang yang normal, yang merupakan produk silang dari dua turunan.


\>dn &= crossproduct(dx,dy);


Kami sekarang mengevaluasi semua ini secara numerik.


\>x:=linspace(-%pi,%pi,40); y:=linspace(-%pi,%pi,100)';


Vektor normal adalah evaluasi dari ekspresi simbolik dn[i] untuk
i=1,2,3. Sintaks untuk ini adalah &amp;"ekspresi"(parameter). Ini adalah
sebuah alternatif dari metode pada contoh sebelumnya, di mana kita
mendefinisikan ekspresi simbolik NX, NY, NZ terlebih dahulu.


\>pov3d(X(x,y),Y(x,y),Z(x,y),\>anaglyph,axis=0,zoom=5,w=450,h=350, ...  
\>     <shadow,look=povlook(blue), ...  
\>     xv=&"dn[1]"(x,y), yv=&"dn[2]"(x,y), zv=&"dn[3]"(x,y));


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-531.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-531.png)

Kami juga dapat menghasilkan grid dalam bentuk 3D.


\>povstart(zoom=4); ...  
\>   x=-1:0.5:1; r=1-(x+1)^2/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-532.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-532.png)

Dengan povgrid(), kurva dapat dibuat.


\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*10\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=3); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-533.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-533.png)

# Objek Povray

Di atas, kami menggunakan pov3d untuk memplot permukaan. Interface
povray di Euler juga dapat menghasilkan objek Povray. Objek-objek ini
disimpan sebagai string di Euler, dan perlu ditulis ke file Povray.


Kita memulai output dengan povstart().


\>povstart(zoom=4);


Pertama, kita mendefinisikan tiga silinder, dan menyimpannya dalam
bentuk string di Euler.


Fungsi povx() dll. hanya mengembalikan vektor [1,0,0], yang dapat
digunakan sebagai gantinya.


\>c1=povcylinder(-povx,povx,1,povlook(red)); ...  
\>   c2=povcylinder(-povy,povy,1,povlook(yellow)); ...  
\>   c3=povcylinder(-povz,povz,1,povlook(blue)); ...  
\>  
String berisi kode Povray, yang tidak perlu kita pahami pada saat itu.


\>c2


    cylinder { &lt;0,0,-1&gt;, &lt;0,0,1&gt;, 1
     texture { pigment { color rgb &lt;0.941176,0.941176,0.392157&gt; }  } 
     finish { ambient 0.2 } 
     }

Seperti yang Anda lihat, kami menambahkan tekstur ke objek dalam tiga
warna berbeda.


Hal ini dilakukan dengan povlook(), yang mengembalikan sebuah string
dengan kode Povray yang relevan. Kita dapat menggunakan warna default
Euler, atau menentukan warna kita sendiri. Kita juga dapat menambahkan
transparansi, atau mengubah cahaya sekitar.


\>povlook(rgb(0.1,0.2,0.3),0.1,0.5)


     texture { pigment { color rgbf &lt;0.101961,0.2,0.301961,0.1&gt; }  } 
     finish { ambient 0.5 } 
    

Sekarang kita mendefinisikan objek perpotongan, dan menulis hasilnya
ke file.


\>writeln(povintersection([c1,c2,c3]));


Perpotongan tiga silinder sulit dibayangkan, jika Anda belum pernah
melihatnya.


\>povend;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-534.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-534.png)

Fungsi-fungsi berikut ini menghasilkan fraktal secara rekursif.


Fungsi pertama menunjukkan, bagaimana Euler menangani objek Povray
sederhana. Fungsi povbox() mengembalikan sebuah string, yang berisi
koordinat kotak, tekstur dan hasil akhir.


\>function onebox(x,y,z,d) := povbox([x,y,z],[x+d,y+d,z+d],povlook());

\>function fractal (x,y,z,h,n) ...  
\>  
<pre class="udf">     if n==1 then writeln(onebox(x,y,z,h));
     else
       h=h/3;
       fractal(x,y,z,h,n-1);
       fractal(x+2*h,y,z,h,n-1);
       fractal(x,y+2*h,z,h,n-1);
       fractal(x,y,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z,h,n-1);
       fractal(x+2*h,y,z+2*h,h,n-1);
       fractal(x,y+2*h,z+2*h,h,n-1);
       fractal(x+2*h,y+2*h,z+2*h,h,n-1);
       fractal(x+h,y+h,z+h,h,n-1);
     endif;
    endfunction
</pre>
\>povstart(fade=10,<shadow);

\>fractal(-1,-1,-1,2,4);

\>povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-535.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-535.png)

Differences memungkinkan pemotongan satu objek dari objek lainnya.
Seperti persimpangan, ada bagian dari objek CSG Povray.


\>povstart(light=[5,-5,5],fade=10);


Untuk demonstrasi ini, kita akan mendefinisikan sebuah objek di
Povray, alih-alih menggunakan sebuah string di Euler. Definisi akan
langsung dituliskan ke file.


A box coordinate -1 berarti [-1,-1,-1].


\>povdefine("mycube",povbox(-1,1));


Kita dapat menggunakan objek ini dalam povobject(), yang mengembalikan
sebuah string seperti biasa.


\>c1=povobject("mycube",povlook(red));


Kami menghasilkan kubus kedua, dan memutar serta menskalakannya
sedikit.


\>c2=povobject("mycube",povlook(yellow),translate=[1,1,1], ...  
\>     rotate=xrotate(10°)+yrotate(10°), scale=1.2);


Kemudian kita ambil difference (selisih) dari kedua objek tersebut.


\>writeln(povdifference(c1,c2));


Sekarang tambahkan tiga sumbu.


\>writeAxis(-1.2,1.2,axis=1); ...  
\>   writeAxis(-1.2,1.2,axis=2); ...  
\>   writeAxis(-1.2,1.2,axis=4); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-536.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-536.png)

# Fungsi Implisit

Povray dapat memplot himpunan di mana f(x,y,z)=0, seperti parameter
implisit di plot3d. Namun, hasilnya terlihat jauh lebih baik.


Sintaks untuk fungsi-fungsi tersebut sedikit berbeda. Anda tidak dapat
menggunakan output dari ekspresi Maxima atau Euler.


$$((x^2+y^2-c^2)^2+(z^2-1)^2)*((y^2+z^2-c^2)^2+(x^2-1)^2)*((z^2+x^2-c^2)^2+(y^2-1)^2)=d$$\>povstart(angle=70°,height=50°,zoom=4);

\>c=0.1; d=0.1; ...  
\>   writeln(povsurface("(pow(pow(x,2)+pow(y,2)-pow(c,2),2)+pow(pow(z,2)-1,2))\*(pow(pow(y,2)+pow(z,2)-pow(c,2),2)+pow(pow(x,2)-1,2))\*(pow(pow(z,2)+pow(x,2)-pow(c,2),2)+pow(pow(y,2)-1,2))-d",povlook(red))); ...  
\>   povend();


    Error : Povray error!
    
    Error generated by error() command
    
    povray:
        error("Povray error!");
    Try "trace errors" to inspect local variables after errors.
    povend:
        povray(file,w,h,aspect,exit); 

\>povstart(angle=25°,height=10°); 

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(blue),povbox(-2,2,"")));

\>povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-538.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-538.png)

\>povstart(angle=70°,height=50°,zoom=4);


Membuat permukaan implisit. Perhatikan sintaks yang berbeda dalam
ekspresi.


\>writeln(povsurface("pow(x,2)\*y-pow(y,3)-pow(z,2)",povlook(green))); ...  
\>   writeAxes(); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-539.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-539.png)

# Objek Jaring

Pada contoh ini, kami menunjukkan cara membuat objek mesh, dan
menggambarnya dengan informasi tambahan.


Kami ingin memaksimalkan xy di bawah kondisi x+y = 1 dan
mendemonstrasikan sentuhan tangensial dari garis level.


\>povstart(angle=-10°,center=[0.5,0.5,0.5],zoom=7);


Kita tidak dapat menyimpan objek dalam sebuah string seperti
sebelumnya, karena ukurannya terlalu besar. Jadi kita mendefinisikan
objek dalam file Povray menggunakan #declare. Fungsi povtriangle()
melakukan hal ini secara otomatis. Fungsi ini dapat menerima vektor
normal seperti halnya pov3d().


Berikut ini mendefinisikan objek mesh, dan menuliskannya langsung ke
dalam file.


\>x=0:0.02:1; y=x'; z=x\*y; vx=-y; vy=-x; vz=1;

\>mesh=povtriangles(x,y,z,"",vx,vy,vz);


Sekarang kita tentukan dua cakram, yang akan berpotongan dengan
permukaan.


\>cl=povdisc([0.5,0.5,0],[1,1,0],2); ...  
\>   ll=povdisc([0,0,1/4],[0,0,1],2);


Tuliskan permukaan dikurangi kedua cakram.


\>writeln(povdifference(mesh,povunion([cl,ll]),povlook(green)));


Tuliskan kedua perpotongan tersebut.


\>writeln(povintersection([mesh,cl],povlook(red))); ...  
\>   writeln(povintersection([mesh,ll],povlook(gray)));


Tulislah satu titik secara maksimal.


\>writeln(povpoint([1/2,1/2,1/4],povlook(gray),size=2\*defaultpointsize));


Tambahkan sumbu dan selesaikan.


\>writeAxes(0,1,0,1,0,1,d=0.015); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-540.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-540.png)

# Anaglyph dalam Povray

Untuk menghasilkan anaglyph untuk kacamata merah/cyan, Povray harus
dijalankan dua kali dari posisi kamera yang berbeda. Ini menghasilkan
dua file Povray dan dua file PNG, yang dimuat dengan fungsi
loadanaglyph().


Tentu saja, Anda membutuhkan kacamata merah/cyan untuk melihat contoh
berikut dengan benar.


Fungsi pov3d() memiliki tombol sederhana untuk menghasilkan anaglyph.


\>pov3d("-exp(-x^2-y^2)/2",r=2,height=45°,\>anaglyph, ...  
\>     center=[0,0,0.5],zoom=3.5);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-541.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-541.png)

Jika Anda membuat scene dengan objek, Anda harus menempatkan pembuatan
scene ke dalam suatu fungsi, dan menjalankannya dua kali dengan nilai
yang berbeda untuk parameter anaglyph.


\>function myscene ...


      s=povsphere(povc,1);
      cl=povcylinder(-povz,povz,0.5);
      clx=povobject(cl,rotate=xrotate(90°));
      cly=povobject(cl,rotate=yrotate(90°));
      c=povbox([-1,-1,0],1);
      un=povunion([cl,clx,cly,c]);
      obj=povdifference(s,un,povlook(red));
      writeln(obj);
      writeAxes();
    endfunction
</pre>
Fungsi povanaglyph() melakukan semua ini. Parameter-parameternya
seperti pada povstart() dan povend() yang digabungkan.


\>povanaglyph("myscene",zoom=4.5);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-542.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-542.png)

# Mendefinisikan Objek sendiri

Interfaces povray dari Euler berisi banyak objek. Namun Anda tidak
dibatasi pada objek-objek tersebut. Anda dapat membuat objek sendiri,
yang menggabungkan objek-objek lain, atau objek yang benar-benar baru.


Kami mendemonstrasikan sebuah torus. Perintah Povray untuk ini adalah
"torus". Jadi kita mengembalikan sebuah string dengan perintah ini dan
parameternya. Perhatikan bahwa torus selalu berpusat pada titik asal.


\>function povdonat (r1,r2,look="") ...


      return "torus {"+r1+","+r2+look+"}";
    endfunction
</pre>
Inilah torus pertama kami.


\>t1=povdonat(0.8,0.2)


    torus {0.8,0.2}

Mari kita gunakan objek ini untuk membuat torus kedua, ditranslasikan
dan diputar.


\>t2=povobject(t1,rotate=xrotate(90°),translate=[0.8,0,0])


    object { torus {0.8,0.2}
     rotate 90 *x 
     translate &lt;0.8,0,0&gt;
     }

Sekarang, kita tempatkan semua benda ini ke dalam suatu pemandangan.
Untuk tampilannya, kami menggunakan Phong Shading.


\>povstart(center=[0.4,0,0],angle=0°,zoom=3.8,aspect=1.5); ...  
\>   writeln(povobject(t1,povlook(green,phong=1))); ...  
\>   writeln(povobject(t2,povlook(green,phong=1))); ...  
\>  
 &gt;povend();  

memanggil program Povray. Namun, jika terjadi kesalahan, program ini
tidak menampilkan kesalahan. Oleh karena itu, Anda harus menggunakan


&gt;povend(&lt;exit);


jika ada yang tidak berhasil. Ini akan membiarkan jendela Povray tetap
terbuka.


\>povend(h=320,w=480);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-543.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-543.png)

Berikut adalah contoh yang lebih rumit. Kami menyelesaikan


$$Ax \le b, \quad x \ge 0, \quad c.x \to \text{Max.}$$dan menunjukkan titik-titik yang layak dan optimal dalam plot 3D.


\>A=[10,8,4;5,6,8;6,3,2;9,5,6];

\>b=[10,10,10,10]';

\>c=[1,1,1];


Pertama, mari kita periksa, apakah contoh ini memiliki solusi atau
tidak.


\>x=simplex(A,b,c,\>max,\>check)'


    [0,  1,  0.5]

Ya, benar.


Selanjutnya kita mendefinisikan dua objek. Yang pertama adalah bidang


$$a \cdot x \le b$$\>function oneplane (a,b,look="") ...


      return povplane(a,b,look)
    endfunction
</pre>
Kemudian kita tentukan perpotongan semua setengah ruang dan kubus.


\>function adm (A, b, r, look="") ...


      ol=[];
      loop 1 to rows(A); ol=ol|oneplane(A[#],b[#]); end;
      ol=ol|povbox([0,0,0],[r,r,r]);
      return povintersection(ol,look);
    endfunction
</pre>
Sekarang, kita bisa memplot scene-nya.


\>povstart(angle=120°,center=[0.5,0.5,0.5],zoom=3.5); ...  
\>   writeln(adm(A,b,2,povlook(green,0.4))); ...  
\>   writeAxes(0,1.3,0,1.6,0,1.5); ...  
\>  
Berikut ini adalah lingkaran di sekeliling optimal.


\>writeln(povintersection([povsphere(x,0.5),povplane(c,c.x')], ...  
\>     povlook(red,0.9)));


Dan eror pada arah yang optimal.


\>writeln(povarrow(x,c\*0.5,povlook(red)));


Kami menambahkan teks ke layar. Teks hanyalah sebuah objek 3D. Kita
perlu menempatkan dan memutarnya sesuai dengan pandangan kita.


\>writeln(povtext("Linear Problem",[0,0.2,1.3],size=0.05,rotate=5°)); ...  
\>   povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-546.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-546.png)

# Contoh Lainnya

Anda dapat menemukan beberapa contoh lain untuk Povray di Euler dalam
file-file berikut.


  <a href="Examples/Dandelin Spheres.html">Examples/Dandelin Spheres</a>  

  <a href="Examples/Donat Math.html">Examples/Donat Math</a>  

  <a href="Examples/Trefoil Knot.html">Examples/Trefoil Knot</a>  

  <a href="Examples/Optimization by Affine Scaling.html">Examples/Optimization by Affine Scaling</a>  

---

---

---

# Kalkulus dengan EMT

Materi Kalkulus mencakup di antaranya:


* 
Fungsi (fungsi aljabar, trigonometri, eksponensial, logaritma,
* komposisi fungsi)

* 
Limit Fungsi,

* 
Turunan Fungsi,

* 
Integral Tak Tentu,

* 
Integral Tentu dan Aplikasinya,

* 
Barisan dan Deret (kekonvergenan barisan dan deret).


EMT (bersama Maxima) dapat digunakan untuk melakukan semua perhitungan
di dalam kalkulus, baik secara numerik maupun analitik (eksak).


## Mendefinisikan Fungsi

Terdapat beberapa cara mendefinisikan fungsi pada EMT, yakni:


* 
Menggunakan format nama_fungsi := rumus fungsi (untuk fungsi
* numerik),

* 
Menggunakan format nama_fungsi &amp;= rumus fungsi (untuk fungsi
* simbolik, namun dapat dihitung secara numerik),

* 
Menggunakan format nama_fungsi &amp;&amp;= rumus fungsi (untuk fungsi
* simbolik murni, tidak dapat dihitung langsung),

* 
Fungsi sebagai program EMT.


Setiap format harus diawali dengan perintah function (bukan sebagai
ekspresi).


Berikut adalah adalah beberapa contoh cara mendefinisikan fungsi:


$$f(x)=2x^2+e^{\sin(x)}.$$\>function f(x) := 2\*x^2+exp(sin(x)) // fungsi numerik

\>f(0), f(1), f(pi)


    1
    4.31977682472
    20.7392088022

\>f(a) // tidak dapat dihitung nilainya


    Real 41 x 1 matrix
    
                1 
          1.21868 
          1.55948 
          2.01872 
          2.58957 
          3.26182 
          4.02223 
          4.85563 
          5.74672 
          6.68221 
          7.65308 
          8.65613 
          9.69456 
          10.7774 
          11.9179 
          13.1314 
          14.4331 
          15.8362 
          17.3508 
           18.984 
        ...

Silakan Anda plot kurva fungsi di atas!


Berikutnya kita definisikan fungsi:


$$g(x)=\frac{\sqrt{x^2-3x}}{x+1}.$$\>function g(x) := sqrt(x^2-3\*x)/(x+1)

\>g(3)


    0

\>g(0)


    0

\>g(1) // kompleks, tidak dapat dihitung oleh fungsi numerik


    Floating point error!
    Error in sqrt
    Try "trace errors" to inspect local variables after errors.
    g:
        useglobal; return sqrt(x^2-3*x)/(x+1) 
    Error in:
    g(1) // kompleks, tidak dapat dihitung oleh fungsi numerik ...
        ^

Silakan Anda plot kurva fungsi di atas!


\>f(g(5)) // komposisi fungsi


    2.20920171961

\>g(f(5))


    0.950898070639

\>function h(x) := f(g(x)) // definisi komposisi fungsi 

\>h(5) // sama dengan f(g(5))


    2.20920171961

Silakan Anda plot kurva fungsi komposisi fungsi f dan g:


$$h(x)=f(g(x))$$dan


$$u(x)=g(f(x))$$bersama-sama kurva fungsi f dan g dalam satu bidang koordinat.


\>f(0:10) // nilai-nilai f(0), f(1), f(2), ..., f(10)


    [1,  4.31978,  10.4826,  19.1516,  32.4692,  50.3833,  72.7562,
    99.929,  130.69,  163.51,  200.58]

\>fmap(0:10) // sama dengan f(0:10), berlaku untuk semua fungsi


    [1,  4.31978,  10.4826,  19.1516,  32.4692,  50.3833,  72.7562,
    99.929,  130.69,  163.51,  200.58]

\>gmap(200:210)


    [0.987534,  0.987596,  0.987657,  0.987718,  0.987778,  0.987837,
    0.987896,  0.987954,  0.988012,  0.988069,  0.988126]

Misalkan kita akan mendefinisikan fungsi


$$f(x) = \begin{cases} x^3 & x>0 \\ x^2 & x\le 0. \end{cases}$$Fungsi tersebut tidak dapat didefinisikan sebagai fungsi numerik
secara "inline" menggunakan format :=, melainkan didefinisikan sebagai
program. Perhatikan, kata "map" digunakan agar fungsi dapat menerima
vektor sebagai input, dan hasilnya berupa vektor. Jika tanpa kata
"map" fungsinya hanya dapat menerima input satu nilai.


\>function map f(x) ...


      if x>0 then return x^3
      else return x^2
      endif;
    endfunction
</pre>
\>f(1)


    1

\>f(-2)


    4

\>f(-5:5)


    [25,  16,  9,  4,  1,  0,  1,  8,  27,  64,  125]

\>aspect(1.5); plot2d("f(x)",-5,5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-552.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-552.png)

\>function f(x) &= 2\*E^x // fungsi simbolik


    
                                        x
                                     2 E
    

\>$f(a) // nilai fungsi secara simbolik


$$2\,e^{a}$$\>f(E) // nilai fungsi berupa bilangan desimal


    30.308524483

\>$f(E), $float(%)


$$30.30852448295852$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-555.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-555.png)

\>function g(x) &= 3\*x+1


    
                                   3 x + 1
    

\>function h(x) &= f(g(x)) // komposisi fungsi


    
                                     3 x + 1
                                  2 E
    

\>plot2d("h(x)",-1,1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-556.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-556.png)

# Latihan

Bukalah buku Kalkulus. Cari dan pilih beberapa (paling sedikit 5 fungsi berbeda
tipe/bentuk/jenis) fungsi dari buku tersebut, kemudian definisikan fungsi-fungsi tersebut dan
komposisinya di EMT pada baris-baris perintah berikut (jika perlu tambahkan lagi). Untuk setiap
fungsi, hitung beberapa nilainya, baik untuk satu nilai maupun vektor. Gambar grafik
fungsi-fungsi tersebut dan komposisi-komposisi 2 fungsi.


Juga, carilah fungsi beberapa (dua) variabel. Lakukan hal sama seperti di atas.


\>function f(x) := x^3-3\*x+5 // Purcell Jilid 1 hal 303

\>function g(x) := x/(x^2+4) // Purcell Jilid 1 hal 303

\>function h(x) := log(abs(x))

\>f(-10), g(-10), h(-10)


    -965
    -0.0961538461538
    2.30258509299

\>f(-2:5), g(-2:5)


    [3,  7,  5,  3,  7,  23,  57,  115]
    [-0.25,  -0.2,  0,  0.2,  0.25,  0.230769,  0.2,  0.172414]

\>f(g(-1)), g(f(-1)), g(h(-1)), h(f(-1))


    5.592
    0.132075471698
    0
    1.94591014906

\>plot2d("f(x)",style="."):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-557.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-557.png)

\>plot2d("g(x)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-558.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-558.png)

\>plot2d("h(x)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-559.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-559.png)

\>plot2d("f(x)","g(x)","h(x)"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-560.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-560.png)

\>function p(x) := (sin(x))^2\*cos(x)

\>p(-2:5)


    [-0.344079,  0.382574,  0,  0.382574,  -0.344079,  -0.0197156,
    -0.374374,  0.260838]

\>function q(x) := abs(g(x))+f(x)/5+p(x)

\>q(-10), plot2d("q(x)",-4,4):


    -193.152176899

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-561.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-561.png)

# Menghitung Limit

Perhitungan limit pada EMT dapat dilakukan dengan menggunakan fungsi
Maxima, yakni "limit". Fungsi "limit" dapat digunakan untuk menghitung
limit fungsi dalam bentuk ekspresi maupun fungsi yang sudah
didefinisikan sebelumnya. Nilai limit dapat dihitung pada sebarang
nilai atau pada tak hingga (-inf, minf, dan inf). Limit kiri dan limit
kanan juga dapat dihitung, dengan cara memberi opsi "plus" atau
"minus". Hasil limit dapat berupa nilai, "und" (tak definisi), "ind"
(tak tentu namun terbatas), "infinity" (kompleks tak hingga).


Perhatikan beberapa contoh berikut. Perhatikan cara menampilkan
perhitungan secara lengkap, tidak hanya menampilkan hasilnya saja.


\>$showev('limit(sqrt(x^2-3\*x)/(x+1),x,inf))


$$\lim_{x\rightarrow \infty }{\frac{\sqrt{x^2-3\,x}}{x+1}}=1$$\>$limit((x^3-13\*x^2+51\*x-63)/(x^3-4\*x^2-3\*x+18),x,3)


$$-\frac{4}{5}$$$$\lim_{x\rightarrow 3}{\frac{x^3-13\,x^2+51\,x-63}{x^3-4\,x^2-3\,x+  18}}=-\frac{4}{5}$$Fungsi tersebut diskontinu di titik x=3. Berikut adalah grafik
fungsinya.


\>aspect(1.5); plot2d("(x^3-13\*x^2+51\*x-63)/(x^3-4\*x^2-3\*x+18)",0,4); plot2d(3,-4/5,\>points,style="ow",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-565.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-565.png)

\>$limit(2\*x\*sin(x)/(1-cos(x)),x,0)


$$4$$$$2\,\left(\lim_{x\rightarrow 0}{\frac{x\,\sin x}{1-\cos x}}\right)=4$$Fungsi tersebut diskontinu di titik x=0. Berikut adalah grafik
fungsinya.


\>plot2d("2\*x\*sin(x)/(1-cos(x))",-pi,pi); plot2d(0,4,\>points,style="ow",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-568.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-568.png)

\>$limit(cot(7\*h)/cot(5\*h),h,0)


$$\frac{5}{7}$$$$\lim_{h\rightarrow 0}{\frac{\cot \left(7\,h\right)}{\cot \left(5\,h  \right)}}=\frac{5}{7}$$Fungsi tersebut juga diskontinu (karena tidak terdefinisi) di x=0.
Berikut adalah grafiknya.


\>plot2d("cot(7\*x)/cot(5\*x)",-0.001,0.001); plot2d(0,5/7,\>points,style="ow",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-571.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-571.png)

\>$showev('limit(((x/8)^(1/3)-1)/(x-8),x,8))


$$\lim_{x\rightarrow 8}{\frac{\frac{x^{\frac{1}{3}}}{2}-1}{x-8}}=  \frac{1}{24}$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(1/(2\*x-1),x,0))


$$\lim_{x\rightarrow 0}{\frac{1}{2\,x-1}}=-1$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit((x^2-3\*x-10)/(x-5),x,5))


$$\lim_{x\rightarrow 5}{\frac{x^2-3\,x-10}{x-5}}=7$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(sqrt(x^2+x)-x,x,inf))


$$\lim_{x\rightarrow \infty }{\sqrt{x^2+x}-x}=\frac{1}{2}$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(abs(x-1)/(x-1),x,1,minus))


$$\lim_{x\uparrow 1}{\frac{\left| x-1\right| }{x-1}}=-1$$Hitung limit di atas untuk x menuju 1 dari kanan.


Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(sin(x)/x,x,0))


$$\lim_{x\rightarrow 0}{\frac{\sin x}{x}}=1$$\>plot2d("sin(x)/x",-pi,pi); plot2d(0,1,\>points,style="ow",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-578.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-578.png)

\>$showev('limit(sin(x^3)/x,x,0))


$$\lim_{x\rightarrow 0}{\frac{\sin x^3}{x}}=0$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(log(x), x, minf))


$$\lim_{x\rightarrow  -\infty }{\log x}={\it infinity}$$\>$showev('limit((-2)^x,x, inf))


$$\lim_{x\rightarrow \infty }{\left(-2\right)^{x}}={\it infinity}$$\>$showev('limit(t-sqrt(2-t),t,2,minus))


$$\lim_{t\uparrow 2}{t-\sqrt{2-t}}=2$$\>$showev('limit(t-sqrt(2-t),t,2,plus))


$$\lim_{t\downarrow 2}{t-\sqrt{2-t}}=2$$\>$showev('limit(t-sqrt(2-t),t,5,plus)) // Perhatikan hasilnya


$$\lim_{t\downarrow 5}{t-\sqrt{2-t}}=5-\sqrt{3}\,i$$\>plot2d("x-sqrt(2-x)",0,2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-585.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-585.png)

\>$showev('limit((x^2-9)/(2\*x^2-5\*x-3),x,3))


$$\lim_{x\rightarrow 3}{\frac{x^2-9}{2\,x^2-5\,x-3}}=\frac{6}{7}$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit((1-cos(x))/x,x,0))


$$\lim_{x\rightarrow 0}{\frac{1-\cos x}{x}}=0$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit((x^2+abs(x))/(x^2-abs(x)),x,0))


$$\lim_{x\rightarrow 0}{\frac{\left| x\right| +x^2}{x^2-\left| x  \right| }}=-1$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit((1+1/x)^x,x,inf))


$$\lim_{x\rightarrow \infty }{\left(\frac{1}{x}+1\right)^{x}}=e$$\>plot2d("(1+1/x)^x",0,1000):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-590.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-590.png)

\>$showev('limit((1+k/x)^x,x,inf))


$$\lim_{x\rightarrow \infty }{\left(\frac{k}{x}+1\right)^{x}}=e^{k}$$\>$showev('limit((1+x)^(1/x),x,0))


$$\lim_{x\rightarrow 0}{\left(x+1\right)^{\frac{1}{x}}}=e$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit((x/(x+k))^x,x,inf))


$$\lim_{x\rightarrow \infty }{\left(\frac{x}{x+k}\right)^{x}}=e^ {- k   }$$\>$showev('limit((E^x-E^2)/(x-2),x,2))


$$\lim_{x\rightarrow 2}{\frac{e^{x}-e^2}{x-2}}=e^2$$Tunjukkan limit tersebut dengan grafik, seperti contoh-contoh sebelumnya.


\>$showev('limit(sin(1/x),x,0))


$$\lim_{x\rightarrow 0}{\sin \left(\frac{1}{x}\right)}={\it ind}$$\>$showev('limit(sin(1/x),x,inf))


$$\lim_{x\rightarrow \infty }{\sin \left(\frac{1}{x}\right)}=0$$\>plot2d("sin(1/x)",-0.001,0.001):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-597.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-597.png)

# Latihan

Bukalah buku Kalkulus. Cari dan pilih beberapa (paling sedikit 5 fungsi berbeda
tipe/bentuk/jenis) fungsi dari buku tersebut, kemudian definisikan di EMT pada
baris-baris perintah berikut (jika perlu tambahkan lagi). Untuk setiap fungsi, hitung
nilai limit fungsi tersebut di beberapa nilai dan di tak hingga. Gambar grafik fungsi
tersebut untuk mengkonfirmasi nilai-nilai limit tersebut.


\>$showev('limit(x/(1+x^2),x,inf)), $showev('limit(x/(1+x^2),x,5,plus)), ...  
\>   $showev('limit(x/(1+x^2),x,-100)), plot2d("x/(1+x^2)"): //purcell jilid 1 hal 291


$$\lim_{x\rightarrow -100}{\frac{x}{x^2+1}}=-\frac{100}{10001}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-599.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-599.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-600.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-600.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-601.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-601.png)

\>$showev('limit((x+1)/(x^2-5\*x+6),x,minf)), $showev('limit((x+1)/(x^2-5\*x+6),x,3)), ...  
\>   $showev('limit((x+1)/(x^2-5\*x+6),x,3,minus)), plot2d("(x+1)/(x^2-5\*x+6)",-2,5): ...  
\>   //purcell jilid 1 hal 293


$$\lim_{x\uparrow 3}{\frac{x+1}{x^2-5\,x+6}}= -\infty $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-603.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-603.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-604.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-604.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-605.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-605.png)

\>$showev('limit(abs(x)/x,x,inf)), $showev('limit(abs(x)/x,x,0)),  ...  
\>   $showev('limit(abs(x)/x,x,0,plus)), $showev('limit(abs(x)/x,x,0,minus)), ...  
\>   plot2d("abs(x)/x"): //purcell jilid 1 hal 296


$$\lim_{x\uparrow 0}{\frac{\left| x\right| }{x}}=-1$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-607.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-607.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-608.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-608.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-609.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-609.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-610.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-610.png)

\>$showev('limit(x\*sin(1/x),x,minf)), $showev('limit(x\*sin(1/x),x,0.5)), ...  
\>   $showev('limit(x\*sin(1/x),x,0.5,plus)), $showev('limit(x\*sin(1/x),x,0.5,minus)), ...  
\>   plot2d("x\*sin(1/x)"): //purcell jilid 1 hal 297


$$\lim_{x\uparrow 0.5}{\sin \left(\frac{1}{x}\right)\,x}=  0.4546487134128409$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-612.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-612.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-613.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-613.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-614.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-614.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-615.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-615.png)

\>$showev('limit((1+sqrt(x))^(1/sqrt(x)),x,inf)),  ...  
\>   $showev('limit((1+sqrt(x))^(1/sqrt(x)),x,0)),  ...  
\>   $showev('limit((1+sqrt(x))^(1/sqrt(x)),x,3,plus)),  ...  
\>   $showev('limit((1+sqrt(x))^(1/sqrt(x)),x,3,minus)), ...  
\>   plot2d("(1+sqrt(x))^(1/sqrt(x))",-10,10): //purcell jilid 1 hal 297


$$\lim_{x\uparrow 3}{\left(\sqrt{x}+1\right)^{\frac{1}{\sqrt{x}}}}=e  ^{\frac{\log \left(\sqrt{3}+1\right)}{\sqrt{3}}}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-617.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-617.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-618.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-618.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-619.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-619.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-620.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-620.png)

# Turunan Fungsi

Definisi turunan:


$$f'(x) = \lim_{h\to 0} \frac{f(x+h)-f(x)}{h}$$Berikut adalah contoh-contoh menentukan turunan fungsi dengan
menggunakan definisi turunan (limit).


\>$showev('limit(((x+h)^2-x^2)/h,h,0)) // turunan x^2


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^2-x^2}{h}}=2\,x$$\>p &= expand((x+h)^2-x^2)|simplify; $p //pembilang dijabarkan dan disederhanakan


$$2\,h\,x+h^2$$\>q &=ratsimp(p/h); $q // ekspresi yang akan dihitung limitnya disederhanakan


$$2\,x+h$$\>$limit(q,h,0) // nilai limit sebagai turunan


$$2\,x$$\>$showev('limit(((x+h)^n-x^n)/h,h,0)) // turunan x^n


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{n}-x^{n}}{h}}=n\,x^{n  -1}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil limit tersebut
benar, sehingga benar turunan fungsinya benar.  Tulis penjelasan Anda di komentar
ini.


Sebagai petunjuk, ekspansikan (x+h)^n dengan menggunakan teorema binomial.


\>$showev('limit((sin(x+h)-sin(x))/h,h,0)) // turunan sin(x)


$$\lim_{h\rightarrow 0}{\frac{\sin \left(x+h\right)-\sin x}{h}}=\cos   x$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil limit tersebut


benar, sehingga benar turunan fungsinya benar.  Tulis penjelasan Anda di komentar
ini.


Sebagai petunjuk, ekspansikan sin(x+h) dengan menggunakan rumus jumlah dua sudut.


\>$showev('limit((log(x+h)-log(x))/h,h,0)) // turunan log(x)


$$\lim_{h\rightarrow 0}{\frac{\log \left(x+h\right)-\log x}{h}}=  \frac{1}{x}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil limit tersebut


benar, sehingga benar turunan fungsinya benar.  Tulis penjelasan Anda di komentar
ini.


Sebagai petunjuk, gunakan sifat-sifat logaritma dan hasil limit pada bagian
sebelumnya di atas.


\>$showev('limit((1/(x+h)-1/x)/h,h,0)) // turunan 1/x


$$\lim_{h\rightarrow 0}{\frac{\frac{1}{x+h}-\frac{1}{x}}{h}}=-\frac{1  }{x^2}$$\>$showev('limit((E^(x+h)-E^x)/h,h,0)) // turunan f(x)=e^x


    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Answering "Is x an integer?" with "integer"
    Maxima is asking
    Acceptable answers are: yes, y, Y, no, n, N, unknown, uk
    Is x an integer?
    
    Use assume!
    Error in:
     $showev('limit((E^(x+h)-E^x)/h,h,0)) // turunan f(x)=e^x ...
                                         ^

Maxima bermasalah dengan limit:


$$\lim_{h\to 0}\frac{e^{x+h}-e^x}{h}.$$Oleh karena itu diperlukan trik khusus agar hasilnya benar.


\>$showev('limit((E^h-1)/h,h,0))


$$\lim_{h\rightarrow 0}{\frac{e^{h}-1}{h}}=1$$\>$showev('factor(E^(x+h)-E^x))


$${\it factor}\left(e^{x+h}-e^{x}\right)=\left(e^{h}-1\right)\,e^{x}$$\>$showev('limit(factor((E^(x+h)-E^x)/h),h,0)) // turunan f(x)=e^x


$$\left(\lim_{h\rightarrow 0}{\frac{e^{h}-1}{h}}\right)\,e^{x}=e^{x}$$\>function f(x) &= x^x


    
                                       x
                                      x
    

\>$showev('limit(f(x),x,0))


$$\lim_{x\rightarrow 0}{x^{x}}=1$$Silakan Anda gambar kurva


$$y=x^x.$$\>$showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=x^x


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{x+h}-x^{x}}{h}}=  {\it infinity}$$Di sini Maxima juga bermasalah terkait limit:


$$\lim_{h\to 0} \frac{(x+h)^{x+h}-x^x}{h}.$$Dalam hal ini diperlukan asumsi nilai x.


\>&assume(x\>0); $showev('limit((f(x+h)-f(x))/h,h,0)) // turunan f(x)=x^x


$$\lim_{h\rightarrow 0}{\frac{\left(x+h\right)^{x+h}-x^{x}}{h}}=x^{x}  \,\left(\log x+1\right)$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil
limit tersebut benar, sehingga benar turunan fungsinya benar. Tulis
penjelasan Anda di komentar ini.


\>&forget(x\>0) // jangan lupa, lupakan asumsi untuk kembali ke semula


    
                                   [x &gt; 0]
    

\>&forget(x<0)


    
                                   [x &lt; 0]
    

\>&facts()


    
            [kind(sinh, one_to_one), kind(log, one_to_one), 
                            kind(tanh, one_to_one), kind(log, increasing)]
    

\>$showev('limit((asin(x+h)-asin(x))/h,h,0)) // turunan arcsin(x)


$$\lim_{h\rightarrow 0}{\frac{\arcsin \left(x+h\right)-\arcsin x}{h}}=  \frac{1}{\sqrt{1-x^2}}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil
limit tersebut benar, sehingga benar turunan fungsinya benar. Tulis
penjelasan Anda di komentar ini.


\>$showev('limit((tan(x+h)-tan(x))/h,h,0)) // turunan tan(x)


$$\lim_{h\rightarrow 0}{\frac{\tan \left(x+h\right)-\tan x}{h}}=  \frac{1}{\cos ^2x}$$Mengapa hasilnya seperti itu? Tuliskan atau tunjukkan bahwa hasil
limit tersebut benar, sehingga benar turunan fungsinya benar. Tulis
penjelasan Anda di komentar ini.


\>function f(x) &= sinh(x) // definisikan f(x)=sinh(x)


    
                                   sinh(x)
    

\>function df(x) &= limit((f(x+h)-f(x))/h,h,0); $df(x) // df(x) = f'(x)


$$\frac{e^ {- x }\,\left(e^{2\,x}+1\right)}{2}$$Hasilnya adalah cosh(x), karena


$$\frac{e^x+e^{-x}}{2}=\cosh(x).$$\>plot2d(["f(x)","df(x)"],-pi,pi,color=[blue,red]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-643.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-643.png)

\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>diff(f,3), diffc(f,3)


    1198.32948904
    1198.72863721

Apakah perbedaan diff dan diffc?


\>$showev('diff(f(x),x))


$$\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right)=30\,x^4\,\cos \left(3  \,x^5+7\right)\,\sin \left(3\,x^5+7\right)$$\>$% with x=3


$${\it \%at}\left(\frac{d}{d\,x}\,\sin ^2\left(3\,x^5+7\right) , x=3  \right)=2430\,\cos 736\,\sin 736$$\>$float(%)


$${\it \%at}\left(\frac{d^{1.0}}{d\,x^{1.0}}\,\sin ^2\left(3.0\,x^5+  7.0\right) , x=3.0\right)=1198.728637211748$$\>plot2d(f,0,3.1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-647.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-647.png)

\>function f(x) &=5\*cos(2\*x)-2\*x\*sin(2\*x) // mendifinisikan fungsi f


    
                          5 cos(2 x) - 2 x sin(2 x)
    

\>function df(x) &=diff(f(x),x) // fd(x) = f'(x)


    
                         - 12 sin(2 x) - 4 x cos(2 x)
    

\>$'f(1)=f(1), $float(f(1)), $'f(2)=f(2), $float(f(2)) // nilai f(1) dan f(2)


$$-0.2410081230863468$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-649.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-649.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-650.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-650.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-651.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-651.png)

\>xp=solve("df(x)",1,2,0) // solusi f'(x)=0 pada interval [1, 2]


    1.35822987384

\>df(xp), f(xp) // cek bahwa f'(xp)=0 dan nilai ekstrim di titik tersebut


    0
    -5.67530133759

\>plot2d(["f(x)","df(x)"],0,2\*pi,color=[blue,red]): //grafik fungsi dan turunannya


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-652.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-652.png)

Perhatikan titik-titik "puncak" grafik y=f(x) dan nilai turunan pada
saat grafik fungsinya mencapai titik "puncak" tersebut.


# Latihan

Bukalah buku Kalkulus. Cari dan pilih beberapa (paling sedikit 5
fungsi berbeda tipe/bentuk/jenis) fungsi dari buku tersebut, kemudian
definisikan di EMT pada baris-baris perintah berikut (jika perlu
tambahkan lagi). Untuk setiap fungsi, tentukan turunannya dengan
menggunakan definisi turunan (limit), menggunakan perintah diff, dan
secara manual (langkah demi langkah yang dihitung dengan Maxima)
seperti contoh-contoh di atas. Gambar grafik fungsi asli dan fungsi
turunannya pada sumbu koordinat yang sama.


\>function f(x) &= 3\*x-x^2; $'f(x)=f(x) //purcell jilid 1 hal 315


$$f\left(x\right)=3\,x-x^2$$\>$showev('limit(f(x),x,0)), $showev('limit((f(x+h)-f(x))/h,h,0)), ...  
\>   function df(x) &= diff(f(x),x); $'df(x)=df(x), plot2d(["f(x)","df(x)"],-1,4.5,color=[red,yellow]):


$${\it df}\left(x\right)=3-2\,x$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-655.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-655.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-656.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-656.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-657.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-657.png)

\>function g(x) &= (3\*x^2+2\*x+sin(x))/x; $'g(x)=g(x) //purcell jilid 1 hal 314


$$g\left(x\right)=\frac{\sin x+3\,x^2+2\,x}{x}$$\>$showev('limit(g(x),x,0)), $showev('limit((g(x+h)-g(x))/h,h,0)), ...  
\>   function dg(x) &= diff(g(x),x); $'dg(x)=dg(x), ...  
\>  
$${\it dg}\left(x\right)=\frac{\cos x+6\,x+2}{x}-\frac{\sin x+3\,x^2+  2\,x}{x^2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-660.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-660.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-661.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-661.png)

\>plot2d(["g(x)","dg(x)"],-5,5,color=[red,yellow]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-662.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-662.png)

\>function h(x) &= cos(x)-sin(x); $'h(x)=h(x), ...  
\>  
$$h\left(x\right)=\cos x-\sin x$$\>$showev('limit(h(x),x,0)), $showev('limit((h(x+h)-h(x))/h,h,0)), ...  
\>   function dh(x) &= diff(h(x),x); $'dh(x)=dh(x), ...  
\>  
$${\it dh}\left(x\right)=-\sin x-\cos x$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-665.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-665.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-666.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-666.png)

\>plot2d(["h(x)","dh(x)"],color=[red,yellow]): //purcell jilid 1 hal 316


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-667.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-667.png)

\>function p(x) &= atan(1/x); $'p(x)=p(x), ...  
\>  
$$p\left(x\right)=\arctan \left(\frac{1}{x}\right)$$\>$showev('limit(p(x),x,0)), $showev('limit((p(x+h)-p(x))/h,h,0)), ...  
\>   function dp(x) &= diff(p(x),x); $'dp(x)=dp(x), ...  
\>  
$${\it dp}\left(x\right)=-\frac{1}{\left(\frac{1}{x^2}+1\right)\,x^2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-670.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-670.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-671.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-671.png)

\>plot2d(["p(x)","dp(x)"],color=[red,yellow]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-672.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-672.png)

\>function q(x) &= log(x+1); $'q(x)=q(x), ...  
\>  
$$q\left(x\right)=\log \left(x+1\right)$$\>$showev('limit(q(x),x,0)), $showev('limit((q(x+h)-q(x))/h,h,0)), ...  
\>   function dq(x) &= diff(q(x),x); $'dq(x)=dq(x), ...  
\>  
$${\it dq}\left(x\right)=\frac{1}{x+1}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-675.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-675.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-676.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-676.png)

\>plot2d(["q(x)","dq(x)"],color=[red,yellow]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-677.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-677.png)

# Integral

EMT dapat digunakan untuk menghitung integral, baik integral tak tentu
maupun integral tentu. Untuk integral tak tentu (simbolik) sudah tentu
EMT menggunakan Maxima, sedangkan untuk perhitungan integral tentu EMT
sudah menyediakan beberapa fungsi yang mengimplementasikan algoritma
kuadratur (perhitungan integral tentu menggunakan metode numerik).


Pada notebook ini akan ditunjukkan perhitungan integral tentu dengan
menggunakan Teorema Dasar Kalkulus:


$$\int_a^b f(x)\ dx = F(b)-F(a), \quad \text{ dengan  } F'(x) = f(x).$$Fungsi untuk menentukan integral adalah integrate. Fungsi ini dapat
digunakan untuk menentukan, baik integral tentu maupun tak tentu (jika
fungsinya memiliki antiderivatif). Untuk perhitungan integral tentu
fungsi integrate menggunakan metode numerik (kecuali fungsinya tidak
integrabel, kita tidak akan menggunakan metode ini).


\>$showev('integrate(x^n,x))


    Answering "Is n equal to -1?" with "no"

$$\int {x^{n}}{\;dx}=\frac{x^{n+1}}{n+1}$$\>$showev('integrate(1/(1+x),x))


$$\int {\frac{1}{x+1}}{\;dx}=\log \left(x+1\right)$$\>$showev('integrate(1/(1+x^2),x))


$$\int {\frac{1}{x^2+1}}{\;dx}=\arctan x$$\>$showev('integrate(1/sqrt(1-x^2),x))


$$\int {\frac{1}{\sqrt{1-x^2}}}{\;dx}=\arcsin x$$\>$showev('integrate(sin(x),x,0,pi))


$$\int_{0}^{\pi}{\sin x\;dx}=2$$\>plot2d("sin(x)",0,2\*pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-684.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-684.png)

\>$showev('integrate(sin(x),x,a,b))


$$\int_{a}^{b}{\sin x\;dx}=\cos a-\cos b$$\>$showev('integrate(x^n,x,a,b))


    Answering "Is n positive, negative or zero?" with "positive"

$$\int_{a}^{b}{x^{n}\;dx}=\frac{b^{n+1}}{n+1}-\frac{a^{n+1}}{n+1}$$\>$showev('integrate(x^2\*sqrt(2\*x+1),x))


$$\int {x^2\,\sqrt{2\,x+1}}{\;dx}=\frac{\left(2\,x+1\right)^{\frac{7  }{2}}}{28}-\frac{\left(2\,x+1\right)^{\frac{5}{2}}}{10}+\frac{\left(  2\,x+1\right)^{\frac{3}{2}}}{12}$$\>$showev('integrate(x^2\*sqrt(2\*x+1),x,0,2))


$$\int_{0}^{2}{x^2\,\sqrt{2\,x+1}\;dx}=\frac{2\,5^{\frac{5}{2}}}{21}-  \frac{2}{105}$$\>$ratsimp(%)


$$\int_{0}^{2}{x^2\,\sqrt{2\,x+1}\;dx}=\frac{2\,5^{\frac{7}{2}}-2}{  105}$$\>$showev('integrate((sin(sqrt(x)+a)\*E^sqrt(x))/sqrt(x),x,0,pi^2))


$$\int_{0}^{\pi^2}{\frac{\sin \left(\sqrt{x}+a\right)\,e^{\sqrt{x}}}{  \sqrt{x}}\;dx}=\left(-e^{\pi}-1\right)\,\sin a+\left(e^{\pi}+1  \right)\,\cos a$$\>$factor(%)


$$\int_{0}^{\pi^2}{\frac{\sin \left(\sqrt{x}+a\right)\,e^{\sqrt{x}}}{  \sqrt{x}}\;dx}=\left(-e^{\pi}-1\right)\,\left(\sin a-\cos a\right)$$\>function map f(x) &= E^(-x^2)


    
                                        2
                                     - x
                                    E
    

\>$showev('integrate(f(x),x))


$$\int {e^ {- x^2 }}{\;dx}=\frac{\sqrt{\pi}\,\mathrm{erf}\left(x  \right)}{2}$$Fungsi f tidak memiliki antiturunan, integralnya masih memuat integral
lain.


$$erf(x) = \int \frac{e^{-x^2}}{\sqrt{\pi}} \ dx.$$Kita tidak dapat menggunakan teorema Dasar kalkulus untuk menghitung
integral tentu fungsi tersebut jika semua batasnya berhingga. Dalam
hal ini dapat digunakan metode numerik (rumus kuadratur).


Misalkan kita akan menghitung:


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}$$\>x=0:0.1:pi-0.1; plot2d(x,f(x+0.1),\>bar); plot2d("f(x)",0,pi,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-695.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-695.png)

Integral tentu


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}$$dapat dihampiri dengan jumlah luas persegi-persegi panjang di bawah
kurva y=f(x) tersebut. Langkah-langkahnya adalah sebagai berikut.


\>t &= makelist(a,a,0,pi-0.1,0.1); // t sebagai list untuk menyimpan nilai-nilai x

\>fx &= makelist(f(t[i]+0.1),i,1,length(t)); // simpan nilai-nilai f(x)

\>// jangan menggunakan x sebagai list, kecuali Anda pakar Maxima!


Hasilnya adalah:


$$\int_{0}^{\pi}{e^ {- x^2 }\;dx}=0.8362196102528469$$Jumlah tersebut diperoleh dari hasil kali lebar sub-subinterval (=0.1)
dan jumlah nilai-nilai f(x) untuk x = 0.1, 0.2, 0.3, ..., 3.2.


\>0.1\*sum(f(x+0.1)) // cek langsung dengan perhitungan numerik EMT


    0.836219610253

Untuk mendapatkan nilai integral tentu yang mendekati nilai
sebenarnya, lebar sub-intervalnya dapat diperkecil lagi, sehingga
daerah di bawah kurva tertutup semuanya, misalnya dapat digunakan
lebar subinterval 0.001. (Silakan dicoba!)


Meskipun Maxima tidak dapat menghitung integral tentu fungsi tersebut
untuk batas-batas yang berhingga, namun integral tersebut dapat
dihitung secara eksak jika batas-batasnya tak hingga. Ini adalah salah
satu keajaiban di dalam matematika, yang terbatas tidak dapat dihitung
secara eksak, namun yang tak hingga malah dapat dihitung secara eksak.


\>$showev('integrate(f(x),x,0,inf))


$$\int_{0}^{\infty }{e^ {- x^2 }\;dx}=\frac{\sqrt{\pi}}{2}$$Tunjukkan kebenaran hasil di atas!


Berikut adalah contoh lain fungsi yang tidak memiliki antiderivatif, sehingga integral tentunya hanya
dapat dihitung dengan metode numerik.


\>function f(x) &= x^x


    
                                       x
                                      x
    

\>$showev('integrate(f(x),x,0,1))


$$\int_{0}^{1}{x^{x}\;dx}=\int_{0}^{1}{x^{x}\;dx}$$\>x=0:0.1:1-0.01; plot2d(x,f(x+0.01),\>bar); plot2d("f(x)",0,1,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-700.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-700.png)

Maxima gagal menghitung integral tentu tersebut secara langsung
menggunakan perintah integrate. Berikut kita lakukan seperti contoh
sebelumnya untuk mendapat hasil atau pendekatan nilai integral tentu
tersebut.


\>t &= makelist(a,a,0,1-0.01,0.01);

\>fx &= makelist(f(t[i]+0.01),i,1,length(t));


$$\int_{0}^{1}{x^{x}\;dx}=0.7834935879025506$$Apakah hasil tersebut cukup baik? perhatikan gambarnya.


\>function f(x) &= sin(3\*x^5+7)^2


    
                                   2    5
                                sin (3 x  + 7)
    

\>integrate(f,0,1)


    0.542581176074

\>&showev('integrate(f(x),x,0,1))


    
              1
             /
             [     2    5                                 1
             I  sin (3 x  + 7) dx = (((I gamma_incomplete(-, 6 I)
             ]                                            5
             /
              0
                          1             2
     - I gamma_incomplete(-, - 6 I)) sin (7)
                          5
                             1                            1
     + (- 2 gamma_incomplete(-, 6 I) - 2 gamma_incomplete(-, - 6 I)
                             5                            5
               1                                       1
     + 4 gamma(-)) cos(7) sin(7) + (I gamma_incomplete(-, - 6 I)
               5                                       5
                          1           2         pi        1/5    2
     - I gamma_incomplete(-, 6 I)) cos (7)) sin(--) + 10 6    sin (7)
                          5                     10
           1/5    2          1/5
     + 10 6    cos (7))/(20 6   )
    

\>&float(%)


    
              1.0
             /
             [       2      5
             I    sin (3.0 x  + 7.0) dx = 
             ]
             /
              0.0
    0.03494135593857896 (0.3090169943749474
     (0.4316313908960832 (I gamma__incomplete(0.2, 6.0 I)
     - 1.0 I gamma__incomplete(0.2, - 6.0 I))
     + 0.5683686091039167 (I gamma__incomplete(0.2, - 6.0 I)
     - 1.0 I gamma__incomplete(0.2, 6.0 I))
     + 0.4953036778474351 (- 2.0 gamma__incomplete(0.2, 6.0 I)
     - 2.0 gamma__incomplete(0.2, - 6.0 I) + 18.36337484799522))
     + 14.30969081105255)
    

\>$showev('integrate(x\*exp(-x),x,0,1)) // Integral tentu (eksak)


$$\int_{0}^{1}{x\,e^ {- x }\;dx}=1-2\,e^ {- 1 }$$# Aplikasi Integral Tentu

\>plot2d("x^3-x",-0.1,1.1); plot2d("-x^2",\>add);  ...  
\>   b=solve("x^3-x+x^2",0.5); x=linspace(0,b,200); xi=flipx(x); ...  
\>   plot2d(x|xi,x^3-x|-xi^2,\>filled,style="|",fillcolor=1,\>add): // Plot daerah antara 2 kurva


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-703.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-703.png)

\>a=solve("x^3-x+x^2",0), b=solve("x^3-x+x^2",1) // absis titik-titik potong kedua kurva


    0
    0.61803398875

\>integrate("(-x^2)-(x^3-x)",a,b) // luas daerah yang diarsir


    0.0758191713542

Hasil tersebut akan kita bandingkan dengan perhitungan secara analitik.


\>a &= solve((-x^2)-(x^3-x),x); $a // menentukan absis titik potong kedua kurva secara eksak


$$\left[ x=\frac{-\sqrt{5}-1}{2} , x=\frac{\sqrt{5}-1}{2} , x=0   \right] $$\>$showev('integrate(-x^2-x^3+x,x,0,(sqrt(5)-1)/2)) // Nilai integral secara eksak


$$\int_{0}^{\frac{\sqrt{5}-1}{2}}{-x^3-x^2+x\;dx}=\frac{13-5^{\frac{3  }{2}}}{24}$$\>$float(%)


$$\int_{0.0}^{0.6180339887498949}{-1.0\,x^3-1.0\,x^2+x\;dx}=  0.07581917135421037$$## Panjang Kurva

Hitunglah panjang kurva berikut ini dan luas daerah di dalam kurva
tersebut.


$$\gamma(t) = (r(t) \cos(t), r(t) \sin(t))$$dengan


$$r(t) = 1 + \dfrac{\sin(3t)}{2},\quad 0\le t\le 2\pi.$$\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t); ...  
\>   plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5): // Kita gambar kurvanya terlebih dahulu


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-709.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-709.png)

\>function r(t) &= 1+sin(3\*t)/2; $'r(t)=r(t)


$$r\left(t\right)=\frac{\sin \left(3\,t\right)}{2}+1$$\>function fx(t) &= r(t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(t\right)=\cos t\,\left(\frac{\sin \left(3\,t\right)}{  2}+1\right)$$\>function fy(t) &= r(t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(t\right)=\sin t\,\left(\frac{\sin \left(3\,t\right)}{  2}+1\right)$$\>function ds(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'ds(t)=ds(t)


$${\it ds}\left(t\right)=\frac{\sqrt{4\,\cos \left(6\,t\right)+4\,  \sin \left(3\,t\right)+9}}{2}$$\>$integrate(ds(x),x,0,2\*pi) //panjang (keliling) kurva


$$\frac{\int_{0}^{2\,\pi}{\sqrt{4\,\cos \left(6\,x\right)+4\,\sin   \left(3\,x\right)+9}\;dx}}{2}$$Maxima gagal melakukan perhitungan eksak integral tersebut.


Berikut kita hitung integralnya secara umerik dengan perintah EMT.


\>integrate("ds(x)",0,2\*pi)


    9.0749467823

Spiral Logaritmik


$$x=e^{ax}\cos x,\ y=e^{ax}\sin x.$$\>a=0.1; plot2d("exp(a\*x)\*cos(x)","exp(a\*x)\*sin(x)",r=2,xmin=0,xmax=2\*pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-716.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-716.png)

\>&kill(a) // hapus expresi a


    
                                     done
    

\>function fx(t) &= exp(a\*t)\*cos(t); $'fx(t)=fx(t)


$${\it fx}\left(t\right)=e^{a\,t}\,\cos t$$\>function fy(t) &= exp(a\*t)\*sin(t); $'fy(t)=fy(t)


$${\it fy}\left(t\right)=e^{a\,t}\,\sin t$$\>function df(t) &= trigreduce(radcan(sqrt(diff(fx(t),t)^2+diff(fy(t),t)^2))); $'df(t)=df(t)


$${\it df}\left(t\right)=\sqrt{a^2+1}\,e^{a\,t}$$\>S &=integrate(df(t),t,0,2\*%pi); $S // panjang kurva (spiral)


$$\sqrt{a^2+1}\,\left(\frac{e^{2\,\pi\,a}}{a}-\frac{1}{a}\right)$$\>S(a=0.1) // Panjang kurva untuk a=0.1


    8.78817491636

Soal:


Tunjukkan bahwa keliling lingkaran dengan jari-jari r adalah K=2.pi.r.


Berikut adalah contoh menghitung panjang parabola.


\>plot2d("x^2",xmin=-1,xmax=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-721.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-721.png)

\>$showev('integrate(sqrt(1+diff(x^2,x)^2),x,-1,1))


$$\int_{-1}^{1}{\sqrt{4\,x^2+1}\;dx}=\frac{{\rm asinh}\; 2+2\,\sqrt{5  }}{2}$$\>$float(%)


$$\int_{-1.0}^{1.0}{\sqrt{4.0\,x^2+1.0}\;dx}=2.957885715089195$$\>x=-1:0.2:1; y=x^2; plot2d(x,y);  ...  
\>     plot2d(x,y,points=1,style="o#",add=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-724.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-724.png)

Panjang tersebut dapat dihampiri dengan menggunakan jumlah panjang
ruas-ruas garis yang menghubungkan titik-titik pada parabola tersebut.


\>i=1:cols(x)-1; sum(sqrt((x[i+1]-x[i])^2+(y[i+1]-y[i])^2))


    2.95191957027

Hasilnya mendekati panjang yang dihitung secara eksak. Untuk
mendapatkan hampiran yang cukup akurat, jarak antar titik dapat
diperkecil, misalnya 0.1, 0.05, 0.01, dan seterusnya. Cobalah Anda
ulangi perhitungannya dengan nilai-nilai tersebut.


## Koordinat Kartesius

Berikut diberikan contoh perhitungan panjang kurva menggunakan
koordinat Kartesius. Kita akan hitung panjang kurva dengan persamaan
implisit:


$$x^3+y^3-3xy=0.$$\>z &= x^3+y^3-3\*x\*y; $z


$$y^3-3\,x\,y+x^3$$\>plot2d(z,r=2,level=0,n=100):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-727.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-727.png)

Kita tertarik pada kurva di kuadran pertama.


\>plot2d(z,a=0,b=2,c=0,d=2,level=[-10;0],n=100,contourwidth=3,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-728.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-728.png)

Kita selesaikan persamaannya untuk x.


\>$z with y=l\*x, sol &= solve(%,x); $sol


$$\left[ x=\frac{3\,l}{l^3+1} , x=0 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-730.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-730.png)

Kita gunakan solusi tersebut untuk mendefinisikan fungsi dengan Maxima.


\>function f(l) &= rhs(sol[1]); $'f(l)=f(l)


$$f\left(l\right)=\frac{3\,l}{l^3+1}$$Fungsi tersebut juga dapat digunaka untuk menggambar kurvanya. Ingat,
bahwa fungsi tersebut adalah nilai x dan nilai y=l*x, yakni x=f(l) dan
y=l*f(l).


\>plot2d(&f(x),&x\*f(x),xmin=-0.5,xmax=2,a=0,b=2,c=0,d=2,r=1.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-732.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-732.png)

Elemen panjang kurva adalah:


$$ds=\sqrt{f'(l)^2+(lf'(l)+f(l))^2}.$$\>function ds(l) &= ratsimp(sqrt(diff(f(l),l)^2+diff(l\*f(l),l)^2)); $'ds(l)=ds(l)


$${\it ds}\left(l\right)=\frac{\sqrt{9\,l^8+36\,l^6-36\,l^5-36\,l^3+  36\,l^2+9}}{\sqrt{l^{12}+4\,l^9+6\,l^6+4\,l^3+1}}$$\>$integrate(ds(l),l,0,1)


$$\int_{0}^{1}{\frac{\sqrt{9\,l^8+36\,l^6-36\,l^5-36\,l^3+36\,l^2+9}  }{\sqrt{l^{12}+4\,l^9+6\,l^6+4\,l^3+1}}\;dl}$$Integral tersebut tidak dapat dihitung secara eksak menggunakan
Maxima. Kita hitung integral etrsebut secara numerik dengan Euler.
Karena kurva simetris, kita hitung untuk nilai variabel integrasi dari
0 sampai 1, kemudian hasilnya dikalikan 2.


\>2\*integrate("ds(x)",0,1)


    4.91748872168

\>2\*romberg(&ds(x),0,1)// perintah Euler lain untuk menghitung nilai hampiran integral yang sama


    4.91748872168

Perhitungan di datas dapat dilakukan untuk sebarang fungsi x dan y
dengan mendefinisikan fungsi EMT, misalnya kita beri nama
panjangkurva. Fungsi ini selalu memanggil Maxima untuk menurunkan
fungsi yang diberikan.


\>function panjangkurva(fx,fy,a,b) ...


    ds=mxm("sqrt(diff(@fx,x)^2+diff(@fy,x)^2)");
    return romberg(ds,a,b);
    endfunction
</pre>
\>panjangkurva("x","x^2",-1,1) // cek untuk menghitung panjang kurva parabola sebelumnya


    2.95788571509

Bandingkan dengan nilai eksak di atas.


\>2\*panjangkurva(mxm("f(x)"),mxm("x\*f(x)"),0,1) // cek contoh terakhir, bandingkan hasilnya!


    4.91748872168

Kita hitung panjang spiral Archimides berikut ini dengan fungsi tersebut.


\>plot2d("x\*cos(x)","x\*sin(x)",xmin=0,xmax=2\*pi,square=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-736.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-736.png)

\>panjangkurva("x\*cos(x)","x\*sin(x)",0,2\*pi)


    21.2562941482

Berikut kita definisikan fungsi yang sama namun dengan Maxima, untuk perhitungan eksak.


\>&kill(ds,x,fx,fy)


    
                                     done
    

\>function ds(fx,fy) &&= sqrt(diff(fx,x)^2+diff(fy,x)^2)


    
                               2              2
                      sqrt(diff (fy, x) + diff (fx, x))
    

\>sol &= ds(x\*cos(x),x\*sin(x)); $sol // Kita gunakan untuk menghitung panjang kurva terakhir di atas


$$\sqrt{\left(\cos x-x\,\sin x\right)^2+\left(\sin x+x\,\cos x\right)  ^2}$$\>$sol | trigreduce | expand, $integrate(%,x,0,2\*pi), %()


$$\frac{{\rm asinh}\; \left(2\,\pi\right)+2\,\pi\,\sqrt{4\,\pi^2+1}}{  2}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-739.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-739.png)

    21.2562941482

Hasilnya sama dengan perhitungan menggunakan fungsi EMT.


Berikut adalah contoh lain penggunaan fungsi Maxima tersebut.


\>plot2d("3\*x^2-1","3\*x^3-1",xmin=-1/sqrt(3),xmax=1/sqrt(3),square=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-740.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-740.png)

\>sol &= radcan(ds(3\*x^2-1,3\*x^3-1)); $sol


$$3\,x\,\sqrt{9\,x^2+4}$$\>$showev('integrate(sol,x,0,1/sqrt(3))), $2\*float(%) // panjang kurva di atas


$$6.0\,\int_{0.0}^{0.5773502691896258}{x\,\sqrt{9.0\,x^2+4.0}\;dx}=  2.337835372767141$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-743.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-743.png)

## Sikloid

Berikut kita akan menghitung panjang kurva lintasan (sikloid) suatu
titik pada lingkaran yang berputar ke kanan pada permukaan datar.
Misalkan jari-jari lingkaran tersebut adalah r. Posisi titik pusat
lingkaran pada saat t adalah:


$$(rt,r).$$Misalkan posisi titik pada lingkaran tersebut mula-mula (0,0) dan
posisinya pada saat t adalah:


$$(r(t-\sin(t)),r(1-\cos(t))).$$Berikut kita plot lintasan tersebut dan beberapa posisi lingkaran
ketika t=0, t=pi/2, t=r*pi.


\>x &= r\*(t-sin(t))


    
            [0, 1.66665833335744e-7 r, 1.33330666692022e-6 r, 
    4.499797504338432e-6 r, 1.066581336583994e-5 r, 
    2.083072932167196e-5 r, 3.599352055540239e-5 r, 
    5.71526624672386e-5 r, 8.530603082730626e-5 r, 
    1.214508019889565e-4 r, 1.665833531718508e-4 r, 
    2.216991628251896e-4 r, 2.877927110806339e-4 r, 
    3.658573803051457e-4 r, 4.568853557635201e-4 r, 
    5.618675264007778e-4 r, 6.817933857540259e-4 r, 
    8.176509330039827e-4 r, 9.704265741758145e-4 r, 
    0.001141105023499428 r, 0.001330669204938795 r, 
    0.001540100153900437 r, 0.001770376919130678 r, 
    0.002022476464811601 r, 0.002297373572865413 r, 
    0.002596040745477063 r, 0.002919448107844891 r, 
    0.003268563311168871 r, 0.003644351435886262 r, 
    0.004047774895164447 r, 0.004479793338660443 r, 0.0049413635565565 r, 
    0.005433439383882244 r, 0.005956971605131645 r, 
    0.006512907859185624 r, 0.007102192544548636 r, 
    0.007725766724910044 r, 0.00838456803503801 r, 
    0.009079530587017326 r, 0.009811584876838586 r, 0.0105816576913495 r, 
    0.01139067201557714 r, 0.01223954694042984 r, 0.01312919757078923 r, 
    0.01406053493400045 r, 0.01503446588876983 r, 0.01605189303448024 r, 
    0.01711371462093175 r, 0.01822082445851714 r, 0.01937411182884202 r, 
    0.02057446139579705 r, 0.02182275311709253 r, 0.02311986215626333 r, 
    0.02446665879515308 r, 0.02586400834688696 r, 0.02731277106934082 r, 
    0.02881380207911666 r, 0.03036795126603076 r, 0.03197606320812652 r, 
    0.0336389770872163 r, 0.03535752660496472 r, 0.03713253989951881 r, 
    0.03896483946269502 r, 0.0408552420577305 r, 0.04280455863760801 r, 
    0.04481359426396048 r, 0.04688314802656623 r, 0.04901401296344043 r, 
    0.05120697598153157 r, 0.05346281777803219 r, 0.05578231276230905 r, 
    0.05816622897846346 r, 0.06061532802852698 r, 0.0631303649963022 r, 
    0.06571208837185505 r, 0.06836123997666599 r, 0.07107855488944881 r, 
    0.07386476137264342 r, 0.07672058079958999 r, 0.07964672758239233 r, 
    0.08264390910047736 r, 0.0857128256298576 r, 0.08885417027310427 r, 
    0.09206862889003742 r, 0.09535688002914089 r, 0.0987195948597075 r, 
    0.1021574371047232 r, 0.1056710629744951 r, 0.1092611211010309 r, 
    0.1129282524731764 r, 0.1166730903725168 r, 0.1204962603100498 r, 
    0.1243983799636342 r, 0.1283800591162231 r, 0.1324418995948859 r, 
    0.1365844952106265 r, 0.140808431699002 r, 0.1451142866615502 r, 
    0.1495026295080298 r, 0.1539740213994798 r]
    

\>y &= r\*(1-cos(t))


    
            [0, 4.999958333473664e-5 r, 1.999933334222437e-4 r, 
    4.499662510124569e-4 r, 7.998933390220841e-4 r, 
    0.001249739605033717 r, 0.00179946006479581 r, 
    0.002448999746720415 r, 0.003198293697380561 r, 
    0.004047266988005727 r, 0.004995834721974179 r, 
    0.006043902043303184 r, 0.00719136414613375 r, 0.00843810628521191 r, 
    0.009784003787362772 r, 0.01122892206395776 r, 0.01277271662437307 r, 
    0.01441523309043924 r, 0.01615630721187855 r, 0.01799576488272969 r, 
    0.01993342215875837 r, 0.02196908527585173 r, 0.02410255066939448 r, 
    0.02633360499462523 r, 0.02866202514797045 r, 0.03108757828935527 r, 
    0.03361002186548678 r, 0.03622910363410947 r, 0.03894456168922911 r, 
    0.04175612448730281 r, 0.04466351087439402 r, 0.04766643011428662 r, 
    0.05076458191755917 r, 0.0539576564716131 r, 0.05724533447165381 r, 
    0.06062728715262111 r, 0.06410317632206519 r, 0.06767265439396564 r, 
    0.07133536442348987 r, 0.07509094014268702 r, 0.07893900599711501 r, 
    0.08287917718339499 r, 0.08691105968769186 r, 0.09103425032511492 r, 
    0.09524833678003664 r, 0.09955289764732322 r, 0.1039475024744748 r, 
    0.1084317118046711 r, 0.113005077220716 r, 0.1176671413898787 r, 
    0.1224174381096274 r, 0.1272554923542488 r, 0.1321808203223502 r, 
    0.1371929294852391 r, 0.1422913186361759 r, 0.1474754779404944 r, 
    0.152744888986584 r, 0.1580990248377314 r, 0.1635373500848132 r, 
    0.1690593208998367 r, 0.1746643850903219 r, 0.1803519821545206 r, 
    0.1861215433374662 r, 0.1919724916878484 r, 0.1979042421157076 r, 
    0.2039162014509444 r, 0.2100077685026351 r, 0.216178334119151 r, 
    0.2224272812490723 r, 0.2287539850028937 r, 0.2351578127155118 r, 
    0.2416381240094921 r, 0.2481942708591053 r, 0.2548255976551299 r, 
    0.2615314412704124 r, 0.2683111311261794 r, 0.2751639892590951 r, 
    0.2820893303890569 r, 0.2890864619877229 r, 0.2961546843477643 r, 
    0.3032932906528349 r, 0.3105015670482534 r, 0.3177787927123868 r, 
    0.3251242399287333 r, 0.3325371741586922 r, 0.3400168541150183 r, 
    0.3475625318359485 r, 0.3551734527599992 r, 0.3628488558014202 r, 
    0.3705879734263036 r, 0.3783900317293359 r, 0.3862542505111889 r, 
    0.3941798433565377 r, 0.4021660177127022 r, 0.4102119749689023 r, 
    0.418316910536117 r, 0.4264800139275439 r, 0.4347004688396462 r, 
    0.4429774532337832 r, 0.451310139418413 r]
    

Berikut kita gambar sikloid untuk r=1.


\>ex &= x-sin(x); ey &= 1-cos(x); aspect(1);

\>plot2d(ex,ey,xmin=0,xmax=4pi,square=1); ...  
\>     plot2d("2+cos(x)","1+sin(x)",xmin=0,xmax=2pi,\>add,color=blue); ...  
\>     plot2d([2,ex(2)],[1,ey(2)],color=red,\>add); ...  
\>     plot2d(ex(2),ey(2),\>points,\>add,color=red); ...  
\>     plot2d("2pi+cos(x)","1+sin(x)",xmin=0,xmax=2pi,\>add,color=blue); ...  
\>     plot2d([2pi,ex(2pi)],[1,ey(2pi)],color=red,\>add);  ...  
\>     plot2d(ex(2pi),ey(2pi),\>points,\>add,color=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-746.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-746.png)

Berikut dihitung panjang lintasan untuk 1 putaran penuh. (Jangan salah
menduga bahwa panjang lintasan 1 putaran penuh sama dengan keliling
lingkaran!)


\>ds &= radcan(sqrt(diff(ex,x)^2+diff(ey,x)^2)); $ds=trigsimp(ds) // elemen panjang kurva sikloid


$$\sqrt{\sin ^2x+\cos ^2x-2\,\cos x+1}=\sqrt{2-2\,\cos x}$$\>ds &= trigsimp(ds); $ds


$$\sqrt{2-2\,\cos x}$$\>$showev('integrate(ds,x,0,2\*pi)) // hitung panjang sikloid satu putaran penuh


$$\int_{0}^{2\,\pi}{\sqrt{2-2\,\cos x}\;dx}=8$$\>integrate(mxm("ds"),0,2\*pi) // hitung secara numerik


    8

\>romberg(mxm("ds"),0,2\*pi) // cara lain hitung secara numerik


    8

Perhatikan, seperti terlihat pada gambar, panjang sikloid lebih besar
daripada keliling lingkarannya, yakni:


$$2\pi.$$## Kurvatur (Kelengkungan) Kurva

image: Osculating.png


Aslinya, kelengkungan kurva diferensiabel (yakni, kurva mulus yang
tidak lancip) di titik P didefinisikan melalui lingkaran oskulasi
(yaitu, lingkaran yang melalui titik P dan terbaik memperkirakan,
paling banyak menyinggung kurva di sekitar P). Pusat dan radius
kelengkungan kurva di P adalah pusat dan radius lingkaran oskulasi.
Kelengkungan adalah kebalikan dari radius kelengkungan:


$$\kappa =\frac {1}{R}$$dengan R adalah radius kelengkungan. (Setiap lingkaran memiliki
kelengkungan ini pada setiap titiknya, dapat diartikan, setiap
lingkaran berputar 2pi sejauh 2piR.)


Definisi ini sulit dimanipulasi dan dinyatakan ke dalam rumus untuk
kurva umum. Oleh karena itu digunakan definisi lain yang ekivalen.


## Definisi Kurvatur dengan Fungsi Parametrik Panjang Kurva



Setiap kurva diferensiabel dapat dinyatakan dengan persamaan
parametrik terhadap panjang kurva s:


$$\gamma(s) = (x(s),\ y(s)),$$dengan x dan y adalah fungsi riil yang diferensiabel, yang memenuhi:


$$\|\gamma'(s)\|=\sqrt{x'(s)^2+y'(s)^2}=1.$$Ini berarti bahwa vektor singgung


$$\mathbf{T}(s)=(x'(s),\ y'(s))$$memiliki norm 1 dan merupakan vektor singgung satuan.


Apabila kurvanya memiliki turunan kedua, artinya turunan kedua x dan y
ada, maka T'(s) ada. Vektor ini merupakan normal kurva yang arahnya
menuju pusat kurvatur, norm-nya merupakan nilai kurvatur
(kelengkungan):


$$ \begin{aligned}\mathbf{T}(s) &= \mathbf{\gamma}'(s),\\ \mathbf{T}^{2}(s) &=1\ \text{(konstanta)}\Rightarrow \mathbf{T}'(s)\cdot \mathbf{T}(s)=0\\ \kappa(s) &=\|\mathbf {T}'(s)\|= \|\mathbf{\gamma}''(s)\|=\sqrt{x''(s)^{2}+y''(s)^{2}}.\end{aligned}$$Nilai


$$R(s)=\frac{1}{\kappa(s)}$$disebut jari-jari (radius) kelengkungan kurva.


Bilangan riil


$$ k(s) = \pm\kappa(s)$$disebut nilai kelengkungan bertanda.


Contoh:


Akan ditentukan kurvatur lingkaran


$$x=r\cos t,\ y= r\sin t.$$\>fx &= r\*cos(t); fy &=r\*sin(t);

\>&assume(t\>0,r\>0); s &=integrate(sqrt(diff(fx,t)^2+diff(fy,t)^2),t,0,t); s // elemen panjang kurva, panjang busur lingkaran (s)


    
                                     r t
    

\>&kill(s); fx &= r\*cos(s/r); fy &=r\*sin(s/r); // definisi ulang persamaan parametrik terhadap s dengan substitusi t=s/r

\>k &= trigsimp(sqrt(diff(fx,s,2)^2+diff(fy,s,2)^2)); $k // nilai kurvatur lingkaran dengan menggunakan definisi di atas


$$\frac{1}{r}$$Untuk representasi parametrik umum, misalkan


$$x = x(t),\ y= y(t)$$merupakan persamaan parametrik untuk kurva bidang yang
terdiferensialkan dua kali. Kurvatur untuk kurva tersebut
didefinisikan sebagai


$$\begin{aligned}\kappa &= \frac{d\phi}{ds}=\frac{\frac{d\phi}{dt}}{\frac{ds}{dt}}\quad (\phi \text{ adalah sudut kemiringan garis singgung dan }s \text{ adalah panjang kurva})\\ &=\frac{\frac{d\phi}{dt}}{\sqrt{(\frac{dx}{dt})^2+(\frac{dy}{dt})^2}}= \frac{\frac{d\phi}{dt}}{\sqrt{x'(t)^2+y'(t)^2}}.\end{aligned}.$$Selanjutnya, pembilang pada persamaan di atas dapat dicari sebagai
berikut.


$$\begin{aligned}\sec^2\phi\frac{d\phi}{dt} &= \frac{d}{dt}\left(\tan\phi\right)= \frac{d}{dt}\left(\frac{dy}{dx}\right)= \frac{d}{dt}\left(\frac{dy/dt}{dx/dt}\right)= \frac{d}{dt}\left(\frac{y'(t)}{x'(t)}\right)=\frac{x'(t)y''(t)-x''(t)y'(t)}{x'(t)^2}.\\ & \\ \frac{d\phi}{dt} &= \frac{1}{\sec^2\phi}\frac{x'(t)y''(t)-x''(t)y'(t)}{x'(t)^2}\\ &= \frac{1}{1+\tan^2\phi}\frac{x'(t)y''(t)-x''(t)y'(t)}{x'(t)^2}\\ &= \frac{1}{1+\left(\frac{y'(t)}{x'(t)}\right)^2}\frac{x'(t)y''(t)-x''(t)y'(t)}{x'(t)^2}\\ &= \frac{x'(t)y''(t)-x''(t)y'(t)}{x'(t)^2+y'(t)^2}.\end{aligned}$$Jadi, rumus kurvatur untuk kurva parametrik


$$x=x(t),\ y=y(t)$$adalah


$$\kappa(t) = \frac{x'(t)y''(t)-x''(t)y'(t)}{\left(x'(t)^2+y'(t)^2\right)^{3/2}}.$$Jika kurvanya dinyatakan dengan persamaan parametrik pada koordinat
kutub


$$x=r(\theta)\cos\theta,\ y=r(\theta)\sin\theta,$$maka rumus kurvaturnya adalah


$$\kappa(\theta) = \frac{r(\theta)^2+2r'(\theta)^2-r(\theta)r''(\theta)}{\left(r'(\theta)^2+r'(\theta)^2\right)^{3/2}}.$$(Silakan Anda turunkan rumus tersebut!)


Contoh:


Lingkaran dengan pusat (0,0) dan jari-jari r dapat dinyatakan dengan
persamaan parametrik


$$x=r\cos t,\ y=r\sin t.$$Nilai kelengkungan lingkaran tersebut adalah


$$\kappa(t)=\frac{x'(t)y''(t)-x''(t)y'(t)}{\left(x'(t)^2+y'(t)^2\right)^{3/2}}=\frac{r^2}{r^3}=\frac 1 r.$$Hasil cocok dengan definisi kurvatur suatu kelengkungan.


Kurva


$$y=f(x)$$dapat dinyatakan ke dalam persamaan parametrik


$$x=t,\ y=f(t),\ \text{ dengan } x'(t)=1,\ x''(t)=0,$$sehingga kurvaturnya adalah


$$\kappa(t) = \frac{y''(t)}{\left(1+y'(t)^2\right)^{3/2}}.$$Contoh:


Akan ditentukan kurvatur parabola


$$y=ax^2+bx+c.$$\>function f(x) &= a\*x^2+b\*x+c; $'y=f(x)


$$y=a\,x^2+b\,x+c$$\>function k(x) &= (diff(f(x),x,2))/(1+diff(f(x),x)^2)^(3/2); $'k(x)=k(x) // kelengkungan parabola 


$$k\left(x\right)=\frac{2\,a}{\left(\left(2\,a\,x+b\right)^2+1\right)  ^{\frac{3}{2}}}$$\>function f(x) &= x^2+x+1; $'y=f(x) // akan kita plot kelengkungan parabola untuk a=b=c=1


$$y=x^2+x+1$$\>function k(x) &= (diff(f(x),x,2))/(1+diff(f(x),x)^2)^(3/2); $'k(x)=k(x) // kelengkungan parabola 


$$k\left(x\right)=\frac{2}{\left(\left(2\,x+1\right)^2+1\right)^{  \frac{3}{2}}}$$Berikut kita gambar parabola tersebut beserta kurva kelengkungan,
kurva jari-jari kelengkungan dan salah satu lingkaran oskulasi di
titik puncak parabola. Perhatikan, puncak parabola dan jari-jari
lingkaran oskulasi di puncak parabola adalah


$$(-1/2,3/4),\ 1/k(2)=1/2,$$sehingga pusat lingkaran oskulasi adalah (-1/2, 5/4).


\>plot2d(["f(x)", "k(x)"],-2,1, color=[blue,red]); plot2d("1/k(x)",-1.5,1,color=green,\>add); ...  
\>   plot2d("-1/2+1/k(-1/2)\*cos(x)","5/4+1/k(-1/2)\*sin(x)",xmin=0,xmax=2pi,\>add,color=blue):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-778.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-778.png)

Untuk kurva yang dinyatakan dengan fungsi implisit


$$F(x,y)=0$$dengan turunan-turunan parsial


$$F_x=\frac{\partial F}{\partial x},\ F_y=\frac{\partial F}{\partial y},\ F_{xy}=\frac{\partial}{\partial y}\left(\frac{\partial F}{\partial x}\right),\ F_{xx}=\frac{\partial}{\partial x}\left(\frac{\partial F}{\partial x}\right),\ F_{yy}=\frac{\partial}{\partial y}\left(\frac{\partial F}{\partial y}\right),$$berlaku


$$F_x dx+ F_y dy = 0\text{ atau } \frac{dy}{dx}=-\frac{F_x}{F_y},$$sehingga kurvaturnya adalah


$$\kappa =\frac {F_y^2F_{xx}-2F_xF_yF_{xy}+F_x^2F_{yy}}{\left(F_x^2+F_y^2\right)^{3/2}}.$$(Silakan Anda turunkan sendiri!)


Contoh 1:


Parabola


$$y=ax^2+bx+c$$dapat dinyatakan ke dalam persamaan implisit


$$ax^2+bx+c-y=0.$$\>function F(x,y) &=a\*x^2+b\*x+c-y; $'F(x,y)=F(x,y)


$$F\left(x , y\right)=-y+a\,x^2+b\,x+c$$\>Fx &= diff(F(x,y),x), Fxx &=diff(F(x,y),x,2), Fy &=diff(F(x,y),y), Fxy &=diff(diff(F(x,y),x),y), Fyy &=diff(F(x,y),y,2)  


    
                                  2 a x + b
    
    
                                     2 a
    
    
                                     - 1
    
    
                                      0
    
    
                                      0
    

\>function k(x) &= (Fy^2\*Fxx-2\*Fx\*Fy\*Fxy+Fx^2\*Fyy)/(Fx^2+Fy^2)^(3/2); $'k(x)=k(x) // kurvatur parabola tersebut


$$k\left(x\right)=\frac{2\,a}{\left(\left(2\,a\,x+b\right)^2+1\right)  ^{\frac{3}{2}}}$$Hasilnya sama dengan sebelumnya yang menggunakan persamaan parabola biasa.


# Latihan

* 
Bukalah buku Kalkulus.

* 
Cari dan pilih beberapa (paling sedikit 5 fungsi berbeda
* tipe/bentuk/jenis) fungsi dari buku tersebut, kemudian definisikan di
* EMT pada baris-baris perintah berikut (jika perlu tambahkan lagi).

* 
Untuk setiap fungsi, tentukan anti turunannya (jika ada), hitunglah
* integral tentu dengan batas-batas yang menarik (Anda tentukan
* sendiri), seperti contoh-contoh tersebut.

* 
Lakukan hal yang sama untuk fungsi-fungsi yang tidak dapat
* diintegralkan (cari sedikitnya 3 fungsi).

* 
Gambar grafik fungsi dan daerah integrasinya pada sumbu koordinat
* yang sama.

* 
Gunakan integral tentu untuk mencari luas daerah yang dibatasi oleh
* dua kurva yang berpotongan di dua titik. (Cari dan gambar kedua kurva
* dan arsir (warnai) daerah yang dibatasi oleh keduanya.)

* 
Gunakan integral tentu untuk menghitung volume benda putar kurva y=
* f(x) yang diputar mengelilingi sumbu x dari x=a sampai x=b, yakni


$$V = \int_a^b \pi (f(x)^2\ dx.$$(Pilih fungsinya dan gambar kurva dan benda putar yang dihasilkan.
Anda dapat mencari contoh-contoh bagaimana cara menggambar benda hasil
perputaran suatu kurva.)


- Gunakan integral tentu untuk menghitung panjang kurva y=f(x) dari
x=a sampai x=b dengan menggunakan rumus:


$$S = \int_a^b \sqrt{1+(f'(x))^2} \ dx.$$(Pilih fungsi dan gambar kurvanya.)


- Apabila fungsi dinyatakan dalam koordinat kutub x=f(r,t), y=g(r,t),
r=h(t), x=a bersesuaian dengan t=t0 dan x=b bersesuian dengan t=t1,
maka rumus di atas akan menjadi:


$$S=\int_{t_0}^{t_1} \sqrt{x'(t)^2+y'(t)^2}\ dt.$$* 
Pilih beberapa kurva menarik (selain lingkaran dan parabola) dari
* buku  kalkulus. Nyatakan setiap kurva tersebut dalam bentuk:
*   a. koordinat Kartesius (persamaan y=f(x))
*   b. koordinat kutub ( r=r(theta))
*   c. persamaan parametrik x=x(t), y=y(t)
*   d. persamaan implit F(x,y)=0

* 
Tentukan kurvatur masing-masing kurva dengan menggunakan keempat
* representasi tersebut (hasilnya harus sama).

* 
Gambarlah kurva asli, kurva kurvatur, kurva jari-jari lingkaran
* oskulasi, dan salah satu lingkaran oskulasinya.


\>function f(x) &= cos(x)-sin(x); $'f(x)=f(x)


$$f\left(x\right)=\cos x-\sin x$$\>$showev('integrate(f(x),x)), $showev('integrate(f(x),x,0,pi))


$$\int_{0}^{\pi}{\cos x-\sin x\;dx}=-2$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-792.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-792.png)

\>function g(x) &= 1/x+sinh(x); $'g(x)=g(x), $showev('integrate(g(x),x))


$$\int {\sinh x+\frac{1}{x}}{\;dx}=\log x+\cosh x$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-794.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-794.png)

# Barisan dan Deret

(Catatan: bagian ini belum lengkap. Anda dapat membaca contoh-contoh
pengguanaan EMT dan Maxima untuk menghitung limit barisan, rumus
jumlah parsial suatu deret, jumlah tak hingga suatu deret konvergen,
dan sebagainya. Anda dapat mengeksplor contoh-contoh di EMT atau
perbagai panduan penggunaan Maxima di software Maxima atau dari
Internet.)


Barisan dapat didefinisikan dengan beberapa cara di dalam EMT, di
antaranya:


* 
dengan cara yang sama seperti mendefinisikan vektor dengan
* elemen-elemen beraturan (menggunakan titik dua ":");

* 
menggunakan perintah "sequence" dan rumus barisan (suku ke -n);

* 
menggunakan perintah "iterate" atau "niterate";

* 
menggunakan fungsi Maxima "create_list" atau "makelist" untuk
* menghasilkan barisan simbolik;

* 
menggunakan fungsi biasa yang inputnya vektor atau barisan;

* 
menggunakan fungsi rekursif.


EMT menyediakan beberapa perintah (fungsi) terkait barisan, yakni:


* 
sum: menghitung jumlah semua elemen suatu barisan

* 
cumsum: jumlah kumulatif suatu barisan

* 
differences: selisih antar elemen-elemen berturutan


EMT juga dapat digunakan untuk menghitung jumlah deret berhingga
maupun deret tak hingga, dengan menggunakan perintah (fungsi) "sum".
Perhitungan dapat dilakukan secara numerik maupun simbolik dan eksak.


Berikut adalah beberapa contoh perhitungan barisan dan deret
menggunakan EMT.


\>1:10 // barisan sederhana


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

\>1:2:30


    [1,  3,  5,  7,  9,  11,  13,  15,  17,  19,  21,  23,  25,  27,  29]

# Iterasi dan Barisan

EMT menyediakan fungsi iterate("g(x)", x0, n) untuk melakukan iterasi


$$x_{k+1}=g(x_k), \ x_0=x_0, k= 1, 2, 3, ..., n.$$Berikut ini disajikan contoh-contoh penggunaan iterasi dan rekursi
dengan EMT. Contoh pertama menunjukkan pertumbuhan dari nilai awal
1000 dengan laju pertambahan 5%, selama 10 periode.


\>q=1.05; iterate("x\*q",1000,n=10)'


             1000 
             1050 
           1102.5 
          1157.63 
          1215.51 
          1276.28 
           1340.1 
           1407.1 
          1477.46 
          1551.33 
          1628.89 

Contoh berikutnya memperlihatkan bahaya menabung di bank pada masa
sekarang! Dengan bunga tabungan sebesar 6% per tahun atau 0.5% per
bulan dipotong pajak 20%, dan biaya administrasi 10000 per bulan,
tabungan sebesar 1 juta tanpa diambil selama sekitar 10 tahunan akan
habis diambil oleh bank!


\>r=0.005; plot2d(iterate("(1+0.8\*r)\*x-10000",1000000,n=130)):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-796.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-796.png)

Silakan Anda coba-coba, dengan tabungan minimal berapa agar tidak akan
habis diambil oleh bank dengan ketentuan bunga dan biaya administrasi
seperti di atas.


Berikut adalah perhitungan minimal tabungan agar aman di bank dengan
bunga sebesar r dan biaya administrasi a, pajak bunga 20%.


\>$solve(0.8\*r\*A-a,A), $% with [r=0.005, a=10] 


$$\left[ A=2500.0 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-798.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-798.png)

Berikut didefinisikan fungsi untuk menghitung saldo tabungan, kemudian
dilakukan iterasi.


\>function saldo(x,r,a) := round((1+0.8\*r)\*x-a,2);

\>iterate({{"saldo",0.005,10}},1000,n=6)


    [1000,  994,  987.98,  981.93,  975.86,  969.76,  963.64]

\>iterate({{"saldo",0.005,10}},2000,n=6)


    [2000,  1998,  1995.99,  1993.97,  1991.95,  1989.92,  1987.88]

\>iterate({{"saldo",0.005,10}},2500,n=6)


    [2500,  2500,  2500,  2500,  2500,  2500,  2500]

Tabungan senilai 2,5 juta akan aman dan tidak akan berubah nilai (jika
tidak ada penarikan), sedangkan jika tabungan awal kurang dari 2,5
juta, lama kelamaan akan berkurang meskipun tidak pernah dilakukan
penarikan uang tabungan.


\>iterate({{"saldo",0.005,10}},3000,n=6)


    [3000,  3002,  3004.01,  3006.03,  3008.05,  3010.08,  3012.12]

Tabungan yang lebih dari 2,5 juta baru akan bertambah jika tidak ada
penarikan.


Untuk barisan yang lebih kompleks dapat digunakan fungsi "sequence()".
Fungsi ini menghitung nilai-nilai x[n] dari semua nilai sebelumnya,
x[1],...,x[n-1] yang diketahui.


Berikut adalah contoh barisan Fibonacci.


$$x_n = x_{n-1}+x_{n-2}, \quad x_1=1, \quad x_2 =1$$\>sequence("x[n-1]+x[n-2]",[1,1],15)


    [1,  1,  2,  3,  5,  8,  13,  21,  34,  55,  89,  144,  233,  377,  610]

Barisan Fibonacci memiliki banyak sifat menarik, salah satunya adalah
akar pangkat ke-n suku ke-n akan konvergen ke pecahan emas:


\>$'(1+sqrt(5))/2=float((1+sqrt(5))/2)


$$\frac{\sqrt{5}+1}{2}=1.618033988749895$$\>plot2d(sequence("x[n-1]+x[n-2]",[1,1],250)^(1/(1:250))):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-801.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-801.png)

Barisan yang sama juga dapat dihasilkan dengan menggunakan loop.


\>x=ones(500); for k=3 to 500; x[k]=x[k-1]+x[k-2]; end;


Rekursi dapat dilakukan dengan menggunakan rumus yang tergantung pada
semua elemen sebelumnya. Pada contoh berikut, elemen ke-n merupakan
jumlah (n-1) elemen sebelumnya, dimulai dengan 1 (elemen ke-1). Jelas,
nilai elemen ke-n adalah 2^(n-2), untuk n=2, 4, 5, ....


\>sequence("sum(x)",1,10)


    [1,  1,  2,  4,  8,  16,  32,  64,  128,  256]

Selain menggunakan ekspresi dalam x dan n, kita juga dapat menggunakan
fungsi.


Pada contoh berikut, digunakan iterasi


$$x_n =A \cdot x_{n-1},$$dengan A suatu matriks 2x2, dan setiap x[n] merupakan matriks/vektor
2x1.


\>A=[1,1;1,2]; function suku(x,n) := A.x[,n-1]

\>sequence("suku",[1;1],6)


    Real 2 x 6 matrix
    
                1             2             5            13     ...
                1             3             8            21     ...

Hasil yang sama juga dapat diperoleh dengan menggunakan fungsi
perpangkatan matriks "matrixpower()". Cara ini lebih cepat, karena
hanya menggunakan perkalian matriks sebanyak log_2(n).


$$x_n=A.x_{n-1}=A^2.x_{n-2}=A^3.x_{n-3}= ... = A^{n-1}.x_1.$$\>sequence("matrixpower(A,n).[1;1]",1,6)


    Real 2 x 6 matrix
    
                1             5            13            34     ...
                1             8            21            55     ...

# Spiral Theodorus

image: Spiral_of_Theodorus.png


Spiral Theodorus (spiral segitiga siku-siku) dapat digambar secara
rekursif. Rumus rekursifnya adalah:


$$x_n = \left( 1 + \frac{i}{\sqrt{n-1}} \right) \, x_{n-1}, \quad x_1=1,$$yang menghasilkan barisan bilangan kompleks.


\>function g(n) := 1+I/sqrt(n)


Rekursinya dapat dijalankan sebanyak 17 untuk menghasilkan barisan 17
bilangan kompleks, kemudian digambar bilangan-bilangan kompleksnya.


\>x=sequence("g(n-1)\*x[n-1]",1,17); plot2d(x,r=3.5); textbox(latex("Spiral\\ Theodorus"),0.4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-805.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-805.png)

Selanjutnya dihubungan titik 0 dengan titik-titik kompleks tersebut
menggunakan loop.


\>for i=1:cols(x); plot2d([0,x[i]],\>add); end:


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-806.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-806.png)

\> 


Spiral tersebut juga dapat didefinisikan menggunakan fungsi rekursif,
yang tidak memmerlukan indeks dan bilangan kompleks. Dalam hal ini
diigunakan vektor kolom pada bidang.


\>function gstep (v) ...


    w=[-v[2];v[1]];
    return v+w/norm(w);
    endfunction
</pre>
Jika dilakukan iterasi 16 kali dimulai dari [1;0] akan didapatkan
matriks yang memuat vektor-vektor dari setiap iterasi.


\>x=iterate("gstep",[1;0],16); plot2d(x[1],x[2],r=3.5,\>points):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-807.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-807.png)

# Kekonvergenan

Terkadang kita ingin melakukan iterasi sampai konvergen. Apabila
iterasinya tidak konvergen setelah ditunggu lama, Anda dapat
menghentikannya dengan menekan tombol [ESC].


\>iterate("cos(x)",1) // iterasi x(n+1)=cos(x(n)), dengan x(0)=1.


    0.739085133216

Iterasi tersebut konvergen ke penyelesaian persamaan


$$x = \cos(x).$$Iterasi ini juga dapat dilakukan pada interval, hasilnya adalah
barisan interval yang memuat akar tersebut.


\>hasil := iterate("cos(x)",~1,2~) //iterasi x(n+1)=cos(x(n)), dengan interval awal (1, 2)


    ~0.739085133211,0.7390851332133~

Jika interval hasil tersebut sedikit diperlebar, akan terlihat bahwa
interval tersebut memuat akar persamaan x=cos(x).


\>h=expand(hasil,100), cos(h) << h


    ~0.73908513309,0.73908513333~
    1

Iterasi juga dapat digunakan pada fungsi yang didefinisikan.


\>function f(x) := (x+2/x)/2


Iterasi x(n+1)=f(x(n)) akan konvergen ke akar kuadrat 2.


\>iterate("f",2), sqrt(2)


    1.41421356237
    1.41421356237

Jika pada perintah iterate diberikan tambahan parameter n, maka hasil
iterasinya akan ditampilkan mulai dari iterasi pertama sampai ke-n.


\>iterate("f",2,5)


    [2,  1.5,  1.41667,  1.41422,  1.41421,  1.41421]

Untuk iterasi ini tidak dapat dilakukan terhadap interval.


\>niterate("f",~1,2~,5)


    [ ~1,2~,  ~1,2~,  ~1,2~,  ~1,2~,  ~1,2~,  ~1,2~ ]

Perhatikan, hasil iterasinya sama dengan interval awal. Alasannya
adalah perhitungan dengan interval bersifat terlalu longgar. Untuk
meingkatkan perhitungan pada ekspresi dapat digunakan pembagian
intervalnya, menggunakan fungsi ieval().


\>function s(x) := ieval("(x+2/x)/2",x,10)


Selanjutnya dapat dilakukan iterasi hingga diperoleh hasil optimal,
dan intervalnya tidak semakin mengecil. Hasilnya berupa interval yang
memuat akar persamaan:


$$x = \frac{1}{2} \left( x + \frac{2}{x} \right).$$Satu-satunya solusi adalah


$$x = \sqrt2.$$\>iterate("s",~1,2~)


    ~1.41421356236,1.41421356239~

Fungsi "iterate()" juga dapat bekerja pada vektor. Berikut adalah
contoh fungsi vektor, yang menghasilkan rata-rata aritmetika dan
rata-rata geometri.


$$(a_{n+1},b_{n+1}) = \left( \frac{a_n+b_n}{2}, \sqrt{a_nb_n} \right)$$Iterasi ke-n disimpan pada vektor kolom x[n].


\>function g(x) := [(x[1]+x[2])/2;sqrt(x[1]\*x[2])]


Iterasi dengan menggunakan fungsi tersebut akan konvergen ke rata-rata
aritmetika dan geometri dari nilai-nilai awal.


\>iterate("g",[1;5])


          2.60401 
          2.60401 

Hasil tersebut konvergen agak cepat, seperti kita cek sebagai berikut.


\>iterate("g",[1;5],4)


                1             3       2.61803       2.60403       2.60401 
                5       2.23607       2.59002       2.60399       2.60401 

Iterasi pada interval dapat dilakukan dan stabil, namun tidak
menunjukkan bahwa limitnya pada batas-batas yang dihitung.


\>iterate("g",[~1~;~5~],4)


    Interval 2 x 5 matrix
    
    ~0.999999999999999778,1.00000000000000022~     ...
    ~4.99999999999999911,5.00000000000000089~     ...

Iterasi berikut konvergen sangat lambat.


$$x_{n+1} = \sqrt{x_n}.$$\>iterate("sqrt(x)",2,10)


    [2,  1.41421,  1.18921,  1.09051,  1.04427,  1.0219,  1.01089,
    1.00543,  1.00271,  1.00135,  1.00068]

Kekonvergenan iterasi tersebut dapat dipercepatdengan percepatan
Steffenson:


\>steffenson("sqrt(x)",2,10)


    [1.04888,  1.00028,  1,  1]

# Iterasi menggunakan Loop yang ditulis Langsung

Berikut adalah beberapa contoh penggunaan loop untuk melakukan iterasi
yang ditulis langsung pada baris perintah.


\>x=2; repeat x=(x+2/x)/2; until x^2~=2; end; x,


    1.41421356237

Penggabungan matriks menggunakan tanda "|" dapat digunakan untuk
menyimpan semua hasil iterasi.


\>v=[1]; for i=2 to 8; v=v|(v[i-1]\*i); end; v,


    [1,  2,  6,  24,  120,  720,  5040,  40320]

hasil iterasi juga dapat disimpan pada vektor yang sudah ada.


\>v=ones(1,100); for i=2 to cols(v); v[i]=v[i-1]\*i; end; ...  
\>   plot2d(v,logplot=1); textbox(latex(&log(n)),x=0.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-813.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-813.png)

\>A =[0.5,0.2;0.7,0.1]; b=[2;2]; ...  
\>   x=[1;1]; repeat xnew=A.x-b; until all(xnew~=x); x=xnew; end; ...  
\>   x,


         -7.09677 
         -7.74194 

# Iterasi di dalam Fungsi

Fungsi atau program juga dapat menggunakan iterasi dan dapat digunakan
untuk melakukan iterasi. Berikut adalah beberapa contoh iterasi di
dalam fungsi.


Contoh berikut adalah suatu fungsi untuk menghitung berapa lama suatu
iterasi konvergen. Nilai fungsi tersebut adalah hasil akhir iterasi
dan banyak iterasi sampai konvergen.


\>function map hiter(f$,x0) ...


    x=x0;
    maxiter=0;
    repeat
      xnew=f$(x);
      maxiter=maxiter+1;
      until xnew~=x;
      x=xnew;
    end;
    return maxiter;
    endfunction
</pre>
Misalnya, berikut adalah iterasi untuk mendapatkan hampiran akar
kuadrat 2, cukup cepat, konvergen pada iterasi ke-5, jika dimulai dari
hampiran awal 2.


\>hiter("(x+2/x)/2",2)


    5

Karena fungsinya didefinisikan menggunakan "map". maka nilai awalnya
dapat berupa vektor.


\>x=1.5:0.1:10; hasil=hiter("(x+2/x)/2",x); ...  
\>     plot2d(x,hasil):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-814.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-814.png)

Dari gambar di atas terlihat bahwa kekonvergenan iterasinya semakin
lambat, untuk nilai awal semakin besar, namun penambahnnya tidak
kontinu. Kita dapat menemukan kapan maksimum iterasinya bertambah.


\>hasil[1:10]


    [4,  5,  5,  5,  5,  5,  6,  6,  6,  6]

\>x[nonzeros(differences(hasil))]


    [1.5,  2,  3.4,  6.6]

maksimum iterasi sampai konvergen meningkat pada saat nilai awalnya
1.5, 2, 3.4, dan 6.6.


Contoh berikutnya adalah metode Newton pada polinomial kompleks
berderajat 3.


\>p &= x^3-1; newton &= x-p/diff(p,x); $newton


$$x-\frac{x^3-1}{3\,x^2}$$Selanjutnya didefinisikan fungsi untuk melakukan iterasi (aslinya 10
kali).


\>function iterasi(f$,x,n=10) ...


    loop 1 to n; x=f$(x); end;
    return x;
    endfunction
</pre>
Kita mulai dengan menentukan titik-titik grid pada bidang kompleksnya.


\>r=1.5; x=linspace(-r,r,501); Z=x+I\*x'; W=iterasi(newton,Z);


Berikut adalah akar-akar polinomial di atas.


\>z=&solve(p)()


    [ -0.5+0.866025i,  -0.5-0.866025i,  1+0i  ]

Untuk menggambar hasil iterasinya, dihitung jarak dari hasil iterasi
ke-10 ke masing-masing akar, kemudian digunakan untuk menghitung warna
yang akan digambar, yang menunjukkan limit untuk masing-masing nilai
awal.


Fungsi plotrgb() menggunakan jendela gambar terkini untuk menggambar
warna RGB sebagai matriks.


\>C=rgb(max(abs(W-z[1]),1),max(abs(W-z[2]),1),max(abs(W-z[3]),1)); ...  
\>     plot2d(none,-r,r,-r,r); plotrgb(C):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-816.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-816.png)

# Iterasi Simbolik

Seperti sudah dibahas sebelumnya, untuk menghasilkan barisan ekspresi
simbolik dengan Maxima dapat digunakan fungsi makelist().


\>&powerdisp:true // untuk menampilkan deret pangkat mulai dari suku berpangkat terkecil


    
                                     true
    

\>deret &= makelist(taylor(exp(x),x,0,k),k,1,3); $deret // barisan deret Taylor untuk e^x


$$\left[ 1+x , 1+x+\frac{x^2}{2} , 1+x+\frac{x^2}{2}+\frac{x^3}{6}   \right] $$Untuk mengubah barisan deret tersebut menjadi vektor string di EMT
digunakan fungsi mxm2str(). Selanjutnya, vektor string/ekspresi
hasilnya dapat digambar seperti menggambar vektor eskpresi pada EMT.


\>plot2d("exp(x)",0,3); // plot fungsi aslinya, e^x

\>plot2d(mxm2str("deret"),\>add,color=4:6): // plot ketiga deret taylor hampiran fungsi tersebut


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-818.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-818.png)

Selain cara di atas dapat juga dengan cara menggunakan indeks pada
vektor/list yang dihasilkan.


\>$deret[3]


$$1+x+\frac{x^2}{2}+\frac{x^3}{6}$$\>plot2d(["exp(x)",&deret[1],&deret[2],&deret[3]],0,3,color=1:4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-820.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-820.png)

\>$sum(sin(k\*x)/k,k,1,5)


$$\sin x+\frac{\sin \left(2\,x\right)}{2}+\frac{\sin \left(3\,x  \right)}{3}+\frac{\sin \left(4\,x\right)}{4}+\frac{\sin \left(5\,x  \right)}{5}$$Berikut adalah cara menggambar kurva


$$y=\sin(x) + \dfrac{\sin 3x}{3} + \dfrac{\sin 5x}{5} + \ldots.$$\>plot2d(&sum(sin((2\*k+1)\*x)/(2\*k+1),k,0,20),0,2pi):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-823.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-823.png)

Hal serupa juga dapat dilakukan dengan menggunakan matriks, misalkan
kita akan menggambar kurva


$$y = \sum_{k=1}^{100} \dfrac{\sin(kx)}{k},\quad 0\le x\le 2\pi.$$\>x=linspace(0,2pi,1000); k=1:100; y=sum(sin(k\*x')/k)'; plot2d(x,y):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-825.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-825.png)

# Tabel Fungsi

Terdapat cara menarik untuk menghasilkan barisan dengan ekspresi
Maxima. Perintah mxmtable() berguna untuk menampilkan dan menggambar
barisan dan menghasilkan barisan sebagai vektor kolom.


Sebagai contoh berikut adalah barisan turunan ke-n x^x di x=1.


\>mxmtable("diffat(x^x,x=1,n)","n",1,8,frac=1);


            1 
            2 
            3 
            8 
           10 
           54 
          -42 
          944 

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-826.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-826.png)

\>$'sum(k, k, 1, n) = factor(ev(sum(k, k, 1, n),simpsum=true)) // simpsum:menghitung deret secara simbolik


$$\sum_{k=1}^{n}{k}=\frac{n\,\left(1+n\right)}{2}$$\>$'sum(1/(3^k+k), k, 0, inf) = factor(ev(sum(1/(3^k+k), k, 0, inf),simpsum=true))


$$\sum_{k=0}^{\infty }{\frac{1}{k+3^{k}}}=\sum_{k=0}^{\infty }{\frac{  1}{k+3^{k}}}$$Di sini masih gagal, hasilnya tidak dihitung.


\>$'sum(1/x^2, x, 1, inf)= ev(sum(1/x^2, x, 1, inf),simpsum=true) // ev: menghitung nilai ekspresi


$$\sum_{x=1}^{\infty }{\frac{1}{x^2}}=\frac{\pi^2}{6}$$\>$'sum((-1)^(k-1)/k, k, 1, inf) = factor(ev(sum((-1)^(x-1)/x, x, 1, inf),simpsum=true))


$$\sum_{k=1}^{\infty }{\frac{\left(-1\right)^{-1+k}}{k}}=-\sum_{x=1  }^{\infty }{\frac{\left(-1\right)^{x}}{x}}$$Di sini masih gagal, hasilnya tidak dihitung.


\>$'sum((-1)^k/(2\*k-1), k, 1, inf) = factor(ev(sum((-1)^k/(2\*k-1), k, 1, inf),simpsum=true))


$$\sum_{k=1}^{\infty }{\frac{\left(-1\right)^{k}}{-1+2\,k}}=\sum_{k=1  }^{\infty }{\frac{\left(-1\right)^{k}}{-1+2\,k}}$$\>$ev(sum(1/n!, n, 0, inf),simpsum=true)


$$\sum_{n=0}^{\infty }{\frac{1}{n!}}$$Di sini masih gagal, hasilnya tidak dihitung, harusnya hasilnya e.


\>&assume(abs(x)<1); $'sum(a\*x^k, k, 0, inf)=ev(sum(a\*x^k, k, 0, inf),simpsum=true), &forget(abs(x)<1);


$$a\,\sum_{k=0}^{\infty }{x^{k}}=\frac{a}{1-x}$$Deret geometri tak hingga, dengan asumsi rasional antara -1 dan 1.


\>$'sum(x^k/k!,k,0,inf)=ev(sum(x^k/k!,k,0,inf),simpsum=true)


$$\sum_{k=0}^{\infty }{\frac{x^{k}}{k!}}=\sum_{k=0}^{\infty }{\frac{x  ^{k}}{k!}}$$\>$limit(sum(x^k/k!,k,0,n),n,inf)


$$\lim_{n\rightarrow \infty }{\sum_{k=0}^{n}{\frac{x^{k}}{k!}}}$$\>function d(n) &= sum(1/(k^2-k),k,2,n); $'d(n)=d(n)


$$d\left(n\right)=\sum_{k=2}^{n}{\frac{1}{-k+k^2}}$$\>$d(10)=ev(d(10),simpsum=true)


$$\sum_{k=2}^{10}{\frac{1}{-k+k^2}}=\frac{9}{10}$$\>$d(100)=ev(d(100),simpsum=true)


$$\sum_{k=2}^{100}{\frac{1}{-k+k^2}}=\frac{99}{100}$$# Deret Taylor

Deret Taylor suatu fungsi f yang diferensiabel sampai tak hingga di
sekitar x=a adalah:


$$f(x) = \sum_{k=0}^\infty \frac{(x-a)^k f^{(k)}(a)}{k!}.$$\>$'e^x =taylor(exp(x),x,0,10) // deret Taylor e^x di sekitar x=0, sampai suku ke-11


$$e^{x}=1+x+\frac{x^2}{2}+\frac{x^3}{6}+\frac{x^4}{24}+\frac{x^5}{120  }+\frac{x^6}{720}+\frac{x^7}{5040}+\frac{x^8}{40320}+\frac{x^9}{  362880}+\frac{x^{10}}{3628800}$$\>$'log(x)=taylor(log(x),x,1,10)// deret log(x) di sekitar x=1


$$\log x=-1-\frac{\left(-1+x\right)^2}{2}+\frac{\left(-1+x\right)^3}{  3}-\frac{\left(-1+x\right)^4}{4}+\frac{\left(-1+x\right)^5}{5}-  \frac{\left(-1+x\right)^6}{6}+\frac{\left(-1+x\right)^7}{7}-\frac{  \left(-1+x\right)^8}{8}+\frac{\left(-1+x\right)^9}{9}-\frac{\left(-1  +x\right)^{10}}{10}+x$$---

---

---

# Visualisasi dan Perhitungan Geometri dengan EMT

Euler menyediakan beberapa fungsi untuk melakukan visualisasi dan
perhitungan geometri, baik secara numerik maupun analitik (seperti
biasanya tentunya, menggunakan Maxima). Fungsi-fungsi untuk
visualisasi dan perhitungan geometeri tersebut disimpan di dalam file
program "geometry.e", sehingga file tersebut harus dipanggil sebelum
menggunakan fungsi-fungsi atau perintah-perintah untuk geometri.


\>load geometry


    Numerical and symbolic geometry.

## Fungsi-fungsi Geometri

Fungsi-fungsi untuk Menggambar Objek Geometri:


  defaultd:=textheight()*1.5: nilai asli untuk parameter d  
  setPlotrange(x1,x2,y1,y2): menentukan rentang x dan y pada bidang  

koordinat


  setPlotRange(r): pusat bidang koordinat (0,0) dan batas-batas
sumbu-x dan y adalah -r sd r


  plotPoint (P, "P"): menggambar titik P dan diberi label "P"


  plotSegment (A,B, "AB", d): menggambar ruas garis AB, diberi label
"AB" sejauh d


  plotLine (g, "g", d): menggambar garis g diberi label "g" sejauh d


  plotCircle (c,"c",v,d): Menggambar lingkaran c dan diberi label "c"


  plotLabel (label, P, V, d): menuliskan label pada posisi P


Fungsi-fungsi Geometri Analitik (numerik maupun simbolik):


  turn(v, phi): memutar vektor v sejauh phi  
  turnLeft(v):   memutar vektor v ke kiri  
  turnRight(v):  memutar vektor v ke kanan  
  normalize(v): normal vektor v  
  crossProduct(v, w): hasil kali silang vektorv dan w.  
  lineThrough(A, B): garis melalui A dan B, hasilnya [a,b,c] sdh.  

ax+by=c.


  lineWithDirection(A,v): garis melalui A searah vektor v


  getLineDirection(g): vektor arah (gradien) garis g


  getNormal(g): vektor normal (tegak lurus) garis g


  getPointOnLine(g):  titik pada garis g


  perpendicular(A, g):  garis melalui A tegak lurus garis g


  parallel (A, g):  garis melalui A sejajar garis g


  lineIntersection(g, h):  titik potong garis g dan h


  projectToLine(A, g):   proyeksi titik A pada garis g


  distance(A, B):  jarak titik A dan B


  distanceSquared(A, B):  kuadrat jarak A dan B


  quadrance(A, B): kuadrat jarak A dan B


  areaTriangle(A, B, C):  luas segitiga ABC


  computeAngle(A, B, C):   besar sudut &lt;ABC


  angleBisector(A, B, C): garis bagi sudut &lt;ABC


  circleWithCenter (A, r): lingkaran dengan pusat A dan jari-jari r


  getCircleCenter(c):  pusat lingkaran c


  getCircleRadius(c):  jari-jari lingkaran c


  circleThrough(A,B,C):  lingkaran melalui A, B, C


  middlePerpendicular(A, B): titik tengah AB


  lineCircleIntersections(g, c): titik potong garis g dan lingkran c


  circleCircleIntersections (c1, c2):  titik potong lingkaran c1 dan
c2


  planeThrough(A, B, C):  bidang melalui titik A, B, C


Fungsi-fungsi Khusus Untuk Geometri Simbolik:


  getLineEquation (g,x,y): persamaan garis g dinyatakan dalam x dan y  
  getHesseForm (g,x,y,A): bentuk Hesse garis g dinyatakan dalam x dan  

y dengan titik A pada


  sisi positif (kanan/atas) garis


  quad(A,B): kuadrat jarak AB


  spread(a,b,c): Spread segitiga dengan panjang sisi-sisi a,b,c, yakni
sin(alpha)^2 dengan


  alpha sudut yang menghadap sisi a.


  crosslaw(a,b,c,sa): persamaan 3 quads dan 1 spread pada segitiga
dengan panjang sisi a, b, c.


  triplespread(sa,sb,sc): persamaan 3 spread sa,sb,sc yang memebntuk
suatu segitiga


  doublespread(sa): Spread sudut rangkap Spread 2*phi, dengan
sa=sin(phi)^2 spread a.


## Contoh 1: Luas, Lingkaran Luar, Lingkaran Dalam Segitiga

Untuk menggambar objek-objek geometri, langkah pertama adalah
menentukan rentang sumbu-sumbu koordinat. Semua objek geometri akan
digambar pada satu bidang koordinat, sampai didefinisikan bidang
koordinat yang baru.


\>setPlotRange(-0.5,2.5,-0.5,2.5); // mendefinisikan bidang koordinat baru 


Sekarang tetapkan tiga titik dan gambarkan.


\>A=[1,0]; plotPoint(A,"A"); // definisi dan gambar tiga titik

\>B=[0,1]; plotPoint(B,"B");

\>C=[2,2]; plotPoint(C,"C");


Lalu tiga segmen.


\>plotSegment(A,B,"c"); // c=AB

\>plotSegment(B,C,"a"); // a=BC

\>plotSegment(A,C,"b"); // b=AC


Fungsi geometri meliputi fungsi untuk membuat garis dan lingkaran.
Format garisnya adalah [a,b,c] yang mewakili garis dengan persamaan
ax+by=c.


\>lineThrough(B,C) // garis yang melalui B dan C


    [-1,  2,  2]

Hitung garis tegak lurus yang melalui A di BC.


\>h=perpendicular(A,lineThrough(B,C)); // garis h tegak lurus BC melalui A


Dan perpotongan h dengan BC.


\>D=lineIntersection(h,lineThrough(B,C)); // D adalah titik potong h dan BC


Buat plot.


\>plotPoint(D,value=1); // koordinat D ditampilkan

\>aspect(1); plotSegment(A,D): // tampilkan semua gambar hasil plot...()


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-842.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-842.png)

Hitung luas ABC:


$$L_{\triangle ABC}= \frac{1}{2}AD.BC.$$\>norm(A-D)\*norm(B-C)/2 // AD=norm(A-D), BC=norm(B-C)


    1.5

Bandingkan dengan rumus determinan.


\>areaTriangle(A,B,C) // hitung luas segitiga langusng dengan fungsi


    1.5

Cara lain menghitung luas segitigas ABC:


\>distance(A,D)\*distance(B,C)/2


    1.5

Sudut di C.


\>degprint(computeAngle(B,C,A))


    36°52'11.63''

Sekarang lingkaran luar segitiga.


\>c=circleThrough(A,B,C); // lingkaran luar segitiga ABC

\>R=getCircleRadius(c); // jari2 lingkaran luar 

\>O=getCircleCenter(c); // titik pusat lingkaran c 

\>plotPoint(O,"O"); // gambar titik "O"

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-844.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-844.png)

Tampilkan koordinat titik pusat dan jari-jari lingkaran luar.


\>O, R


    [1.16667,  1.16667]
    1.17851130198

Sekarang akan digambar lingkaran dalam segitiga ABC. Titik pusat
lingkaran dalam adalah titik potong garis-garis bagi sudut.


\>l=angleBisector(A,C,B); // garis bagi <ACB

\>g=angleBisector(C,A,B); // garis bagi <CAB

\>P=lineIntersection(l,g) // titik potong kedua garis bagi sudut


    [0.86038,  0.86038]

Tambahkan semua ke dalam plot.


\>color(5); plotLine(l); plotLine(g); color(1);  ...  
\>   // gambar kedua garis bagi sudut

\>plotPoint(P,"P"); // gambar titik potongnya

\>r=norm(P-projectToLine(P,lineThrough(A,B)))  ...  
\>   // jari-jari lingkaran dalam


    0.509653732104

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"):  ...  
\>   // gambar lingkaran dalam


    Syntax error in expression, or unfinished expression!
    Error in:
    ...  dalam segitiga ABC"):  // gambar lingkaran dalam ...
                                                         ^

## Latihan

1. Tentukan ketiga titik singgung lingkaran dalam dengan sisi-sisi
segitiga ABC.


2. Gambar segitiga dengan titik-titik sudut ketiga titik singgung
tersebut. Merupakan segitiga apakah itu?


3. Hitung luas segitiga tersebut.


4. Tunjukkan bahwa garis bagi sudut yang ke tiga juga melalui titik
pusat lingkaran dalam.


5. Gambar jari-jari lingkaran dalam.


6. Hitung luas lingkaran luar dan luas lingkaran dalam segitiga ABC.
Adakah hubungan antara luas kedua lingkaran tersebut dengan luas
segitiga ABC?


---

Nomor 1


\>pA=perpendicular(P,lineThrough(B,C));  ...  
\>   PA=lineIntersection(pA,lineThrough(B,C)), plotPoint(PA,value=1)


    [0.632456,  1.31623]

\>pB=perpendicular(P,lineThrough(A,C));  ...  
\>   PB=lineIntersection(pB,lineThrough(A,C)), plotPoint(PB,value=1)


    [1.31623,  0.632456]

\>pC=perpendicular(P,lineThrough(A,B));  ...  
\>   PC=lineIntersection(pC,lineThrough(A,B)), plotPoint(PC,value=1)


    [0.5,  0.5]

Nomor 2


\>plotSegment(PA,PB,"pc"), plotSegment(PA,PC,"pb"), plotSegment(PB,PC,"pa")


Nomor 3


\>areaTriangle(PA,PB,PC)


    0.324341649025

Nomor 4


\>k=angleBisector(A,B,C); color(5); plotLine(k); color(1);


Nomor 5


\>plotSegment(P,PA), plotSegment(P,PB), plotSegment(P,PC)


Nomor 6


\>Luar=pi\*R^2 //luas lingkaran luar segitiga ABC


    4.36332312999

\>Dalam=pi\*r^2 //luas lingkaran dalam segitiga ABC


    0.81601903655

\>areaTriangle(A,B,C) //luas segitiga ABC


    1.5

Dari perhitungan ini saya belum bisa mengetaui hubungan antara luas
kedua lingkaran tersebut dengan luas segitiga ABC.


# Contoh 2: Geometri Simbolik

Kita dapat menghitung geometri eksak dan simbolik menggunakan Maxima.


File geometri.e menyediakan fungsi yang sama (dan lebih banyak lagi)
di Maxima. Namun, sekarang kita dapat menggunakan perhitungan
simbolik.


\>A &= [1,0]; B &= [0,1]; C &= [2,2]; // menentukan tiga titik A, B, C


Fungsi untuk garis dan lingkaran berfungsi sama seperti fungsi Euler,
namun menyediakan komputasi simbolis.


\>c &= lineThrough(B,C) // c=BC


    
                                 [- 1, 2, 2]
    

Kita bisa memperoleh persamaan garis dengan mudah.


\>$getLineEquation(c,x,y), $solve(%,y) | expand // persamaan garis c


$$\left[ y=\frac{x}{2}+1 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-846.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-846.png)

\>$getLineEquation(lineThrough([x1,y1],[x2,y2]),x,y), $solve(%,y)  ...  
\>   // persamaan garis melalui(x1, y1) dan (x2, y2)


$$\left[ y=\frac{-\left({\it x_1}-x\right)\,{\it y_2}-\left(x-  {\it x_2}\right)\,{\it y_1}}{{\it x_2}-{\it x_1}} \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-848.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-848.png)

\>$getLineEquation(lineThrough(A,[x1,y1]),x,y)  ...  
\>   // persamaan garis melalui A dan (x1, y1)


$$\left({\it x_1}-1\right)\,y-x\,{\it y_1}=-{\it y_1}$$\>h &= perpendicular(A,lineThrough(B,C)) // h melalui A tegak lurus BC


    
                                  [2, 1, 2]
    

\>Q &= lineIntersection(c,h) // Q titik potong garis c=BC dan h


    
                                     2  6
                                    [-, -]
                                     5  5
    

\>$projectToLine(A,lineThrough(B,C)) // proyeksi A pada BC


$$\left[ \frac{2}{5} , \frac{6}{5} \right] $$\>$distance(A,Q) // jarak AQ


$$\frac{3}{\sqrt{5}}$$\>cc &= circleThrough(A,B,C); $cc  ...  
\>   // (titik pusat dan jari-jari) lingkaran melalui A, B, C


$$\left[ \frac{7}{6} , \frac{7}{6} , \frac{5}{3\,\sqrt{2}} \right] $$\>r&=getCircleRadius(cc); $r , $float(r) // tampilkan nilai jari-jari


$$1.178511301977579$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-854.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-854.png)

\>$computeAngle(A,C,B) // nilai <ACB


$$\arccos \left(\frac{4}{5}\right)$$\>$solve(getLineEquation(angleBisector(A,C,B),x,y),y)[1]  ...  
\>   // persamaan garis bagi <ACB


$$y=x$$\>P &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A)); $P,  ...  
\>   $float(P) // titik potong 2 garis bagi sudut


$$\left[ 0.8603796100280633 , 0.8603796100280633 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-858.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-858.png)

\>P() // hasilnya sama dengan perhitungan sebelumnya


    [0.86038,  0.86038]

## Perpotongan Garis dan Lingkaran

Tentu saja, kita juga bisa memotong garis dengan lingkaran, dan
lingkaran dengan lingkaran.


\>A &:= [1,0]; c=circleWithCenter(A,4);

\>B &:= [1,2]; C &:= [2,1]; l=lineThrough(B,C);

\>setPlotRange(5); plotCircle(c); plotLine(l);


Perpotongan garis dengan lingkaran menghasilkan dua titik dan jumlah
titik perpotongan.


\>{P1,P2,f}=lineCircleIntersections(l,c);

\>P1, P2, f


    [4.64575,  -1.64575]
    [-0.645751,  3.64575]
    2

\>plotPoint(P1); plotPoint(P2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-859.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-859.png)

Masih sama di Maxima.


\>c &= circleWithCenter(A,4) // lingkaran dengan pusat A jari-jari 4


    
                                  [1, 0, 4]
    

\>l &= lineThrough(B,C) // garis l melalui B dan C


    
                                  [1, 1, 3]
    

\>$lineCircleIntersections(l,c) | radcan,  ...  
\>   // titik potong garis l dan lingkaran c 


$$\left[ \left[ \sqrt{7}+2 , 1-\sqrt{7} \right]  , \left[ 2-\sqrt{7}   , \sqrt{7}+1 \right]  \right] $$Akan ditunjukkan bahwa sudut-sudut yang menghadap busur yang sama
adalah sama besar.


\>C=A+normalize([-2,-3])\*4; plotPoint(C); plotSegment(P1,C);  ...  
\>   plotSegment(P2,C);

\>degprint(computeAngle(P1,C,P2))


    69°17'42.68''

\>C=A+normalize([-4,-3])\*4; plotPoint(C); plotSegment(P1,C);  ...  
\>   plotSegment(P2,C);

\>degprint(computeAngle(P1,C,P2))


    69°17'42.68''

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-861.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-861.png)

## Garis Sumbu

Berikut adalah langkah-langkah menggambar garis sumbu ruas garis AB:


1. Gambar lingkaran dengan pusat A melalui B.


2. Gambar lingkaran dengan pusat B melalui A.


3. Tarik garis melalui kedua titik potong kedua lingkaran tersebut.
Garis ini merupakan garis sumbu (melalui titik tengah dan tegak lurus)
AB.


\>A=[2,2]; B=[-1,-2];

\>c1=circleWithCenter(A,distance(A,B));

\>c2=circleWithCenter(B,distance(A,B));

\>{P1,P2,f}=circleCircleIntersections(c1,c2);

\>l=lineThrough(P1,P2);

\>setPlotRange(5); plotCircle(c1); plotCircle(c2);

\>plotPoint(A); plotPoint(B); plotSegment(A,B); plotLine(l):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-862.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-862.png)

Selanjutnya kita melakukan hal yang sama di Maxima dengan koordinat
umum.


\>A &= [a1,a2]; B &= [b1,b2];

\>c1 &= circleWithCenter(A,distance(A,B));

\>c2 &= circleWithCenter(B,distance(A,B));

\>P &= circleCircleIntersections(c1,c2); P1 &= P[1]; P2 &= P[2];


Persamaan untuk perpotongan cukup rumit. Tapi kita bisa
menyederhanakannya jika kita mencari y.


\>g &= getLineEquation(lineThrough(P1,P2),x,y);

\>$solve(g,y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}  ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}   \right] $$Ini memang sama dengan garis tengah tegak lurus, yang dihitung dengan
cara yang sangat berbeda.


\>$solve(getLineEquation(middlePerpendicular(A,B),x,y),y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}  ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}   \right] $$\>h &=getLineEquation(lineThrough(A,B),x,y);

\>$solve(h,y)


$$\left[ y=\frac{\left({\it b_2}-{\it a_2}\right)\,x-{\it a_1}\,  {\it b_2}+{\it a_2}\,{\it b_1}}{{\it b_1}-{\it a_1}} \right] $$Perhatikan hasil kali gradien garis g dan h adalah:


$$\frac{-(b_1-a_1)}{(b_2-a_2)}\times \frac{(b_2-a_2)}{(b_1-a_1)} = -1.$$Artinya kedua garis tegak lurus.


# Contoh 3: Rumus Heron

Rumus Heron menyatakan bahwa luas segitiga dengan panjang sisi-sisi a,
b dan c adalah:


$$L = \sqrt{s(s-a)(s-b)(s-c)}\quad \text{ dengan } s=(a+b+c)/2,$$atau bisa ditulis dalam bentuk lain:


$$L = \frac{1}{4}\sqrt{(a+b+c)(b+c-a)(a+c-b)(a+b-c)}$$Untuk membuktikan hal ini kita misalkan C(0,0), B(a,0) dan A(x,y),
b=AC, c=AB. Luas segitiga ABC adalah


$$L_{\triangle ABC}=\frac{1}{2}a\times y.$$Nilai y didapat dengan menyelesaikan sistem persamaan:


$$x^2+y^2=b^2, \quad (x-a)^2+y^2=c^2.$$\>setPlotRange(-1,10,-1,8); plotPoint([0,0], "C(0,0)");  ...  
\>   plotPoint([5.5,0], "B(a,0)"); plotPoint([7.5,6], "A(x,y)");

\>plotSegment([0,0],[5.5,0], "a",25); plotSegment([5.5,0],[7.5,6],"c",15);  ...  
\>   plotSegment([0,0],[7.5,6],"b",25); //25,15,25 itu jarak label

\>plotSegment([7.5,6],[7.5,0],"t=y",25):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-871.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-871.png)

\>&assume(a\>0); sol &= solve([x^2+y^2=b^2,(x-a)^2+y^2=c^2],[x,y])


    
                                      []
    

Extrak solusi y.


\>ysol &= y with sol[2][2]; $'y=sqrt(factor(ysol^2))


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ysol &amp;= y with sol[2][2]; $'y=sqrt(factor(ysol^2)) ...
                            ^

Kita peroleh rumus Heron.


\>function H(a,b,c) &= sqrt(factor((ysol\*a/2)^2)); $'H(a,b,c)=H(a,b,c)


$$H\left(a , b , \left[ 1 , 0 , 4 \right] \right)=\frac{a\,\left|   {\it ysol}\right| }{2}$$\>$'Luas=H(2,5,6) // luas segitiga dengan panjang sisi-sisi 2, 5, 6


$${\it Luas}=\left| {\it ysol}\right| $$Tentu saja, setiap segitiga siku-siku adalah kasus yang terkenal.


\>H(3,4,5) //luas segitiga siku-siku dengan panjang sisi 3, 4, 5


    Variable or function ysol not found.
    Try "trace errors" to inspect local variables after errors.
    H:
        useglobal; return a*abs(ysol)/2 
    Error in:
    H(3,4,5) //luas segitiga siku-siku dengan panjang sisi 3, 4, 5 ...
            ^

Dan jelas juga bahwa ini adalah segitiga dengan luas maksimal dan
panjang kedua sisinya 3 dan 4.


\>aspect (1.5); plot2d(&H(3,4,x),1,7):  ...  
\>   // Kurva luas segitiga sengan panjang sisi 3, 4, x (1<= x <=7)


    Variable or function ysol not found.
    Error in expression: 3*abs(ysol)/2
     %ploteval:
        y0=f$(x[1],args());
    adaptiveevalone:
        s=%ploteval(g$,t;args());
    Try "trace errors" to inspect local variables after errors.
    plot2d:
        dw/n,dw/n^2,dw/n,auto;args());
    Syntax error in expression, or unfinished expression!

Kasus umum juga berhasil.


\>$solve(diff(H(a,b,c)^2,c)=0,c)


    Maxima said:
    diff: second argument must be a variable; found [1,0,4]
     -- an error. To debug this try: debugmode(true);
    
    Error in:
     $solve(diff(H(a,b,c)^2,c)=0,c) ...
                                  ^

Sekarang mari kita cari himpunan semua titik di mana b+c=d untuk suatu
konstanta d. Diketahui bahwa ini adalah elips.


\>s1 &= subst(d-c,b,sol[2]); $s1


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    s1 &amp;= subst(d-c,b,sol[2]); $s1 ...
                             ^

Buat fungsi dari ini.


\>function fx(a,c,d) &= rhs(s1[1]); $fx(a,c,d),  ...  
\>  
$$0$$\>function fy(a,c,d) &= rhs(s1[2]); $fy(a,c,d)


$$0$$Sekarang kita bisa menggambar setnya. Sisi b bervariasi dari 1 sampai
4. Diketahui bahwa kita memperoleh elips.


\>aspect(1); plot2d(&fx(3,x,5),&fy(3,x,5),xmin=1,xmax=4,square=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-876.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-876.png)

Kita dapat memeriksa persamaan umum elips ini, yaitu.


$$\frac{(x-x_m)^2}{u^2}+\frac{(y-y_m)}{v^2}=1,$$dimana (xm,ym) adalah pusat, u dan v adalah setengah sumbu.


\>$ratsimp((fx(a,c,d)-a/2)^2/u^2+fy(a,c,d)^2/v^2 with [u=d/2,v=sqrt(d^2-a^2)/2])


$$\frac{a^2}{d^2}$$Kita melihat bahwa tinggi dan luas segitiga adalah maksimal untuk x=0.
Jadi luas segitiga dengan a+b+c=d adalah maksimal jika segitiga
tersebut sama sisi. Kita ingin memperolehnya secara analitis.


\>eqns &= [diff(H(a,b,d-(a+b))^2,a)=0,diff(H(a,b,d-(a+b))^2,b)=0]; $eqns


$$\left[ \frac{a\,{\it ysol}^2}{2}=0 , 0=0 \right] $$Kita mendapatkan nilai minimum yang dimiliki oleh segitiga dengan
salah satu sisinya 0, dan solusinya a=b=c=d/3.


\>$solve(eqns,[a,b])


$$\left[ \left[ a=0 , b={\it \%r_1} \right]  \right] $$Ada juga metode Lagrange, yang memaksimalkan H(a,b,c)^2 terhadap
a+b+d=d.


\>&solve([diff(H(a,b,c)^2,a)=la,diff(H(a,b,c)^2,b)=la, ...  
\>      diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la])


    Maxima said:
    diff: second argument must be a variable; found [1,0,4]
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ... la,    diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la]) ...
                                                         ^

Kita bisa membuat plotnya.


Pertama atur titik di Maxima.


\>A &= at([x,y],sol[2]); $A


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    A &amp;= at([x,y],sol[2]); $A ...
                         ^

\>B &= [0,0]; $B, C &= [a,0]; $C


$$\left[ a , 0 \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-882.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-882.png)

Kemudian atur rentang plot, dan plot titik-titiknya.


\>setPlotRange(0,5,-2,3); ...  
\>   a=4; b=3; c=2; ...  
\>   plotPoint(mxmeval("B"),"B"); plotPoint(mxmeval("C"),"C"); ...  
\>   plotPoint(mxmeval("A"),"A"):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    ... otPoint(mxmeval("C"),"C"); plotPoint(mxmeval("A"),"A"): ...
                                                         ^

Plot segmennya.


\>plotSegment(mxmeval("A"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("A")):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    plotSegment(mxmeval("A"),mxmeval("C")); plotSegment(mxmeval("B ...
                            ^

Hitung garis tengah tegak lurus di Maxima.


\>h &= middlePerpendicular(A,B); g &= middlePerpendicular(B,C);


Dan pusat lingkarannya.


\>U &= lineIntersection(h,g);


Kita mendapatkan rumus jari-jari lingkaran luar.


\>&assume(a\>0,b\>0,c\>0); $distance(U,B) | radcan


$$\frac{\sqrt{{\it a_2}^2+{\it a_1}^2}\,\sqrt{{\it a_2}^2+{\it a_1}^2  -2\,a\,{\it a_1}+a^2}}{2\,\left| {\it a_2}\right| }$$Mari kita tambahkan ini ke dalam plot.


\>plotPoint(U()); ...  
\>   plotCircle(circleWithCenter(mxmeval("U"),mxmeval("distance(U,C)"))):


    Variable a2 not found!
    Use global variables or parameters for string evaluation.
    Error in ^
    Error in expression: [a/2,(a2^2+a1^2-a*a1)/(2*a2)]
    Error in:
    plotPoint(U()); plotCircle(circleWithCenter(mxmeval("U"),mxmev ...
                 ^

Dengan menggunakan geometri, kita memperoleh rumus sederhana


$$\frac{a}{\sin(\alpha)}=2r$$untuk radius. Kita bisa cek, apakah ini benar adanya pada Maxima.
Maxima akan memfaktorkan ini hanya jika kita mengkuadratkannya.


\>$c^2/sin(computeAngle(A,B,C))^2  | factor


$$\left[ \frac{{\it a_2}^2+{\it a_1}^2}{{\it a_2}^2} , 0 , \frac{16\,  \left({\it a_2}^2+{\it a_1}^2\right)}{{\it a_2}^2} \right] $$# Contoh 4: Garis Euler dan Parabola

Garis Euler adalah garis yang ditentukan dari sembarang segitiga yang
tidak sama sisi. Merupakan garis tengah segitiga, dan melewati
beberapa titik penting yang ditentukan dari segitiga, antara lain
orthocenter, circumcenter, centroid, titik Exeter dan pusat lingkaran
sembilan titik segitiga.


Untuk demonstrasinya, kita menghitung dan memplot garis Euler dalam
sebuah segitiga.


Pertama, kita mendefinisikan sudut-sudut segitiga di Euler. Kami
menggunakan definisi, yang terlihat dalam ekspresi simbolik.


\>A::=[-1,-1]; B::=[2,0]; C::=[1,2];


Untuk memplot objek geometris, kita menyiapkan area plot, dan
menambahkan titik ke dalamnya. Semua plot objek geometris ditambahkan
ke plot saat ini.


\>setPlotRange(3); plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C");


Kita juga bisa menjumlahkan sisi-sisi segitiga.


\>plotSegment(A,B,""); plotSegment(B,C,""); plotSegment(C,A,""):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-886.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-886.png)

Berikut luas segitiga menggunakan rumus determinan. Tentu saja kami
harus mengambil nilai absolut dari hasil ini.


\>$areaTriangle(A,B,C)


$$-\frac{7}{2}$$Kita dapat menghitung koefisien dari sisi c.


\>c &= lineThrough(A,B)


    
                                [- 1, 3, - 2]
    

Dan juga mendapatkan formula untuk baris ini.


\>$getLineEquation(c,x,y)


$$3\,y-x=-2$$Untuk bentuk Hesse, kita perlu menentukan sebuah titik, sehingga titik
tersebut berada di sisi positif dari bentuk Hesse. Memasukkan titik
tersebut akan menghasilkan jarak positif ke garis.


\>$getHesseForm(c,x,y,C), $at(%,[x=C[1],y=C[2]])


$$\frac{7}{\sqrt{10}}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-890.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-890.png)

Sekarang kita menghitung keliling ABC.


\>LL &= circleThrough(A,B,C); $getCircleEquation(LL,x,y)


$$\left(y-\frac{5}{14}\right)^2+\left(x-\frac{3}{14}\right)^2=\frac{  325}{98}$$\>O &= getCircleCenter(LL); $O


$$\left[ \frac{3}{14} , \frac{5}{14} \right] $$Plot lingkaran dan pusatnya. Cu dan U adalah simbolik. Kami
mengevaluasi ekspresi ini untuk Euler.


\>plotCircle(LL()); plotPoint(O(),"O"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-893.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-893.png)

Kita dapat menghitung perpotongan ketinggian di ABC (pusat
ortosentrum) secara numerik dengan perintah berikut ini.


\>H &= lineIntersection(perpendicular(A,lineThrough(C,B)),...  
\>     perpendicular(B,lineThrough(A,C))); $H


$$\left[ \frac{11}{7} , \frac{2}{7} \right] $$Sekarang kita dapat menghitung garis Euler dari segitiga tersebut.


\>el &= lineThrough(H,O); $getLineEquation(el,x,y)


$$-\frac{19\,y}{14}-\frac{x}{14}=-\frac{1}{2}$$Tambahkan ke plot kita.


\>plotPoint(H(),"H"); plotLine(el(),"Garis Euler"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-896.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-896.png)

Pusat gravitasi harus berada pada garis ini.


\>M &= (A+B+C)/3; $getLineEquation(el,x,y) with [x=M[1],y=M[2]]


$$-\frac{1}{2}=-\frac{1}{2}$$\>plotPoint(M(),"M"): // titik berat


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-898.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-898.png)

Teori mengatakan bahwa MH = 2*MO. Kita perlu menyederhanakan dengan
radcan untuk mencapai hal ini.


\>$distance(M,H)/distance(M,O)|radcan


$$2$$Fungsi-fungsi ini juga mencakup fungsi untuk sudut.


\>$computeAngle(A,C,B), degprint(%())


$$\arccos \left(\frac{4}{\sqrt{5}\,\sqrt{13}}\right)$$    60°15'18.43''

Persamaan untuk bagian tengah lingkaran tidak terlalu bagus.


\>Q &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A))|radcan; $Q


$$\left[ \frac{\left(2^{\frac{3}{2}}+1\right)\,\sqrt{5}\,\sqrt{13}-15  \,\sqrt{2}+3}{14} , \frac{\left(\sqrt{2}-3\right)\,\sqrt{5}\,\sqrt{  13}+5\,2^{\frac{3}{2}}+5}{14} \right] $$Mari kita hitung juga ekspresi untuk jari-jari lingkaran yang
tertulis.


\>r &= distance(Q,projectToLine(Q,lineThrough(A,B)))|ratsimp; $r


$$\frac{\sqrt{\left(-41\,\sqrt{2}-31\right)\,\sqrt{5}\,\sqrt{13}+115  \,\sqrt{2}+614}}{7\,\sqrt{2}}$$\>LD &=  circleWithCenter(Q,r); // Lingkaran dalam


Mari kita tambahkan ini ke dalam plot.


\>color(5); plotCircle(LD()):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-903.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-903.png)

## Parabola

Selanjutnya akan dicari persamaan tempat kedudukan titik-titik yang
berjarak sama ke titik C dan ke garis AB.


\>p &= getHesseForm(lineThrough(A,B),x,y,C)-distance([x,y],C); $p='0


$$\frac{3\,y-x+2}{\sqrt{10}}-\sqrt{\left(2-y\right)^2+\left(1-x  \right)^2}=0$$Persamaan tersebut dapat digambar menjadi satu dengan gambar
sebelumnya.


\>plot2d(p,level=0,add=1,contourcolor=6):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-905.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-905.png)

Ini seharusnya merupakan suatu fungsi, tetapi solver default Maxima
hanya bisa menemukan solusinya jika kita mengkuadratkan persamaannya.
Akibatnya, kita mendapatkan solusi palsu.


\>akar &= solve(getHesseForm(lineThrough(A,B),x,y,C)^2-distance([x,y],C)^2,y)


    
            [y = - 3 x - sqrt(70) sqrt(9 - 2 x) + 26, 
                                  y = - 3 x + sqrt(70) sqrt(9 - 2 x) + 26]
    

Solusi pertama adalah


$$y=-3\,x-\sqrt{70}\,\sqrt{9-2\,x}+26$$Menambahkan solusi pertama ke dalam plot menunjukkan, bahwa ini memang
jalur yang kita cari. Teori mengatakan bahwa ini adalah sebuah
parabola yang diputar.


\>plot2d(&rhs(akar[1]),add=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-907.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-907.png)

\>function g(x) &= rhs(akar[1]); $'g(x)= g(x)  ...  
\>   // fungsi yang mendefinisikan kurva di atas

\>T &=[-1, g(-1)]; // ambil sebarang titik pada kurva tersebut


    Maxima said:
    incorrect syntax: T is not an infix operator
    'g(x)= g(x)  T 
                 ^
    
    Error in:
    T &amp;=[-1, g(-1)]; // ambil sebarang titik pada kurva tersebut ...
                   ^

\>dTC &= distance(T,C); $fullratsimp(dTC), $float(%) // jarak T ke C


$$\sqrt{2.0\,T^2-6.0\,T+5.0}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-909.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-909.png)

\>U &= projectToLine(T,lineThrough(A,B)); $U // proyeksi T pada garis AB 


$$\left[ \frac{3\,\left[ 3 , 1 \right] \cdot T+2}{10} , \frac{\left[   3 , 1 \right] \cdot T-6}{10} \right] $$\>dU2AB &= distance(T,U); $fullratsimp(dU2AB), $float(%) // jatak T ke AB


$$0.3162277660168379\,\sqrt{20.0\,T^2+\left(8.0-8.0\,\left[ 3.0 , 1.0   \right] \cdot T\right)\,T+\left(\left[ 3.0 , 1.0 \right] \cdot T  \right)^2+4.0}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-912.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-912.png)

Ternyata jarak T ke C sama dengan jarak T ke AB. Coba Anda pilih titik
T yang lain dan ulangi perhitungan-perhitungan di atas untuk
menunjukkan bahwa hasilnya juga sama.


# Contoh 5: Trigonometri Rasional

Ini terinspirasi dari sebuah ceramah N.J. Wildberger. Dalam bukunya
"Proporsi Ilahi", Wildberger mengusulkan untuk mengganti gagasan
klasik tentang jarak dan sudut dengan kuadransi dan penyebaran. Dengan
menggunakan ini, memang memungkinkan untuk menghindari fungsi
trigonometri dalam banyak contoh, dan tetap "rasional".


Berikut ini, saya akan memperkenalkan konsep-konsep tersebut, dan
memecahkan beberapa masalah. Saya menggunakan komputasi simbolik
Maxima di sini, yang menyembunyikan keuntungan utama dari trigonometri
rasional yaitu komputasi dapat dilakukan dengan kertas dan pensil
saja. Anda dipersilakan untuk memeriksa hasilnya tanpa komputer.


Intinya adalah bahwa komputasi rasional simbolik sering kali
memberikan hasil yang sederhana. Sebaliknya, trigonometri klasik
menghasilkan hasil trigonometri yang rumit, yang dievaluasi dengan
pendekatan numerik saja.


\>load geometry;


Untuk pengenalan pertama, kita menggunakan segitiga persegi panjang
dengan proporsi Mesir yang terkenal 3, 4, dan 5. Perintah berikut ini
adalah perintah Euler untuk memplot geometri bidang yang terdapat pada
file Euler "geometry.e".


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg(30);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-913.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-913.png)

Tentu saja,


$$\sin(w_a)=\frac{a}{c},$$di mana wa adalah sudut di A. Cara biasa untuk menghitung sudut ini,
adalah dengan mengambil kebalikan dari fungsi sinus. Hasilnya adalah
sudut yang tidak dapat dicerna, yang hanya dapat dicetak kira-kira.


\>wa := arcsin(3/5); degprint(wa)


    36°52'11.63''

Trigonometri rasional mencoba menghindari hal ini.


Gagasan pertama trigonometri rasional adalah kuadrat, yang
menggantikan jarak. Sebenarnya, ini hanyalah jarak yang dikuadratkan.
Berikut ini, a, b, dan c menunjukkan kuadran sisi-sisinya.


Teorema Pythogoras menjadi a + b = c.


\>a &= 3^2; b &= 4^2; c &= 5^2; &a+b=c


    
                                   25 = 25
    

Gagasan kedua dari trigonometri rasional adalah penyebaran. Penyebaran
mengukur bukaan di antara garis-garis. Ini adalah 0, jika
garis-garisnya sejajar, dan 1, jika garis-garisnya persegi panjang.
Ini adalah kuadrat dari sinus sudut antara dua garis.


Penyebaran garis AB dan AC pada gambar di atas didefinisikan sebagai


$$s_a = \sin(\alpha)^2 = \frac{a}{c},$$di mana a dan c adalah kuadran dari segitiga persegi panjang dengan
satu sudut di A.


\>sa &= a/c; $sa


$$\frac{9}{25}$$Tentu saja, hal ini lebih mudah dihitung daripada sudut. Tetapi Anda
kehilangan sifat bahwa sudut dapat ditambahkan dengan mudah.


Tentu saja, kita bisa mengonversi nilai perkiraan kita untuk sudut wa
ke sprad, dan mencetaknya sebagai pecahan.


\>fracprint(sin(wa)^2)


    9/25

Hukum kosinus trgonometri klasik diterjemahkan ke dalam " cross law "
berikut ini.


$$(c+b-a)^2 = 4 b c \, (1-s_a)$$Di sini a, b, dan c adalah kuadran dari sisi-sisi segitiga, dan sa
adalah penyebaran di sudut A. Sisi a, seperti biasa, berlawanan dengan
sudut A.


Hukum-hukum ini diimplementasikan dalam file geometri.e yang kita
masukkan ke dalam Euler.


\>$crosslaw(aa,bb,cc,saa)


$$\left[ \left({\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left(  {\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left({\it bb}-{\it aa}+  \frac{5}{3\,\sqrt{2}}\right)^2 \right] =\left[ \frac{14\,{\it bb}\,  \left(1-{\it saa}\right)}{3} , \frac{14\,{\it bb}\,\left(1-{\it saa}  \right)}{3} , \frac{5\,2^{\frac{3}{2}}\,{\it bb}\,\left(1-{\it saa}  \right)}{3} \right] $$Dalam kasus ini, kita mendapatkan


\>$crosslaw(a,b,c,sa)


$$1024=1024$$Mari kita gunakan crosslaw ini untuk mencari sebaran di A. Untuk
melakukannya, kita buat crosslaw untuk kuadran a, b, dan c, dan
selesaikan untuk sebaran sa yang tidak diketahui.


Anda bisa melakukan ini dengan tangan dengan mudah, tapi saya
menggunakan Maxima. Tentu saja, kita mendapatkan hasil yang sudah kita
dapatkan.


\>$crosslaw(a,b,c,x), $solve(%,x)


$$\left[ x=\frac{9}{25} \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-921.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-921.png)

Kita sudah mengetahui hal ini. Definisi penyebaran adalah kasus khusus
dari crosslaw.


Kita juga dapat menyelesaikannya untuk a, b, c secara umum. Hasilnya
adalah sebuah rumus yang menghitung penyebaran sudut sebuah segitiga
dengan kuadran ketiga sisinya.


\>$solve(crosslaw(aa,bb,cc,x),x)


$$\left[ \left[ \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,  {\it aa}-84\right)\,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} ,   \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,{\it aa}-84\right)  \,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} , \frac{15\,2^{\frac{  5}{2}}\,{\it bb}\,x+18\,{\it bb}^2+\left(-36\,{\it aa}-15\,2^{\frac{  3}{2}}\right)\,{\it bb}+18\,{\it aa}^2-15\,2^{\frac{3}{2}}\,{\it aa}  +25}{18} \right] =0 \right] $$Kita dapat membuat sebuah fungsi dari hasil tersebut. Fungsi seperti
itu sudah didefinisikan dalam file geometry.e dari Euler.


\>$spread(a,b,c)


$$\frac{9}{25}$$Sebagai contoh, kita dapat menggunakannya untuk menghitung sudut
segitiga dengan sisi


$$a, \quad a, \quad \frac{4a}{7}$$Hasilnya adalah rasional, yang tidak mudah didapat jika kita
menggunakan trigonometri klasik.


\>$spread(a,a,4\*a/7)


$$\frac{6}{7}$$Ini adalah sudut dalam derajat.


\>degprint(arcsin(sqrt(6/7)))


    67°47'32.44''

## Contoh Lain

Sekarang, mari kita coba contoh yang lebih lanjut.


Kita tentukan tiga sudut segitiga sebagai berikut.


\>A&:=[1,2]; B&:=[4,3]; C&:=[0,4]; ...  
\>   setPlotRange(-1,5,1,7); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-926.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-926.png)

Dengan menggunakan Pythogoras, mudah untuk menghitung jarak antara dua
titik. Pertama-tama saya menggunakan jarak fungsi dari file Euler
untuk geometri. Jarak fungsi menggunakan geometri klasik.


\>$distance(A,B)


$$\sqrt{10}$$Euler juga memiliki fungsi untuk kuadranan antara dua titik.


Pada contoh berikut, karena c+b bukan a, maka segitiga tersebut tidak
berbentuk persegi panjang.


\>c &= quad(A,B); $c, b &= quad(A,C); $b, a &= quad(B,C); $a,


$$17$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-929.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-929.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-930.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-930.png)

Pertama, mari kita menghitung sudut tradisional. Fungsi computeAngle
menggunakan metode yang biasa berdasarkan hasil kali titik dari dua
vektor. Hasilnya adalah beberapa perkiraan titik mengambang.


$$A=<1,2>\quad B=<4,3>,\quad C=<0,4>$$$$\mathbf{a}=C-B=<-4,1>,\quad \mathbf{c}=A-B=<-3,-1>,\quad \beta=\angle ABC$$$$\mathbf{a}.\mathbf{c}=|\mathbf{a}|.|\mathbf{c}|\cos \beta$$$$\cos \angle ABC =\cos\beta=\frac{\mathbf{a}.\mathbf{c}}{|\mathbf{a}|.|\mathbf{c}|}=\frac{12-1}{\sqrt{17}\sqrt{10}}=\frac{11}{\sqrt{17}\sqrt{10}}$$\>wb &= computeAngle(A,B,C); $wb, $(wb/pi\*180)()


$$\arccos \left(\frac{11}{\sqrt{10}\,\sqrt{17}}\right)$$    32.4711922908

Dengan menggunakan pensil dan kertas, kita dapat melakukan hal yang
sama dengan hukum silang. Kita masukkan kuadran a, b, dan c ke dalam
hukum silang dan selesaikan untuk x.


\>$crosslaw(a,b,c,x), $solve(%,x), //(b+c-a)^=4b.c(1-x)


$$\left[ x=\frac{49}{50} \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-937.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-937.png)

Itulah yang dilakukan oleh fungsi spread yang didefinisikan dalam
"geometry.e".


\>sb &= spread(b,a,c); $sb


$$\frac{49}{170}$$Maxima mendapatkan hasil yang sama dengan menggunakan trigonometri
biasa, jika kita memaksakannya. Ia menyelesaikan suku sin(arccos(...))
menjadi hasil pecahan. Sebagian besar siswa tidak dapat melakukan ini.


\>$sin(computeAngle(A,B,C))^2


$$\frac{49}{170}$$Setelah kita memiliki penyebaran di B, kita dapat menghitung tinggi ha
di sisi a. Ingatlah bahwa


$$s_b = \frac{h_a}{c}$$menurut definisi.


\>ha &= c\*sb; $ha


$$\frac{49}{17}$$Gambar berikut ini dibuat dengan program geometri C.a.R., yang dapat
menggambar kuadran dan penyebaran.


image: (20) Rational_Geometry_CaR.png


Menurut definisi, panjang ha adalah akar kuadrat dari kuadrannya.


\>$sqrt(ha)


$$\frac{7}{\sqrt{17}}$$Sekarang kita dapat menghitung luas segitiga. Jangan lupa, bahwa kita
berurusan dengan kuadran!


\>$sqrt(ha)\*sqrt(a)/2


$$\frac{7}{2}$$Rumus penentu yang biasa menghasilkan hasil yang sama.


\>$areaTriangle(B,A,C)


$$\frac{7}{2}$$## Rumus Heron (bangau)

Sekarang, mari kita selesaikan masalah ini secara umum!


\>&remvalue(a,b,c,sb,ha);


Pertama-tama kita menghitung penyebaran di B untuk segitiga dengan
sisi a, b, dan c. Kemudian kita menghitung luas kuadrat ("quadrea"?),
memfaktorkannya dengan Maxima, dan kita mendapatkan rumus Heron yang
terkenal.


Memang, hal ini sulit dilakukan dengan pensil dan kertas.


\>$spread(b^2,c^2,a^2), $factor(%\*c^2\*a^2/4)


$$\frac{\left(-c+b+a\right)\,\left(c-b+a\right)\,\left(c+b-a\right)\,  \left(c+b+a\right)}{16}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-946.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-946.png)

## Aturan Triple Spread

Kerugian dari spread adalah bahwa mereka tidak lagi hanya menambahkan
sudut seperti.


Namun, tiga spread dari sebuah segitiga memenuhi aturan "triple
spread" berikut ini.


\>&remvalue(sa,sb,sc); $triplespread(sa,sb,sc)


$$\left({\it sc}+{\it sb}+{\it sa}\right)^2=2\,\left({\it sc}^2+  {\it sb}^2+{\it sa}^2\right)+4\,{\it sa}\,{\it sb}\,{\it sc}$$Aturan ini berlaku untuk tiga sudut yang berjumlah 180°.


$$\alpha+\beta+\gamma=\pi$$Karena spread dari


$$\alpha, \pi-\alpha$$adalah sama, aturan triple spread juga benar, jika


$$\alpha+\beta=\gamma$$Karena penyebaran sudut negatif adalah sama, aturan triple spread juga
berlaku, jika


$$\alpha+\beta+\gamma=0$$Sebagai contoh, kita bisa menghitung penyebaran sudut 60°. Ini adalah
3/4. Namun, persamaan ini memiliki solusi kedua, di mana semua
penyebarannya adalah 0.


\>$solve(triplespread(x,x,x),x)


$$\left[ x=\frac{3}{4} , x=0 \right] $$Penyebaran 90° jelas adalah 1. Jika dua sudut ditambahkan ke 90°,
penyebarannya akan menyelesaikan persamaan penyebaran tiga dengan a,
b, 1. Dengan perhitungan berikut, kita mendapatkan a + b = 1.


\>$triplespread(x,y,1), $solve(%,x)


$$\left[ x=1-y \right] $$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-954.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-954.png)

Karena penyebaran 180°-t sama dengan penyebaran t, rumus penyebaran
tiga kali lipat juga berlaku, jika satu sudut adalah jumlah atau
selisih dari dua sudut lainnya.


Jadi kita dapat menemukan penyebaran sudut dua kali lipat. Perhatikan
bahwa ada dua solusi lagi. Kita jadikan ini sebuah fungsi.


\>$solve(triplespread(a,a,x),x), function doublespread(a) &= factor(rhs(%[1]))


$$\left[ x=4\,a-4\,a^2 , x=0 \right] $$    
                                - 4 (a - 1) a
    

## Pembagi Sudut

Ini adalah situasi yang sudah kita ketahui.


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-956.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-956.png)

Mari kita hitung panjang garis bagi sudut di A. Tetapi kita ingin
menyelesaikannya untuk a, b, c secara umum.


\>&remvalue(a,b,c);


Jadi, pertama-tama kita menghitung penyebaran sudut yang dibelah dua
di A, menggunakan rumus penyebaran tiga.


Masalah dengan rumus ini muncul lagi. Rumus ini memiliki dua solusi.
Kita harus memilih salah satu yang benar. Solusi lainnya mengacu pada
sudut terbagi dua 180°-wa.


\>$triplespread(x,x,a/(a+b)), $solve(%,x), sa2 &= rhs(%[1]); $sa2


$$\frac{-\sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a}$$![images/EMT_Annisa%20Nur%20Rohmah_22305141031-958.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-958.png)

![images/EMT_Annisa%20Nur%20Rohmah_22305141031-959.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-959.png)

Mari kita periksa persegi panjang Mesir.


\>$sa2 with [a=3^2,b=4^2]


$$\frac{1}{10}$$Kita bisa mencetak sudut dalam Euler, setelah mentransfer penyebaran
ke radian.


\>wa2 := arcsin(sqrt(1/10)); degprint(wa2)


    18°26'5.82''

Titik P adalah perpotongan garis bagi sudut dengan sumbu y.


\>P := [0,tan(wa2)\*4]


    [0,  1.33333]

\>plotPoint(P,"P"); plotSegment(A,P):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-961.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-961.png)

Mari kita periksa sudut-sudutnya dalam contoh spesifik kita.


\>computeAngle(C,A,P), computeAngle(P,A,B)


    0.321750554397
    0.321750554397

Sekarang kita hitung panjang garis bagi AP.


Kita menggunakan teorema sinus dalam segitiga APC. Teorema ini
menyatakan bahwa


$$\frac{BC}{\sin(w_a)} = \frac{AC}{\sin(w_b)} = \frac{AB}{\sin(w_c)}$$berlaku untuk semua segitiga. Kuadratkan, ini diterjemahkan ke dalam
apa yang disebut "hukum penyebaran"


$$\frac{a}{s_a} = \frac{b}{s_b} = \frac{c}{s_b}$$di mana a, b, c menunjukkan qudrance.


Karena spread CPA adalah 1-sa2, kita mendapatkan bisa/1 = b/(1-sa2)
dan bisa menghitung bisa (kuadransi dari garis-bagi sudut).


\>&factor(ratsimp(b/(1-sa2))); bisa &= %; $bisa


$$\frac{2\,b\,\left(b+a\right)}{\sqrt{b}\,\sqrt{b+a}+b+a}$$Mari kita periksa rumus ini untuk nilai-nilai Mesir kita.


\>sqrt(mxmeval("at(bisa,[a=3^2,b=4^2])")), distance(A,P)


    4.21637021356
    4.21637021356

Kita juga dapat menghitung P dengan menggunakan rumus penyebaran.


\>py&=factor(ratsimp(sa2\*bisa)); $py


$$-\frac{b\,\left(\sqrt{b}\,\sqrt{b+a}-b-a\right)}{\sqrt{b}\,\sqrt{b+  a}+b+a}$$Nilainya sama dengan yang kita dapatkan dengan rumus trigonometri.


\>sqrt(mxmeval("at(py,[a=3^2,b=4^2])"))


    1.33333333333

## Sudut Akor

Lihatlah situasi berikut ini.


\>setPlotRange(1.2); ...  
\>   color(1); plotCircle(circleWithCenter([0,0],1)); ...  
\>   A:=[cos(1),sin(1)]; B:=[cos(2),sin(2)]; C:=[cos(6),sin(6)]; ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   color(3); plotSegment(A,B,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   color(1); O:=[0,0];  plotPoint(O,"0"); ...  
\>   plotSegment(A,O); plotSegment(B,O); plotSegment(C,O,"r"); ...  
\>   insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-966.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-966.png)

Kita dapat menggunakan Maxima untuk menyelesaikan rumus penyebaran
tiga untuk sudut-sudut di pusat O untuk r. Dengan demikian kita
mendapatkan rumus untuk jari-jari kuadrat dari pericircle dalam hal
kuadran sisi-sisinya.


Kali ini, Maxima menghasilkan beberapa angka nol yang rumit, yang kita
abaikan.


\>&remvalue(a,b,c,r); // hapus nilai-nilai sebelumnya untuk perhitungan baru

\>rabc &= rhs(solve(triplespread(spread(b,r,r),spread(a,r,r), ...  
\>   spread(c,r,r)),r)[4]); $rabc


$$-\frac{a\,b\,c}{c^2-2\,b\,c+a\,\left(-2\,c-2\,b\right)+b^2+a^2}$$Kita dapat menjadikannya sebuah fungsi Euler.


\>function periradius(a,b,c) &= rabc;


Mari kita periksa hasilnya untuk poin A, B, C.


\>a:=quadrance(B,C); b:=quadrance(A,C); c:=quadrance(A,B);


Radiusnya memang 1.


\>periradius(a,b,c)


    1

Faktanya adalah, bahwa penyebaran CBA hanya bergantung pada b dan c.
Ini adalah teorema sudut akor.


\>$spread(b,a,c)\*rabc | ratsimp


$$\frac{b}{4}$$Faktanya, penyebarannya adalah b/(4r), dan kita melihat bahwa sudut
chord b adalah setengah dari sudut tengah.


\>$doublespread(b/(4\*r))-spread(b,r,r) | ratsimp


$$0$$# Contoh 6: Jarak Minimal pada Bidang

## Keterangan awal

Fungsi yang, pada sebuah titik M pada bidang, menetapkan jarak AM
antara titik tetap A dan M, memiliki garis-garis tingkat yang cukup
sederhana: lingkaran yang berpusat di A.


\>&remvalue();

\>A=[-1,-1];

\>function d1(x,y):=sqrt((x-A[1])^2+(y-A[2])^2)

\>fcontour("d1",xmin=-2,xmax=0,ymin=-2,ymax=0,hue=1, ...  
\>   title="If you see ellipses, please set your window square"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-970.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-970.png)

dan grafiknya juga cukup sederhana: bagian atas kerucut:


\>plot3d("d1",xmin=-2,xmax=0,ymin=-2,ymax=0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-971.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-971.png)

Tentu saja nilai minimum 0 diperoleh dalam A.


## Dua titik

Sekarang kita lihat fungsi MA+MB di mana A dan B adalah dua titik
(tetap). Ini adalah "fakta yang sudah diketahui" bahwa kurva-kurva
tingkat adalah elips, titik fokusnya adalah A dan B; kecuali AB
minimum yang konstan pada segmen [AB]:v


\>B=[1,-1];

\>function d2(x,y):=d1(x,y)+sqrt((x-B[1])^2+(y-B[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-972.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-972.png)

Grafiknya lebih menarik:


\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-973.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-973.png)

Pembatasan pada garis (AB) lebih terkenal:


\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-974.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-974.png)

## Tiga poin

Sekarang, hal-hal menjadi kurang sederhana: Hal ini sedikit kurang
dikenal bahwa MA+MB+MC mencapai minimumnya pada satu titik di bidang,
tetapi untuk menentukannya tidak sesederhana itu:


1) Jika salah satu sudut segitiga ABC lebih dari 120° (katakanlah di
A), maka minimum dicapai pada titik ini (katakanlah AB+AC).


Contoh:


\>C=[-4,1];

\>function d3(x,y):=d2(x,y)+sqrt((x-C[1])^2+(y-C[2])^2)

\>plot3d("d3",xmin=-5,xmax=3,ymin=-4,ymax=4);

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-975.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-975.png)

\>fcontour("d3",xmin=-4,xmax=1,ymin=-2,ymax=2,hue=1,title="The minimum is on A");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-976.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-976.png)

2) Tetapi jika semua sudut segitiga ABC kurang dari 120°, minimumnya
adalah pada titik F di bagian dalam segitiga, yang merupakan
satu-satunya titik yang melihat sisi-sisi ABC dengan sudut yang sama
(masing-masing 120°):


\>C=[-0.5,1];

\>plot3d("d3",xmin=-2,xmax=2,ymin=-2,ymax=2):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-977.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-977.png)

\>fcontour("d3",xmin=-2,xmax=2,ymin=-2,ymax=2,hue=1,title="The Fermat point");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-978.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-978.png)

Merupakan kegiatan yang menarik untuk merealisasikan gambar di atas
dengan perangkat lunak geometri; sebagai contoh, saya tahu sebuah
perangkat lunak yang ditulis dalam bahasa Java yang memiliki instruksi
"garis kontur"...


Semua hal di atas telah ditemukan oleh seorang hakim Perancis bernama
Pierre de Fermat; dia menulis surat kepada para ahli lain seperti
pendeta Marin Mersenne dan Blaise Pascal yang bekerja di bagian pajak
penghasilan. Jadi titik unik F sedemikian rupa sehingga FA+FB+FC
minimal, disebut titik Fermat dari segitiga. Namun tampaknya beberapa
tahun sebelumnya, Torriccelli dari Italia telah menemukan titik ini
sebelum Fermat menemukannya! Bagaimanapun juga, tradisinya adalah
mencatat titik F ini...


## Empat titik

Langkah selanjutnya adalah menambahkan titik ke-4 D dan mencoba
meminimumkan MA+MB+MC+MD; misalkan Anda adalah operator TV kabel dan
ingin mencari di daerah mana Anda harus memasang antena sehingga Anda
dapat memberi makan empat desa dan menggunakan panjang kabel yang
sesedikit mungkin!


\>D=[1,1];

\>function d4(x,y):=d3(x,y)+sqrt((x-D[1])^2+(y-D[2])^2)

\>plot3d("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-979.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-979.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],points=1,add=1,color=12);

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-980.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-980.png)

Masih ada nilai minimum dan tidak ada simpul A, B, C, maupun D:


\>function f(x):=d4(x[1],x[2])

\>neldermin("f",[0.2,0.2])


    [0.142858,  0.142857]

Tampaknya dalam kasus ini, koordinat titik optimal adalah rasional
atau mendekati rasional...


Karena ABCD adalah sebuah bujur sangkar, maka kita berharap bahwa
titik optimalnya adalah pusat dari ABCD:


\>C=[-1,1];

\>plot3d("d4",xmin=-1,xmax=1,ymin=-1,ymax=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-981.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-981.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],add=1,color=12,points=1);

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-982.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-982.png)

# Contoh 7: Bola Dandelin dengan Povray

Anda dapat menjalankan demonstrasi ini, jika Anda telah menginstal
Povray, dan pvengine.exe pada path program.


Pertama, kita menghitung jari-jari bola.


Jika Anda melihat gambar di bawah ini, Anda dapat melihat bahwa kita
membutuhkan dua lingkaran yang menyentuh dua garis yang membentuk
kerucut, dan satu garis yang membentuk bidang yang memotong kerucut.


Kita menggunakan file geometri.e dari Euler untuk hal ini.


\>load geometry;


Pertama, dua garis yang membentuk kerucut.


\>g1 &= lineThrough([0,0],[1,a])


    
                                 [- a, 1, 0]
    

\>g2 &= lineThrough([0,0],[-1,a])


    
                                [- a, - 1, 0]
    

Kemudian baris ketiga.


\>g &= lineThrough([-1,0],[1,1])


    
                                 [- 1, 2, 1]
    

Kita plot semuanya sejauh ini.


\>setPlotRange(-1,1,0,2);

\>color(black); plotLine(g(),"")

\>a:=2; color(blue); plotLine(g1(),""), plotLine(g2(),""):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-983.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-983.png)

Sekarang, kita ambil titik umum pada sumbu y.


\>P &= [0,u]


    
                                    [0, u]
    

Hitung jarak ke g1.


\>d1 &= distance(P,projectToLine(P,g1)); $d1


$$\sqrt{\left(\frac{a^2\,u}{a^2+1}-u\right)^2+\frac{a^2\,u^2}{\left(a  ^2+1\right)^2}}$$Hitung jarak ke g.


\>d &= distance(P,projectToLine(P,g)); $d


$$\sqrt{\left(\frac{u+2}{5}-u\right)^2+\frac{\left(2\,u-1\right)^2}{  25}}$$Dan temukan pusat kedua lingkaran, yang jaraknya sama.


\>sol &= solve(d1^2=d^2,u); $sol


$$\left[ u=\frac{-\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} , u=  \frac{\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} \right] $$Ada dua solusi.


Kami mengevaluasi solusi simbolis, dan menemukan kedua pusat, dan
kedua jarak.


\>u := sol()


    [0.333333,  1]

\>dd := d()


    [0.149071,  0.447214]

Plot lingkaran ke dalam gambar.


\>color(red);

\>plotCircle(circleWithCenter([0,u[1]],dd[1]),"");

\>plotCircle(circleWithCenter([0,u[2]],dd[2]),"");

\>insimg;


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-987.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-987.png)

## Plot dengan Povray

Selanjutnya kita plot semuanya dengan Povray. Perhatikan bahwa Anda
mengubah perintah apapun pada urutan perintah Povray berikut ini, dan
jalankan kembali semua perintah dengan Shift-Return.


Pertama kita memuat fungsi povray.


\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Kami menyiapkan pemandangan dengan tepat.


\>povstart(zoom=11,center=[0,0,0.5],height=10°,angle=140°);


Selanjutnya kita tuliskan kedua bola tersebut ke file Povray.


\>writeln(povsphere([0,0,u[1]],dd[1],povlook(red)));

\>writeln(povsphere([0,0,u[2]],dd[2],povlook(red)));


Dan kerucutnya, transparan.


\>writeln(povcone([0,0,0],0,[0,0,a],1,povlook(lightgray,1)));


Kami menghasilkan bidang yang terbatas pada kerucut.


\>gp=g();

\>pc=povcone([0,0,0],0,[0,0,a],1,"");

\>vp=[gp[1],0,gp[2]]; dp=gp[3];

\>writeln(povplane(vp,dp,povlook(blue,0.5),pc));


Sekarang kita menghasilkan dua titik pada lingkaran, di mana bola
menyentuh kerucut.


\>function turnz(v) := return [-v[2],v[1],v[3]]

\>P1=projectToLine([0,u[1]],g1()); P1=turnz([P1[1],0,P1[2]]);

\>writeln(povpoint(P1,povlook(yellow)));

\>P2=projectToLine([0,u[2]],g1()); P2=turnz([P2[1],0,P2[2]]);

\>writeln(povpoint(P2,povlook(yellow)));


Kemudian, kita menghasilkan dua titik di mana bola-bola tersebut
menyentuh bidang. Ini adalah fokus elips.


\>P3=projectToLine([0,u[1]],g()); P3=[P3[1],0,P3[2]];

\>writeln(povpoint(P3,povlook(yellow)));

\>P4=projectToLine([0,u[2]],g()); P4=[P4[1],0,P4[2]];

\>writeln(povpoint(P4,povlook(yellow)));


Selanjutnya kita menghitung perpotongan P1P2 dengan bidang.


\>t1=scalp(vp,P1)-dp; t2=scalp(vp,P2)-dp; P5=P1+t1/(t1-t2)\*(P2-P1);

\>writeln(povpoint(P5,povlook(yellow)));


Kami menghubungkan titik-titik dengan segmen garis.


\>writeln(povsegment(P1,P2,povlook(yellow)));

\>writeln(povsegment(P5,P3,povlook(yellow)));

\>writeln(povsegment(P5,P4,povlook(yellow)));


Sekarang, kita menghasilkan pita abu-abu, di mana bola-bola menyentuh
kerucut.


\>pcw=povcone([0,0,0],0,[0,0,a],1.01);

\>pc1=povcylinder([0,0,P1[3]-defaultpointsize/2],[0,0,P1[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc1],povlook(gray)));

\>pc2=povcylinder([0,0,P2[3]-defaultpointsize/2],[0,0,P2[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc2],povlook(gray)));


Mulai program Povray.


\>povend();


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-988.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-988.png)

Untuk mendapatkan Anaglyph ini, kita harus memasukkan semuanya ke
dalam fungsi scene. Fungsi ini akan digunakan dua kali nanti.


\>function scene () ...


    global a,u,dd,g,g1,defaultpointsize;
    writeln(povsphere([0,0,u[1]],dd[1],povlook(red)));
    writeln(povsphere([0,0,u[2]],dd[2],povlook(red)));
    writeln(povcone([0,0,0],0,[0,0,a],1,povlook(lightgray,1)));
    gp=g();
    pc=povcone([0,0,0],0,[0,0,a],1,"");
    vp=[gp[1],0,gp[2]]; dp=gp[3];
    writeln(povplane(vp,dp,povlook(blue,0.5),pc));
    P1=projectToLine([0,u[1]],g1()); P1=turnz([P1[1],0,P1[2]]);
    writeln(povpoint(P1,povlook(yellow)));
    P2=projectToLine([0,u[2]],g1()); P2=turnz([P2[1],0,P2[2]]);
    writeln(povpoint(P2,povlook(yellow)));
    P3=projectToLine([0,u[1]],g()); P3=[P3[1],0,P3[2]];
    writeln(povpoint(P3,povlook(yellow)));
    P4=projectToLine([0,u[2]],g()); P4=[P4[1],0,P4[2]];
    writeln(povpoint(P4,povlook(yellow)));
    t1=scalp(vp,P1)-dp; t2=scalp(vp,P2)-dp; P5=P1+t1/(t1-t2)*(P2-P1);
    writeln(povpoint(P5,povlook(yellow)));
    writeln(povsegment(P1,P2,povlook(yellow)));
    writeln(povsegment(P5,P3,povlook(yellow)));
    writeln(povsegment(P5,P4,povlook(yellow)));
    pcw=povcone([0,0,0],0,[0,0,a],1.01);
    pc1=povcylinder([0,0,P1[3]-defaultpointsize/2],[0,0,P1[3]+defaultpointsize/2],1);
    writeln(povintersection([pcw,pc1],povlook(gray)));
    pc2=povcylinder([0,0,P2[3]-defaultpointsize/2],[0,0,P2[3]+defaultpointsize/2],1);
    writeln(povintersection([pcw,pc2],povlook(gray)));
    endfunction
</pre>
Anda memerlukan kacamata merah/sian untuk mengapresiasi efek berikut
ini.


\>povanaglyph("scene",zoom=11,center=[0,0,0.5],height=10°,angle=140°);


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-989.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-989.png)

# Contoh 8: Geometri Bumi

Pada buku catatan ini, kita ingin melakukan beberapa komputasi bola.
Fungsi-fungsi tersebut terdapat pada file "spherical.e" pada folder
contoh. Kita perlu memuat file tersebut terlebih dahulu.


\>load "spherical.e";


Untuk memasukkan posisi geografis, kita menggunakan vektor dengan dua
koordinat dalam radian (utara dan timur, nilai negatif untuk selatan
dan barat). Berikut ini adalah koordinat untuk Kampus FMIPA UNY.


\>FMIPA=[rad(-7,-46.467),rad(110,23.05)]


    [-0.13569,  1.92657]

Anda dapat mencetak posisi ini dengan sposprint (cetak posisi bola).


\>sposprint(FMIPA) // posisi garis lintang dan garis bujur FMIPA UNY


    S 7°46.467' E 110°23.050'

Mari kita tambahkan dua kota lagi, Solo dan Semarang.


\>Solo=[rad(-7,-34.333),rad(110,49.683)]; Semarang=[rad(-6,-59.05),rad(110,24.533)];

\>sposprint(Solo), sposprint(Semarang),


    S 7°34.333' E 110°49.683'
    S 6°59.050' E 110°24.533'

Pertama, kita menghitung vektor dari satu titik ke titik lainnya pada
bola ideal. Vektor ini adalah [heading, distance] dalam radian. Untuk
menghitung jarak di bumi, kita kalikan dengan jari-jari bumi pada
garis lintang 7°.


\>br=svector(FMIPA,Solo); degprint(br[1]), br[2]\*rearth(7°)-\>km // perkiraan jarak FMIPA-Solo


    65°20'26.60''
    53.8945384608

Ini adalah perkiraan yang baik. Rutinitas berikut ini menggunakan
perkiraan yang lebih baik lagi. Pada jarak yang pendek, hasilnya
hampir sama.


\>esdist(FMIPA,Semarang)-\>" km" // perkiraan jarak FMIPA-Semarang


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan jarak FMIPA-Semarang (character 32)
    You can disable this in the Options menu.
    Error in:
    esdist(FMIPA,Semarang)-&gt;" km" // perkiraan jarak FMIPA-Semaran ...
                                 ^

Ada fungsi untuk judul, dengan mempertimbangkan bentuk elips bumi.
Sekali lagi, kami mencetak dengan cara yang canggih.


\>sdegprint(esdir(FMIPA,Solo))


         65.34°

Sudut segitiga melebihi 180° pada bola.


\>asum=sangle(Solo,FMIPA,Semarang)+sangle(FMIPA,Solo,Semarang) ...  
\>   +sangle(FMIPA,Semarang,Solo); degprint(asum)


    180°0'10.77''

Ini bisa digunakan untuk menghitung luas area segitiga. Catatan: Untuk
segitiga kecil, cara ini tidak akurat karena kesalahan pengurangan
dalam asum-pi.


\>(asum-pi)\*rearth(48°)^2-\>" km^2" // perkiraan luas segitiga FMIPA-Solo-Semarang


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan luas segitiga FMIPA-Solo-Semarang (character 32)
    You can disable this in the Options menu.
    Error in:
    (asum-pi)*rearth(48°)^2-&gt;" km^2" // perkiraan luas segitiga FM ...
                                    ^

Ada sebuah fungsi untuk hal ini, yang menggunakan garis lintang
rata-rata segitiga untuk menghitung radius bumi, dan menangani
kesalahan pembulatan untuk segitiga yang sangat kecil.


\>esarea(Solo,FMIPA,Semarang)-\>" km^2", //perkiraan yang sama dengan fungsi esarea()


    2123.64310526 km^2

Kita juga dapat menambahkan vektor ke posisi. Sebuah vektor berisi
arah dan jarak, keduanya dalam radian. Untuk mendapatkan sebuah
vektor, kita menggunakan svector. Untuk menambahkan sebuah vektor ke
sebuah posisi, kita menggunakan saddvector.


\>v=svector(FMIPA,Solo); sposprint(saddvector(FMIPA,v)), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Fungsi-fungsi ini mengasumsikan bola yang ideal. Hal yang sama di
bumi.


\>sposprint(esadd(FMIPA,esdir(FMIPA,Solo),esdist(FMIPA,Solo))), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Mari kita beralih ke contoh yang lebih besar, Tugu Jogja dan Monas
Jakarta (menggunakan Google Earth untuk menemukan koordinatnya).


\>Tugu=[-7.7833°,110.3661°]; Monas=[-6.175°,106.811944°];

\>sposprint(Tugu), sposprint(Monas)


    S 7°46.998' E 110°21.966'
    S 6°10.500' E 106°48.717'

Menurut Google Earth, jaraknya adalah 429,66 km. Kami mendapatkan
perkiraan yang bagus.


\>esdist(Tugu,Monas)-\>" km" // perkiraan jarak Tugu Jogja - Monas Jakarta


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan jarak Tugu Jogja - Monas Jakarta (character 32)
    You can disable this in the Options menu.
    Error in:
    esdist(Tugu,Monas)-&gt;" km" // perkiraan jarak Tugu Jogja - Mona ...
                             ^

Judulnya sama dengan yang dihitung di Google Earth.


\>degprint(esdir(Tugu,Monas))


    294°17'2.85''

Namun demikian, kita tidak lagi mendapatkan posisi target yang tepat,
jika kita menambahkan arah dan jarak ke posisi semula. Hal ini
terjadi, karena kita tidak menghitung fungsi inversi secara tepat,
tetapi mengambil perkiraan radius bumi di sepanjang jalur.


\>sposprint(esadd(Tugu,esdir(Tugu,Monas),esdist(Tugu,Monas)))


    S 6°10.500' E 106°48.717'

Namun demikian, kesalahannya tidak besar.


\>sposprint(Monas),


    S 6°10.500' E 106°48.717'

Tentu saja, kita tidak bisa berlayar dengan arah yang sama dari satu
tujuan ke tujuan lainnya, jika kita ingin mengambil jalur terpendek.
Bayangkan, Anda terbang ke arah NE mulai dari titik mana pun di bumi.
Kemudian Anda akan berputar ke kutub utara. Lingkaran besar tidak
mengikuti arah yang konstan!


Perhitungan berikut ini menunjukkan bahwa kita akan melenceng dari
tujuan yang benar, jika kita menggunakan arah yang sama selama
perjalanan.


\>dist=esdist(Tugu,Monas); hd=esdir(Tugu,Monas);


Sekarang kita tambahkan 10 kali sepersepuluh dari jarak tersebut,
dengan menggunakan arah menuju Monas, kita akan sampai di Tugu.


\>p=Tugu; loop 1 to 10; p=esadd(p,hd,dist/10); end;


Hasilnya jauh berbeda.


\>sposprint(p), skmprint(esdist(p,Monas))


    S 6°11.250' E 106°48.372'
         1.529km

Sebagai contoh lain, mari kita ambil dua titik di bumi pada garis
lintang yang sama.


\>P1=[30°,10°]; P2=[30°,50°];


Jalur terpendek dari P1 ke P2 bukanlah lingkaran lintang 30°, tetapi
jalur yang lebih pendek yang dimulai 10° lebih jauh ke utara di P1.


\>sdegprint(esdir(P1,P2))


         79.69°

Namun, jika kita mengikuti pembacaan kompas ini, kita akan berputar ke
kutub utara! Jadi, kita harus menyesuaikan arah kita di sepanjang
jalan. Untuk tujuan kasar, kita sesuaikan pada 1/10 dari jarak total.


\>p=P1;  dist=esdist(P1,P2); ...  
\>     loop 1 to 10; dir=esdir(p,P2); sdegprint(dir), p=esadd(p,dir,dist/10); end;


         79.69°
         81.67°
         83.71°
         85.78°
         87.89°
         90.00°
         92.12°
         94.22°
         96.29°
         98.33°

Jaraknya tidak tepat, karena kita akan menambahkan sedikit kesalahan,
jika kita mengikuti judul yang sama terlalu lama.


\>skmprint(esdist(p,P2))


         0.203km

Kita akan mendapatkan perkiraan yang baik, jika kita menyesuaikan arah
setiap 1/100 dari total jarak dari Tugu ke Monas.


\>p=Tugu; dist=esdist(Tugu,Monas); ...  
\>     loop 1 to 100; p=esadd(p,esdir(p,Monas),dist/100); end;

\>skmprint(esdist(p,Monas))


         0.000km

Untuk keperluan navigasi, kita bisa mendapatkan urutan posisi GPS di
sepanjang Bundaran Hotel Indonesia menuju Monas dengan fungsi
navigate.


\>load spherical; v=navigate(Tugu,Monas,10); ...  
\>     loop 1 to rows(v); sposprint(v[#]), end;


    S 7°46.998' E 110°21.966'
    S 7°37.422' E 110°0.573'
    S 7°27.829' E 109°39.196'
    S 7°18.219' E 109°17.834'
    S 7°8.592' E 108°56.488'
    S 6°58.948' E 108°35.157'
    S 6°49.289' E 108°13.841'
    S 6°39.614' E 107°52.539'
    S 6°29.924' E 107°31.251'
    S 6°20.219' E 107°9.977'
    S 6°10.500' E 106°48.717'

Kami menulis sebuah fungsi, yang memplot bumi, dua posisi, dan posisi
di antaranya.


\>function testplot ...


    useglobal;
    plotearth;
    plotpos(Tugu,"Tugu Jogja"); plotpos(Monas,"Tugu Monas");
    plotposline(v);
    endfunction
</pre>
Sekarang plot semuanya.


\>plot3d("testplot",angle=25, height=6,\>own,\>user,zoom=4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-990.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-990.png)

Atau gunakan plot3d untuk mendapatkan tampilan anaglyph. Ini terlihat
sangat bagus dengan kacamata merah/cyan.


\>plot3d("testplot",angle=25,height=6,distance=5,own=1,anaglyph=1,zoom=4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-991.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-991.png)

# Latihan

1. Gambarlah segi-n beraturan jika diketahui titik pusat O, n, dan
jarak titik pusat ke titik-titik sudut segi-n tersebut (jari-jari
lingkaran luar segi-n), r.


Petunjuk:


* 
Besar sudut pusat yang menghadap masing-masing sisi segi-n adalah
* (360/n).

* 
Titik-titik sudut segi-n merupakan perpotongan lingkaran luar segi-n
* dan garis-garis yang melalui pusat dan saling membentuk sudut sebesar
* kelipatan (360/n).

* 
Untuk n ganjil, pilih salah satu titik sudut adalah di atas.

* 
Untuk n genap, pilih 2 titik di kanan dan kiri lurus dengan titik
* pusat.

* 
Anda dapat menggambar segi-3, 4, 5, 6, 7, dst beraturan.


\>load geometry


    Numerical and symbolic geometry.

\>setPlotRange(-3.5,3.5,-3.5,3.5);

\>O=[0,0]; plotPoint(O,"O");

\>A=[-2,-1]; plotPoint(A,"A");

\>B=[2,-1]; plotPoint(B,"B");

\>C=[0,2\*3^0.5-1]; plotPoint(A,"A");

\>plotSegment(A,B,"c");

\>plotSegment(B,C,"a");

\>plotSegment(A,C,"b");

\>aspect(1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-992.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-992.png)

\>c=circleThrough(A,B,C):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-993.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-993.png)

\>R=getCircleRadius(c);

\>O=getCircleCenter(c)


    [0,  0.154701]

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-994.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-994.png)

2. Gambarlah suatu parabola yang melalui 3 titik yang diketahui.


Petunjuk:


- Misalkan persamaan parabolanya y= ax^2+bx+c.


- Substitusikan koordinat titik-titik yang diketahui ke persamaan
tersebut.


- Selesaikan SPL yang terbentuk untuk mendapatkan nilai-nilai a, b, c.


\>setPlotRange(5); 

\>K=[-4,0];  L=[4,0] ; M=[0,2];

\>plotPoint(K,"K"); plotPoint(L,"L"); plotPoint(M,"M"): 


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-995.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-995.png)

\>sol &= solve([16\*a+8\*b=-c,16\*a-8\*b=-c,c=2],[a,b,c])


    
                                  1
                          [[a = - -, b = 0, c = 2]]
                                  8
    

\>function y&=-1/8\*(x^2)-0\*x+2


    
                                         2
                                        x
                                    2 - --
                                        8
    

\>plot2d("-1/8\*(x^2)-0\*x+2",-5,5,-5,5); ...  
\>   plotPoint(K,"K"); plotPoint(L,"L"); plotPoint(M,"M"): 


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-996.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-996.png)

3. Gambarlah suatu segi-4 yang diketahui keempat titik sudutnya,
misalnya A, B, C, D.


   - Tentukan apakah segi-4 tersebut merupakan segi-4 garis singgung
(sisinya-sisintya merupakan garis singgung lingkaran yang sama yakni
lingkaran dalam segi-4 tersebut).


   - Suatu segi-4 merupakan segi-4 garis singgung apabila keempat
garis bagi sudutnya bertemu di satu titik.


   - Jika segi-4 tersebut merupakan segi-4 garis singgung, gambar
lingkaran dalamnya.


   - Tunjukkan bahwa syarat suatu segi-4 merupakan segi-4 garis
singgung apabila hasil kali panjang sisi-sisi yang berhadapan sama.


\>setPlotRange(5);

\>A=[-3,-3];  B=[3,-3] ; C=[3,3]; D=[-3,3];

\>plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); plotPoint(D,"D");

\>plotSegment(A,B,""); plotSegment(B,C,""); plotSegment(C,D,""); plotSegment(D,A,""):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-997.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-997.png)

\>l=angleBisector(A,B,C);

\>g=angleBisector(B,C,D);

\>P=lineIntersection(l,g)


    [0,  0]

\>color(5); plotLine(l); plotLine(g); color(1);

\>plotPoint(P,"P"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-998.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-998.png)

\>r=norm(P-projectToLine(P,lineThrough(A,B)))


    3

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segiempat ABC"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-999.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-999.png)

Darai gambar di atas, terlihat bahwa sisi-sisinya merupakan garis
singgung lingkaran yang sama yaitu lingkaran dalam segiempat.


Kemudian akan ditunjukkan bahwa hasil kali panjang sisi-sisi yang
berhadapan sama.


\>AB=norm(A-B) // panjang sisi AB


    6

\>BC=norm(B-C) // panjang sisi ABC


    6

\>CD=norm(C-D) // panjang sisi CD


    6

\>DA=norm(D-A) // panjang sisi DA


    6

\>AB.CD


    36

\>DA.BC


    36

5. Gambarlah suatu hiperbola jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang selisih jarak ke P dan ke Q selalu sama
(konstan).


\>P=[-1,2]; Q=[1,2];

\>function d1(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)

\>function d2(x,y):=d1(x,y)+sqrt((x-Q[1])^2+(y-Q[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=0,ymax=4,hue=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1000.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1000.png)

Grafik yang lebih menarik


\>plot3d("d2",xmin=-2,xmax=2,ymin=0,ymax=4,hue=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1001.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1001.png)

Batasan garis PQ


\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1002.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1002.png)

5. Gambarlah suatu hiperbola jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang selisih jarak ke P dan ke Q selalu sama
(konstan).


\>P=[-1,2]; Q=[1,2];

\>function d3(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)

\>function d4(x,y):=d3(x,y)+sqrt((x-Q[1])^2+(y-Q[2])^2

\>fcontour("d3",xmin=-4,xmax=2,ymin=0,ymax=4,hue=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1003.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1003.png)

Grafik yang lebih menarik


\>plot3d("d3",xmin=-2,xmax=2,ymin=0,ymax=4,hue=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1004.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1004.png)

\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1005.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1005.png)

---

---

---

# EMT untuk Statistika

Dalam buku catatan ini, kami mendemonstrasikan plot statistik utama,
tes, dan distribusi dalam Euler.


Mari kita mulai dengan beberapa statistik deskriptif. Ini bukanlah
sebuah pengantar statistik. Jadi, Anda mungkin memerlukan latar
belakang untuk memahami detailnya.


Asumsikan pengukuran berikut. Kita ingin menghitung nilai rata-rata
dan deviasi standar yang diukur.


\>M=[1000,1004,998,997,1002,1001,998,1004,998,997]; ...  
\>   median(M), mean(M), dev(M),


    999
    999.9
    2.72641400622

Kita dapat memplot plot kotak dan whisker untuk data tersebut. Dalam
kasus kita, tidak ada pencilan. 


\>aspect(1.75); boxplot(M):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1006.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1006.png)

Kami menghitung probabilitas bahwa suatu nilai lebih besar dari 1005,
dengan mengasumsikan nilai yang diukur dari distribusi normal.


Semua fungsi untuk distribusi dalam Euler diakhiri dengan ...dis dan
menghitung distribusi probabilitas kumulatif (CPF).


$$\text{normaldis(x,m,d)}=\int_{-\infty}^x \frac{1}{d\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{t-m}{d})^2}\ dt.$$Kami mencetak hasilnya dalam % dengan akurasi 2 digit menggunakan
fungsi cetak.


\>print((1-normaldis(1005,mean(M),dev(M)))\*100,2,unit=" %")


          3.07 %

Untuk contoh berikutnya, kami mengasumsikan jumlah pria berikut ini
dalam rentang ukuran tertentu.


\>r=155.5:4:187.5; v=[22,71,136,169,139,71,32,8];


Berikut ini adalah plot distribusinya.


\>plot2d(r,v,a=150,b=200,c=0,d=190,bar=1,style="\\/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1008.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1008.png)

Kita dapat memasukkan data mentah tersebut ke dalam tabel.


Tabel adalah sebuah metode untuk menyimpan data statistik. Tabel kita
harus berisi tiga kolom: Awal rentang, akhir rentang, jumlah orang
dalam rentang.


Tabel dapat dicetak dengan header. Kami menggunakan vektor string
untuk mengatur header.


\>T:=r[1:8]' | r[2:9]' | v'; writetable(T,labc=["BB","BA","Frek"])


            BB        BA      Frek
         155.5     159.5        22
         159.5     163.5        71
         163.5     167.5       136
         167.5     171.5       169
         171.5     175.5       139
         175.5     179.5        71
         179.5     183.5        32
         183.5     187.5         8

Jika kita membutuhkan nilai rata-rata dan statistik lain dari ukuran,
kita perlu menghitung titik tengah rentang. Kita dapat menggunakan dua
kolom pertama dari tabel kita untuk hal ini.


Sumbol "|" digunakan untuk memisahkan kolom, fungsi "writetable"
digunakan untuk menulis tabel, dengan opsi "labc" untuk menentukan
judul kolom.


\>(T[,1]+T[,2])/2 // the midpoint of each interval


            157.5 
            161.5 
            165.5 
            169.5 
            173.5 
            177.5 
            181.5 
            185.5 

Tetapi akan lebih mudah, untuk melipat rentang dengan vektor
[1/2,1/2].


\>M=fold(r,[0.5,0.5])


    [157.5,  161.5,  165.5,  169.5,  173.5,  177.5,  181.5,  185.5]

Sekarang kita dapat menghitung rata-rata dan deviasi sampel dengan
frekuensi yang diberikan.


\>{m,d}=meandev(M,v); m, d,


    169.901234568
    5.98912964449

Mari kita tambahkan distribusi normal dari nilai-nilai tersebut ke
dalam diagram batang di atas. Rumus untuk distribusi normal dengan
rata-rata m dan deviasi standar d adalah:


$$y=\frac{1}{d\sqrt{2\pi}}e^{\frac{-(x-m)^2}{2d^2}}.$$Karena nilainya antara 0 dan 1, untuk memplotnya pada diagram batang,
nilai tersebut harus dikalikan dengan 4 kali jumlah data.


\>plot2d("qnormal(x,m,d)\*sum(v)\*4", ...  
\>     xmin=min(r),xmax=max(r),thickness=3,add=1):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1010.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1010.png)

# Tabel

Dalam direktori buku catatan ini, Anda dapat menemukan file dengan
tabel. Data tersebut mewakili hasil survei. Berikut adalah empat baris
pertama dari file tersebut. Data berasal dari buku online berbahasa
Jerman "Einführung in die Statistik mit R" oleh A. Handl.


\>printfile("table.dat",4);


    Person Sex Age Titanic Evaluation Tip Problem
    1 m 30 n . 1.80 n
    2 f 23 y g 1.80 n
    3 f 26 y g 1.80 y

Tabel berisi 7 kolom angka atau token (string). Kita ingin membaca
tabel tersebut dari file. Pertama, kita menggunakan terjemahan kita
sendiri untuk token-token tersebut.


Untuk itu, kita mendefinisikan set token. Fungsi strtokens()
mendapatkan vektor string token dari string yang diberikan.


\>mf:=["m","f"]; yn:=["y","n"]; ev:=strtokens("g vg m b vb");


Sekarang kita membaca tabel dengan terjemahan ini.


Argumen tok2, tok4, dan lain-lain adalah terjemahan dari kolom-kolom
tabel. Argumen-argumen ini tidak ada dalam daftar parameter
readtable(), jadi Anda harus menyediakannya dengan ":=".


\>{MT,hd}=readtable("table.dat",tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);

\>load over statistics;


Untuk mencetak, kita perlu menentukan set token yang sama. Kami
mencetak empat baris pertama saja.


\>writetable(MT[1:10],labc=hd,wc=5,tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);


     Person  Sex  Age Titanic Evaluation  Tip Problem
          1    m   30       n          .  1.8       n
          2    f   23       y          g  1.8       n
          3    f   26       y          g  1.8       y
          4    m   33       n          .  2.8       n
          5    m   37       n          .  1.8       n
          6    m   28       y          g  2.8       y
          7    f   31       y         vg  2.8       n
          8    m   23       n          .  0.8       n
          9    f   24       y         vg  1.8       y
         10    m   26       n          .  1.8       n

Tanda titik "." mewakili nilai yang tidak tersedia.


Jika kita tidak ingin menentukan token untuk terjemahan sebelumnya,
kita hanya perlu menentukan kolom mana yang berisi token dan bukan
angka.


\>ctok=[2,4,5,7]; {MT,hd,tok}=readtable("table.dat",ctok=ctok);


Fungsi readtable() sekarang mengembalikan satu set token.


\>tok


    m
    n
    f
    y
    g
    vg

Tabel berisi entri dari file dengan token yang diterjemahkan ke angka.


String khusus NA="." ditafsirkan sebagai " Not Available", dan
mendapatkan NAN ( not a number ) dalam tabel. Terjemahan ini dapat
diubah dengan parameter NA, dan NAval.


\>MT[1]


    [1,  1,  30,  2,  NAN,  1.8,  2]

Berikut ini adalah isi tabel dengan angka yang tidak diterjemahkan.


\>writetable(MT,wc=5)


        1    1   30    2    .  1.8    2
        2    3   23    4    5  1.8    2
        3    3   26    4    5  1.8    4
        4    1   33    2    .  2.8    2
        5    1   37    2    .  1.8    2
        6    1   28    4    5  2.8    4
        7    3   31    4    6  2.8    2
        8    1   23    2    .  0.8    2
        9    3   24    4    6  1.8    4
       10    1   26    2    .  1.8    2
       11    3   23    4    6  1.8    4
       12    1   32    4    5  1.8    2
       13    1   29    4    6  1.8    4
       14    3   25    4    5  1.8    4
       15    3   31    4    5  0.8    2
       16    1   26    4    5  2.8    2
       17    1   37    2    .  3.8    2
       18    1   38    4    5    .    2
       19    3   29    2    .  3.8    2
       20    3   28    4    6  1.8    2
       21    3   28    4    1  2.8    4
       22    3   28    4    6  1.8    4
       23    3   38    4    5  2.8    2
       24    3   27    4    1  1.8    4
       25    1   27    2    .  2.8    4

Untuk kenyamanan, Anda dapat menaruh output dari readtable() ke dalam
sebuah daftar.


\>Table={{readtable("table.dat",ctok=ctok)}};


Dengan menggunakan kolom token yang sama dan token yang dibaca dari
file, kita dapat mencetak tabel. Kita dapat menentukan ctok, tok, dll.
atau menggunakan daftar Tabel.


\>writetable(Table,ctok=ctok,wc=5);


     Person  Sex  Age Titanic Evaluation  Tip Problem
          1    m   30       n          .  1.8       n
          2    f   23       y          g  1.8       n
          3    f   26       y          g  1.8       y
          4    m   33       n          .  2.8       n
          5    m   37       n          .  1.8       n
          6    m   28       y          g  2.8       y
          7    f   31       y         vg  2.8       n
          8    m   23       n          .  0.8       n
          9    f   24       y         vg  1.8       y
         10    m   26       n          .  1.8       n
         11    f   23       y         vg  1.8       y
         12    m   32       y          g  1.8       n
         13    m   29       y         vg  1.8       y
         14    f   25       y          g  1.8       y
         15    f   31       y          g  0.8       n
         16    m   26       y          g  2.8       n
         17    m   37       n          .  3.8       n
         18    m   38       y          g    .       n
         19    f   29       n          .  3.8       n
         20    f   28       y         vg  1.8       n
         21    f   28       y          m  2.8       y
         22    f   28       y         vg  1.8       y
         23    f   38       y          g  2.8       n
         24    f   27       y          m  1.8       y
         25    m   27       n          .  2.8       y

Fungsi tablecol() mengembalikan nilai kolom dari tabel, melewatkan
setiap baris dengan nilai NAN ("." dalam file), dan indeks kolom, yang
berisi nilai-nilai ini.


\>{c,i}=tablecol(MT,[5,6]);


Kita dapat menggunakan ini untuk mengekstrak kolom dari tabel untuk
tabel baru.


\>j=[1,5,6]; writetable(MT[i,j],labc=hd[j],ctok=[2],tok=tok)


        Person Evaluation       Tip
             2          g       1.8
             3          g       1.8
             6          g       2.8
             7         vg       2.8
             9         vg       1.8
            11         vg       1.8
            12          g       1.8
            13         vg       1.8
            14          g       1.8
            15          g       0.8
            16          g       2.8
            20         vg       1.8
            21          m       2.8
            22         vg       1.8
            23          g       2.8
            24          m       1.8

Tentu saja, kita perlu mengekstrak tabel itu sendiri dari daftar Tabel
dalam kasus ini.


\>MT=Table[1];


Tentu saja, kita juga dapat menggunakannya untuk menentukan nilai
rata-rata kolom atau nilai statistik lainnya.


\>mean(tablecol(MT,6))


    2.175

Fungsi getstatistics() mengembalikan elemen-elemen dalam sebuah
vektor, dan jumlahnya. Kita menerapkannya pada nilai "m" dan "f" pada
kolom kedua tabel kita.


\>{xu,count}=getstatistics(tablecol(MT,2)); xu, count,


    [1,  3]
    [12,  13]

Kita bisa mencetak hasilnya dalam tabel baru.


\>writetable(count',labr=tok[xu])


             m        12
             f        13

Fungsi selecttable() mengembalikan sebuah tabel baru dengan nilai
dalam satu kolom yang dipilih dari vektor indeks. Pertama, kita
mencari indeks dari dua nilai kita dalam tabel token.


\>v:=indexof(tok,["g","vg"])


    [5,  6]

Sekarang kita dapat memilih baris-baris dari tabel, yang memiliki
salah satu nilai dalam v di baris ke-5.


\>MT1:=MT[selectrows(MT,5,v)]; i:=sortedrows(MT1,5);


Sekarang kita dapat mencetak tabel, dengan nilai yang diekstrak dan
diurutkan di kolom ke-5.


\>writetable(MT1[i],labc=hd,ctok=ctok,tok=tok,wc=7);


     Person    Sex    Age Titanic Evaluation    Tip Problem
          2      f     23       y          g    1.8       n
          3      f     26       y          g    1.8       y
          6      m     28       y          g    2.8       y
         18      m     38       y          g      .       n
         16      m     26       y          g    2.8       n
         15      f     31       y          g    0.8       n
         12      m     32       y          g    1.8       n
         23      f     38       y          g    2.8       n
         14      f     25       y          g    1.8       y
          9      f     24       y         vg    1.8       y
          7      f     31       y         vg    2.8       n
         20      f     28       y         vg    1.8       n
         22      f     28       y         vg    1.8       y
         13      m     29       y         vg    1.8       y
         11      f     23       y         vg    1.8       y

Untuk statistik berikutnya, kita ingin menghubungkan dua kolom tabel.
Jadi kita mengekstrak kolom 2 dan 4 dan mengurutkan tabel.


\>i=sortedrows(MT,[2,4]);  ...  
\>     writetable(tablecol(MT[i],[2,4])',ctok=[1,2],tok=tok)


             m         n
             m         n
             m         n
             m         n
             m         n
             m         n
             m         n
             m         y
             m         y
             m         y
             m         y
             m         y
             f         n
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y
             f         y

Dengan getstatistics(), kita juga dapat menghubungkan hitungan dalam
dua kolom tabel satu sama lain.


\>MT24=tablecol(MT,[2,4]); ...  
\>   {xu1,xu2,count}=getstatistics(MT24[1],MT24[2]); ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2])


                       n         y
             m         7         5
             f         1        12

Tabel dapat ditulis ke sebuah file.


\>filename="test.dat"; ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2],file=filename);


Kemudian kita dapat membaca tabel dari file tersebut.


\>{MT2,hd,tok2,hdr}=readtable(filename,\>clabs,\>rlabs); ...  
\>   writetable(MT2,labr=hdr,labc=hd)


                       n         y
             m         7         5
             f         1        12

Dan hapus file tersebut.


\>fileremove(filename);


# Distribusi

Dengan plot2d, ada metode yang sangat mudah untuk memplot distribusi
data eksperimen.


\>p=normal(1,1000); //1000 random normal-distributed sample p

\>plot2d(p,distribution=20,style="\\/"); // plot the random sample p

\>plot2d("qnormal(x,0,1)",add=1): // add the standard normal distribution plot


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1011.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1011.png)

Perhatikan perbedaan antara plot batang (sampel) dan kurva normal
(distribusi sesungguhnya). Masukkan kembali ketiga perintah tersebut
untuk melihat hasil pengambilan sampel yang lain.


Berikut ini adalah perbandingan 10 simulasi dari 1000 nilai
terdistribusi normal dengan menggunakan apa yang disebut plot kotak.
Plot ini menunjukkan median, kuartil 25% dan 75%, nilai minimal dan
maksimal, serta outlier.


\>p=normal(10,1000); boxplot(p):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1012.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1012.png)

Untuk menghasilkan bilangan bulat acak, Euler memiliki intrandom. Mari
kita simulasikan pelemparan dadu dan memplot distribusinya.


Kita menggunakan fungsi getmultiplicities(v,x), yang menghitung
seberapa sering elemen-elemen dari v muncul di dalam x. Kemudian kita
memplot hasilnya menggunakan columnsplot().


\>k=intrandom(1,6000,6);  ...  
\>   columnsplot(getmultiplicities(1:6,k));  ...  
\>   ygrid(1000,color=red):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1013.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1013.png)

Meskipun intrandom(n,m,k) menghasilkan bilangan bulat yang
terdistribusi secara seragam dari 1 sampai k, adalah mungkin untuk
menggunakan distribusi bilangan bulat yang lain dengan randpint().


Pada contoh berikut, probabilitas untuk 1,2,3 adalah 0.4, 0.1, 0.5
secara berurutan.


\>randpint(1,1000,[0.4,0.1,0.5]); getmultiplicities(1:3,%)


    [378,  102,  520]

Euler dapat menghasilkan nilai acak dari lebih banyak distribusi.
Lihatlah ke dalam referensi.


Misalnya, kita mencoba distribusi eksponensial. Sebuah variabel acak
kontinu X dikatakan memiliki distribusi eksponensial, jika PDF-nya
diberikan oleh


$$f_X(x)=\lambda e^{-\lambda x},\quad x>0,\quad \lambda>0,$$

dengan parameter


$$\lambda=\frac{1}{\mu},\quad \mu \text{ is the mean, and denoted by } X \sim \text{Exponential}(\lambda).$$\>plot2d(randexponential(1,1000,2),\>distribution):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1016.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1016.png)

Untuk banyak distribusi, Euler dapat menghitung fungsi distribusi dan
kebalikannya.


\>plot2d("normaldis",-4,4): 


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1017.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1017.png)

Berikut ini adalah salah satu cara untuk memplot kuantil.


\>plot2d("qnormal(x,1,1.5)",-4,6);  ...  
\>   plot2d("qnormal(x,1,1.5)",a=2,b=5,\>add,\>filled):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1018.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1018.png)

$$\text{normaldis(x,m,d)}=\int_{-\infty}^x \frac{1}{d\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{t-m}{d})^2}\ dt.$$

Probabilitas untuk berada di area hijau adalah sebagai berikut.


\>normaldis(5,1,1.5)-normaldis(2,1,1.5)


    0.248662156979

Hal ini dapat dihitung secara numerik dengan integral berikut ini.


$$\int_2^5 \frac{1}{1.5\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{x-1}{1.5})^2}\ dx.$$\>gauss("qnormal(x,1,1.5)",2,5)


    0.248662156979

Mari kita bandingkan distribusi binomial dengan distribusi normal
dengan rata-rata dan deviasi yang sama. Fungsi invbindis()
menyelesaikan interpolasi linier antara nilai bilangan bulat.


\>invbindis(0.95,1000,0.5), invnormaldis(0.95,500,0.5\*sqrt(1000))


    525.516721219
    526.007419394

Fungsi qdis() adalah densitas dari distribusi chi-square. Seperti
biasa, Euler memetakan vektor ke fungsi ini. Dengan demikian kita
mendapatkan plot semua distribusi chi-kuadrat dengan derajat 5 hingga
30 dengan mudah dengan cara berikut.


\>plot2d("qchidis(x,(5:5:50)')",0,50):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1021.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1021.png)

Euler memiliki fungsi-fungsi yang akurat untuk mengevaluasi
distribusi-distribusi. Mari kita periksa chidis() dengan sebuah
integral.


Penamaannya diusahakan untuk konsisten. Sebagai contoh,


* 
distribusi chi-kuadrat adalah chidis(),

* 
fungsi kebalikannya adalah invchidis(),

* 
densitasnya adalah qchidis().


Pelengkap dari distribusi (upper tail) adalah chicdis().


\>chidis(1.5,2), integrate("qchidis(x,2)",0,1.5)


    0.527633447259
    0.527633447259

# Distribusi Diskrit

Untuk menentukan distribusi diskrit Anda sendiri, Anda dapat
menggunakan metode berikut.


Pertama, kita tetapkan fungsi distribusinya.


\>wd = 0|((1:6)+[-0.01,0.01,0,0,0,0])/6


    [0,  0.165,  0.335,  0.5,  0.666667,  0.833333,  1]

Artinya, dengan probabilitas wd[i+1]-wd[i] kita menghasilkan nilai
acak i.


Ini hampir merupakan distribusi yang seragam. Mari kita definisikan
sebuah generator bilangan acak untuk ini. Fungsi find(v,x) menemukan
nilai x dalam vektor v. Fungsi ini juga dapat digunakan untuk vektor
x.


\>function wrongdice (n,m) := find(wd,random(n,m))


Kesalahan ini sangat halus sehingga kita hanya bisa melihatnya setelah
melakukan iterasi yang sangat banyak.


\>columnsplot(getmultiplicities(1:6,wrongdice(1,1000000))):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1022.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1022.png)

Berikut ini adalah fungsi sederhana untuk memeriksa distribusi seragam
dari nilai 1... K dalam v. Kami menerima hasilnya, jika untuk semua
frekuensi


$$\left|f_i-\frac{1}{K}\right| < \frac{\delta}{\sqrt{n}}.$$\>function checkrandom (v, delta=1) ...


      K=max(v); n=cols(v);
      fr=getfrequencies(v,1:K);
      return max(fr/n-1/K)<delta/sqrt(n);
      endfunction
</pre>
Memang fungsi ini menolak distribusi seragam.


\>checkrandom(wrongdice(1,1000000))


    0

Dan ini menerima generator acak built-in.


\>checkrandom(intrandom(1,1000000,6))


    1

Kita dapat menghitung distribusi binomial. Pertama, ada binomialsum(),
yang mengembalikan probabilitas i atau kurang dari n percobaan.


\>bindis(410,1000,0.4)


    0.751401349654

Fungsi Beta invers digunakan untuk menghitung interval kepercayaan
Clopper-Pearson untuk parameter p. Tingkat defaultnya adalah alpha.


Arti dari interval ini adalah jika p berada di luar interval, hasil
yang diamati sebesar 410 dalam 1000 jarang terjadi.


\>clopperpearson(410,1000)


    [0.37932,  0.441212]

Perintah berikut ini adalah cara langsung untuk mendapatkan hasil di
atas. Tetapi untuk n yang besar, penjumlahan langsung tidak akurat dan
lambat.


\>p=0.4; i=0:410; n=1000; sum(bin(n,i)\*p^i\*(1-p)^(n-i))


    0.751401349655

Omong-omong, invbinsum() menghitung kebalikan dari binomialsum().


\>invbindis(0.75,1000,0.4)


    409.932733047

Dalam Bridge, kita mengasumsikan 5 kartu yang terbuka (dari 52 kartu)
di dua tangan (26 kartu). Mari kita hitung probabilitas distribusi
yang lebih buruk dari 3:2 (misalnya 0:5, 1:4, 4:1, atau 5:0).


\>2\*hypergeomsum(1,5,13,26)


    0.321739130435

Ada juga simulasi distribusi multinomial.


\>randmultinomial(10,1000,[0.4,0.1,0.5])


              381           100           519 
              376            91           533 
              417            80           503 
              440            94           466 
              406           112           482 
              408            94           498 
              395           107           498 
              399            96           505 
              428            87           485 
              400            99           501 

# Memplot Data

Untuk memplot data, kami mencoba hasil pemilihan umum Jerman sejak
tahun 1990, yang diukur dalam kursi.


\>BW := [ ...  
\>   1990,662,319,239,79,8,17; ...  
\>   1994,672,294,252,47,49,30; ...  
\>   1998,669,245,298,43,47,36; ...  
\>   2002,603,248,251,47,55,2; ...  
\>   2005,614,226,222,61,51,54; ...  
\>   2009,622,239,146,93,68,76; ...  
\>   2013,631,311,193,0,63,64];


Untuk partai-partai, kami menggunakan serangkaian nama.


\>P:=["CDU/CSU","SPD","FDP","Gr","Li"];


Mari kita cetak persentasenya dengan baik.


Pertama kita ekstrak kolom-kolom yang diperlukan. Kolom 3 sampai 7
adalah kursi masing-masing partai, dan kolom 2 adalah jumlah total
kursi. kolom adalah tahun pemilihan.


\>BT:=BW[,3:7]; BT:=BT/sum(BT); YT:=BW[,1]';


Kemudian kita mencetak statistik dalam bentuk tabel. Kita menggunakan
nama sebagai judul kolom, dan tahun sebagai judul baris. Lebar default
untuk kolom adalah wc = 10, tetapi kami lebih suka output yang lebih
padat. Kolom-kolom akan diperluas untuk label-label kolom, jika perlu.


\>writetable(BT\*100,wc=6,dc=0,\>fixed,labc=P,labr=YT)


           CDU/CSU   SPD   FDP    Gr    Li
      1990      48    36    12     1     3
      1994      44    38     7     7     4
      1998      37    45     6     7     5
      2002      41    42     8     9     0
      2005      37    36    10     8     9
      2009      38    23    15    11    12
      2013      49    31     0    10    10

Perkalian matriks berikut ini mengekstrak jumlah persentase dua partai
besar yang menunjukkan bahwa partai-partai kecil telah memperoleh
suara di parlemen hingga tahun 2009.


\>BT1:=(BT.[1;1;0;0;0])'\*100


    [84.29,  81.25,  81.1659,  82.7529,  72.9642,  61.8971,  79.8732]

Ada juga plot statistik sederhana. Kita menggunakannya untuk
menampilkan garis dan titik secara bersamaan. Alternatif lainnya
adalah memanggil plot2d dua kali dengan &gt;add.


\>statplot(YT,BT1,"b"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1024.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1024.png)

Tentukan beberapa warna untuk masing-masing pihak.


\>CP:=[rgb(0.5,0.5,0.5),red,yellow,green,rgb(0.8,0,0)];


Sekarang kita dapat memplot hasil pemilu 2009 dan perubahannya ke
dalam satu plot menggunakan figure. Kita dapat menambahkan vektor
kolom pada setiap plot.


\>figure(2,1);  ...  
\>   figure(1); columnsplot(BW[6,3:7],P,color=CP); ...  
\>   figure(2); columnsplot(BW[6,3:7]-BW[5,3:7],P,color=CP);  ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1025.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1025.png)

Plot data menggabungkan baris data statistik dalam satu plot.


\>J:=BW[,1]'; DP:=BW[,3:7]'; ...  
\>   dataplot(YT,BT',color=CP);  ...  
\>   labelbox(P,colors=CP,styles="[]",\>points,w=0.2,x=0.3,y=0.4):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1026.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1026.png)

Plot kolom 3D menunjukkan deretan data statistik dalam bentuk kolom.
Kami menyediakan label untuk baris dan kolom. angle adalah sudut
pandang.


\>columnsplot3d(BT,scols=P,srows=YT, ...  
\>     angle=30°,ccols=CP):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1027.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1027.png)

Representasi lainnya adalah plot mosaik. Perhatikan bahwa kolom-kolom
pada plot mewakili kolom-kolom pada matriks di sini. Karena panjangnya
label CDU/CSU, kita mengambil jendela yang lebih kecil dari biasanya.


\>shrinkwindow(\>smaller);  ...  
\>   mosaicplot(BT',srows=YT,scols=P,color=CP,style="#"); ...  
\>   shrinkwindow():


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1028.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1028.png)

Kita juga bisa membuat diagram lingkaran. Karena warna hitam dan
kuning membentuk koalisi, kita menyusun ulang elemen-elemennya.


\>i=[1,3,5,4,2]; piechart(BW[6,3:7][i],color=CP[i],lab=P[i]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1029.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1029.png)

Berikut ini jenis plot yang lain.


\>starplot(normal(1,10)+4,lab=1:10,\>rays):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1030.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1030.png)

Beberapa plot di plot2d bagus untuk statika. Berikut ini adalah plot
impuls dari data acak, yang terdistribusi secara seragam dalam [0,1].


\>plot2d(makeimpulse(1:10,random(1,10)),\>bar):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1031.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1031.png)

Tetapi untuk data yang terdistribusi secara eksponensial, kita mungkin
memerlukan plot logaritmik.


\>logimpulseplot(1:10,-log(random(1,10))\*10):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1032.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1032.png)

Fungsi columnsplot() lebih mudah digunakan, karena hanya membutuhkan
sebuah vektor nilai. Selain itu, fungsi ini dapat mengatur labelnya
menjadi apa pun yang kita inginkan, kita telah mendemonstrasikan hal
ini dalam tutorial ini.


Berikut ini adalah aplikasi lain, di mana kita menghitung karakter
dalam sebuah kalimat dan memplot statistik.


\>v=strtochar("the quick brown fox jumps over the lazy dog"); ...  
\>   w=ascii("a"):ascii("z"); x=getmultiplicities(w,v); ...  
\>   cw=[]; for k=w; cw=cw|char(k); end; ...  
\>   columnsplot(x,lab=cw,width=0.05):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1033.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1033.png)

Anda juga dapat menetapkan sumbu secara manual.


\>n=10; p=0.4; i=0:n; x=bin(n,i)\*p^i\*(1-p)^(n-i); ...  
\>   columnsplot(x,lab=i,width=0.05,<frame,<grid); ...  
\>   yaxis(0,0:0.1:1,style="-\>",\>left); xaxis(0,style="."); ...  
\>   label("p",0,0.25), label("i",11,0); ...  
\>   textbox(["Binomial distribution","with p=0.4"]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1034.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1034.png)

Berikut ini adalah cara untuk memplot frekuensi angka dalam vektor.


Kami membuat vektor angka acak bilangan bulat 1 hingga 10.


\>v:=intrandom(1,10,10)


    [8,  5,  8,  8,  6,  8,  8,  3,  5,  5]

Kemudian ekstrak nomor unik dalam v.


\>vu:=unique(v)


    [3,  5,  6,  8]

Dan memplot frekuensi dalam plot kolom.


\>columnsplot(getmultiplicities(vu,v),lab=vu,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1035.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1035.png)

Kami ingin mendemonstrasikan fungsi untuk distribusi nilai empiris.


\>x=normal(1,20);


Fungsi empdist(x,vs) membutuhkan larik nilai yang telah diurutkan.
Jadi kita harus mengurutkan x sebelum dapat menggunakannya.


\>xs=sort(x);


Kemudian kita memplot distribusi empiris dan beberapa batang kepadatan
ke dalam satu plot. Alih-alih plot batang untuk distribusi, kali ini
kami menggunakan plot gigi gergaji.


\>figure(2,1); ...  
\>   figure(1); plot2d("empdist",-4,4;xs); ...  
\>   figure(2); plot2d(histo(x,v=-4:0.2:4,<bar));  ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1036.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1036.png)

Plot sebaran mudah dilakukan di Euler dengan plot titik biasa. Grafik
berikut ini menunjukkan bahwa X dan X+Y berkorelasi positif secara
jelas.


\>x=normal(1,100); plot2d(x,x+rotright(x),\>points,style=".."):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1037.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1037.png)

Sering kali, kita ingin membandingkan dua sampel dari distribusi yang
berbeda. Hal ini dapat dilakukan dengan plot kuantil-kuantil.


Untuk pengujian, kami mencoba distribusi student-t dan distribusi
eksponensial.


\>x=randt(1,1000,5); y=randnormal(1,1000,mean(x),dev(x)); ...  
\>   plot2d("x",r=6,style="--",yl="normal",xl="student-t",\>vertical); ...  
\>   plot2d(sort(x),sort(y),\>points,color=red,style="x",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1038.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1038.png)

Plot ini dengan jelas menunjukkan bahwa nilai yang terdistribusi
normal cenderung lebih kecil pada ujung yang ekstrim.


Jika kita memiliki dua distribusi dengan ukuran yang berbeda, kita
dapat memperluas distribusi yang lebih kecil atau memperkecil
distribusi yang lebih besar. Fungsi berikut ini bagus untuk keduanya.
Fungsi ini mengambil nilai median dengan persentase antara 0 dan 1.


\>function medianexpand (x,n) := median(x,p=linspace(0,1,n-1));


Mari kita bandingkan dua distribusi yang sama.


\>x=random(1000); y=random(400); ...  
\>   plot2d("x",0,1,style="--"); ...  
\>   plot2d(sort(medianexpand(x,400)),sort(y),\>points,color=red,style="x",\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1039.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1039.png)

# Regresi dan Korelasi

Regresi linier dapat dilakukan dengan fungsi polyfit() atau berbagai
fungsi kecocokan.


Sebagai permulaan, kita mencari garis regresi untuk data univariat
dengan polyfit(x,y,1).


\>x=1:10; y=[2,3,1,5,6,3,7,8,9,8]; writetable(x'|y',labc=["x","y"])


             x         y
             1         2
             2         3
             3         1
             4         5
             5         6
             6         3
             7         7
             8         8
             9         9
            10         8

Kami ingin membandingkan kecocokan tanpa bobot dan dengan bobot.
Pertama, koefisien dari kecocokan linier.


\>p=polyfit(x,y,1)


    [0.733333,  0.812121]

Sekarang, koefisien dengan bobot yang menekankan nilai terakhir.


\>w &= "exp(-(x-10)^2/10)"; pw=polyfit(x,y,1,w=w(x))


    [4.71566,  0.38319]

Kami menempatkan semuanya ke dalam satu plot untuk titik-titik dan
garis regresi, dan untuk bobot yang digunakan.


\>figure(2,1);  ...  
\>   figure(1); statplot(x,y,"b",xl="Regression"); ...  
\>     plot2d("evalpoly(x,p)",\>add,color=blue,style="--"); ...  
\>     plot2d("evalpoly(x,pw)",5,10,\>add,color=red,style="--"); ...  
\>   figure(2); plot2d(w,1,10,\>filled,style="/",fillcolor=red,xl=w); ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1040.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1040.png)

Untuk contoh lain, kita membaca survei tentang siswa, usia mereka,
usia orang tua mereka, dan jumlah saudara kandung dari sebuah file.


Tabel ini berisi "m" dan "f" pada kolom kedua. Kita menggunakan
variabel tok2 untuk mengatur terjemahan yang tepat dan bukannya
membiarkan readtable() mengumpulkan terjemahan.


\>{MS,hd}:=readtable("table1.dat",tok2:=["m","f"]);  ...  
\>   writetable(MS,labc=hd,tok2:=["m","f"]);


        Person       Sex       Age    Mother    Father  Siblings
             1         m        29        58        61         1
             2         f        26        53        54         2
             3         m        24        49        55         1
             4         f        25        56        63         3
             5         f        25        49        53         0
             6         f        23        55        55         2
             7         m        23        48        54         2
             8         m        27        56        58         1
             9         m        25        57        59         1
            10         m        24        50        54         1
            11         f        26        61        65         1
            12         m        24        50        52         1
            13         m        29        54        56         1
            14         m        28        48        51         2
            15         f        23        52        52         1
            16         m        24        45        57         1
            17         f        24        59        63         0
            18         f        23        52        55         1
            19         m        24        54        61         2
            20         f        23        54        55         1

Bagaimana usia saling bergantung satu sama lain? Kesan pertama datang
dari scatterplot berpasangan.


\>scatterplots(tablecol(MS,3:5),hd[3:5]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1041.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1041.png)

Jelas bahwa usia ayah dan ibu saling bergantung satu sama lain. Mari
kita tentukan dan plot garis regresinya.


\>cs:=MS[,4:5]'; ps:=polyfit(cs[1],cs[2],1)


    [17.3789,  0.740964]

Ini jelas merupakan model yang salah. Garis regresinya adalah s = 17 +
0,74t, di mana t adalah usia ibu dan s adalah usia ayah. Perbedaan
usia mungkin sedikit bergantung pada usia, tetapi tidak terlalu
banyak.


Sebaliknya, kami menduga fungsi seperti s = a + t. Kemudian a adalah
rata-rata dari s-t. Ini adalah perbedaan usia rata-rata antara ayah
dan ibu.


\>da:=mean(cs[2]-cs[1])


    3.65

Mari kita plotkan ini ke dalam satu scatter plot.


\>plot2d(cs[1],cs[2],\>points);  ...  
\>   plot2d("evalpoly(x,ps)",color=red,style=".",\>add);  ...  
\>   plot2d("x+da",color=blue,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1042.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1042.png)

Berikut ini adalah plot kotak dari kedua usia tersebut. Ini hanya
menunjukkan, bahwa usia keduanya berbeda.


\>boxplot(cs,["mothers","fathers"]):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1043.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1043.png)

Sangat menarik bahwa perbedaan dalam median tidak sebesar perbedaan
dalam mean.


\>median(cs[2])-median(cs[1])


    1.5

Koefisien korelasi menunjukkan korelasi positif.


\>correl(cs[1],cs[2])


    0.7588307236

Korelasi peringkat adalah ukuran untuk urutan yang sama dalam kedua
vektor. Korelasi ini juga cukup positif.


\>rankcorrel(cs[1],cs[2])


    0.758925292358

# Membuat Fungsi baru

Tentu saja, bahasa EMT dapat digunakan untuk memprogram fungsi baru.
Sebagai contoh, kita mendefinisikan fungsi kemiringan.


$$\text{sk}(x) = \dfrac{\sqrt{n} \sum_i (x_i-m)^3}{\left(\sum_i (x_i-m)^2\right)^{3/2}}$$di mana m adalah rata-rata dari x.


\>function skew (x:vector) ...


    m=mean(x);
    return sqrt(cols(x))*sum((x-m)^3)/(sum((x-m)^2))^(3/2);
    endfunction
</pre>
Seperti yang Anda lihat, kita dapat dengan mudah menggunakan bahasa
matriks untuk mendapatkan implementasi yang sangat singkat dan
efisien. Mari kita coba fungsi ini.


\>data=normal(20); skew(normal(10))


    -0.198710316203

Berikut ini adalah fungsi lain, yang disebut koefisien kemencengan
Pearson.


\>function skew1 (x) := 3\*(mean(x)-median(x))/dev(x)

\>skew1(data)


    -0.0801873249135

# Simulasi Monte Carlo

Euler dapat digunakan untuk mensimulasikan kejadian acak. Kita telah
melihat contoh sederhana di atas. Berikut ini adalah contoh lainnya,
yang mensimulasikan 1000 kali pelemparan 3 dadu, dan menanyakan
distribusi dari jumlah tersebut.


\>ds:=sum(intrandom(1000,3,6))';  fs=getmultiplicities(3:18,ds)


    [5,  17,  35,  44,  75,  97,  114,  116,  143,  116,  104,  53,  40,
    22,  13,  6]

Kita bisa plot ini sekarang.


\>columnsplot(fs,lab=3:18):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1045.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1045.png)

Untuk menentukan distribusi yang diharapkan tidaklah mudah. Kami
menggunakan rekursi tingkat lanjut untuk hal ini.


Fungsi berikut ini menghitung jumlah cara angka k dapat
direpresentasikan sebagai jumlah n angka dalam rentang 1 hingga m.
Fungsi ini bekerja secara rekursif dengan cara yang jelas.


\>function map countways (k; n, m) ...


      if n==1 then return k>=1 && k<=m
      else
        sum=0; 
        loop 1 to m; sum=sum+countways(k-#,n-1,m); end;
        return sum;
      end;
    endfunction
</pre>
Berikut ini adalah hasil dari tiga lemparan dadu.


\>countways(5:25,5,5)


    [1,  5,  15,  35,  70,  121,  185,  255,  320,  365,  381,  365,  320,
    255,  185,  121,  70,  35,  15,  5,  1]

\>cw=countways(3:18,3,6)


    [1,  3,  6,  10,  15,  21,  25,  27,  27,  25,  21,  15,  10,  6,  3,
    1]

Kami menambahkan nilai yang diharapkan ke plot.


\>plot2d(cw/6^3\*1000,\>add); plot2d(cw/6^3\*1000,\>points,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1046.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1046.png)

Untuk simulasi lainnya, deviasi nilai rata-rata dari n variabel acak
berdistribusi normal 0-1 adalah 1/sqrt(n).


\>longformat; 1/sqrt(10)


    0.316227766017

Mari kita periksa dengan sebuah simulasi. Kami menghasilkan 10.000
kali 10 vektor acak.


\>M=normal(10000,10); dev(mean(M)')


    0.319493614817

\>plot2d(mean(M)',\>distribution):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1047.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1047.png)

Median dari 10 bilangan acak berdistribusi normal 0-1 memiliki deviasi
yang lebih besar.


\>dev(median(M)')


    0.374460271535

Karena kita dapat dengan mudah menghasilkan jalan acak, kita dapat
mensimulasikan proses Wiener. Kami mengambil 1000 langkah dari 1000
proses. Kami kemudian memplot deviasi standar dan rata-rata dari
langkah ke-n dari proses-proses ini bersama dengan nilai yang
diharapkan dalam warna merah.


\>n=1000; m=1000; M=cumsum(normal(n,m)/sqrt(m)); ...  
\>   t=(1:n)/n; figure(2,1); ...  
\>   figure(1); plot2d(t,mean(M')'); plot2d(t,0,color=red,\>add); ...  
\>   figure(2); plot2d(t,dev(M')'); plot2d(t,sqrt(t),color=red,\>add); ...  
\>   figure(0):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1048.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1048.png)

# Tes

Tes adalah alat yang penting dalam statistik. Dalam Euler, banyak tes
yang diterapkan. Semua tes ini mengembalikan kesalahan yang kita
terima jika kita menolak hipotesis nol.


Sebagai contoh, kita menguji lemparan dadu untuk distribusi yang
seragam. Pada 600 lemparan, kita mendapatkan nilai berikut, yang kita
masukkan ke dalam uji chi-kuadrat.


\>chitest([90,103,114,101,103,89],dup(100,6)')


    0.498830517952

Uji chi-square juga memiliki mode, yang menggunakan simulasi Monte
Carlo untuk menguji statistik. Hasilnya seharusnya hampir sama.
Parameter &gt;p menginterpretasikan vektor y sebagai vektor probabilitas.


\>chitest([90,103,114,101,103,89],dup(1/6,6)',\>p,\>montecarlo)


    0.526

Kesalahan ini terlalu besar. Jadi kita tidak bisa menolak distribusi
seragam. Ini tidak membuktikan bahwa dadu kita adil. Tetapi kita tidak
bisa menolak hipotesis kita.


Selanjutnya kita buat 1000 lemparan dadu dengan menggunakan generator
bilangan acak, dan lakukan pengujian yang sama.


\>n=1000; t=random([1,n\*6]); chitest(count(t\*6,6),dup(n,6)')


    0.528028118442

Mari kita uji nilai rata-rata 100 dengan uji-t.


\>s=200+normal([1,100])\*10; ...  
\>   ttest(mean(s),dev(s),100,200)


    0.0218365848476

Fungsi ttest() membutuhkan nilai rata-rata, deviasi, jumlah data, dan
nilai rata-rata untuk diuji.


Sekarang mari kita periksa dua pengukuran untuk mean yang sama. Kita
tolak hipotesis bahwa kedua pengukuran tersebut memiliki nilai
rata-rata yang sama, jika hasilnya &lt;0,05.


\>tcomparedata(normal(1,10),normal(1,10))


    0.38722000942

Jika kita menambahkan bias pada satu distribusi, kita akan mendapatkan
lebih banyak penolakan. Ulangi simulasi ini beberapa kali untuk
melihat efeknya.


\>tcomparedata(normal(1,10),normal(1,10)+2)


    5.60009101758e-07

Pada contoh berikut, kita membuat 20 lemparan dadu secara acak
sebanyak 100 kali dan menghitung jumlah dadu yang muncul. Rata-rata
harus ada 20/6 = 3,3 mata dadu.


\>R=random(100,20); R=sum(R\*6<=1)'; mean(R)


    3.28

Sekarang kita bandingkan jumlah satu dengan distribusi binomial.
Pertama, kita memplot distribusi angka satu.


\>plot2d(R,distribution=max(R)+1,even=1,style="\\/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1049.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1049.png)

\>t=count(R,21);


Kemudian kita menghitung nilai yang diharapkan.


\>n=0:20; b=bin(20,n)\*(1/6)^n\*(5/6)^(20-n)\*100;


Kita harus mengumpulkan beberapa angka untuk mendapatkan kategori yang
cukup besar.


\>t1=sum(t[1:2])|t[3:7]|sum(t[8:21]); ...  
\>   b1=sum(b[1:2])|b[3:7]|sum(b[8:21]);


Uji chi-square menolak hipotesis bahwa distribusi kita adalah
distribusi binomial, jika hasilnya &lt;0,05.


\>chitest(t1,b1)


    0.53921579764

Contoh berikut ini berisi hasil dari dua kelompok orang (laki-laki dan
perempuan, katakanlah) yang memberikan suara untuk satu dari enam
partai.


\>A=[23,37,43,52,64,74;27,39,41,49,63,76];  ...  
\>     writetable(A,wc=6,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m    23    37    43    52    64    74
         f    27    39    41    49    63    76

Kami ingin menguji independensi suara dari jenis kelamin. Uji tabel
chi^2 melakukan hal ini. Hasilnya terlalu besar untuk menolak
independensi. Jadi kita tidak dapat mengatakan, jika pemungutan suara
tergantung pada jenis kelamin dari data ini.


\>tabletest(A)


    0.990701632326

Berikut ini adalah tabel yang diharapkan, jika kita mengasumsikan
frekuensi pemungutan suara yang diamati.


\>writetable(expectedtable(A),wc=6,dc=1,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m  24.9  37.9  41.9  50.3  63.3  74.7
         f  25.1  38.1  42.1  50.7  63.7  75.3

Kita dapat menghitung koefisien kontingensi yang telah dikoreksi.
Karena koefisien ini sangat dekat dengan 0, kami menyimpulkan bahwa
pemungutan suara tidak bergantung pada jenis kelamin.


\>contingency(A)


    0.0427225484717

# Beberapa Tes Lainnya

Selanjutnya kita menggunakan analisis varians (uji F) untuk menguji
tiga sampel data yang terdistribusi secara normal dengan nilai
rata-rata yang sama. Metode ini disebut ANOVA (analisis varians).
Dalam Euler, fungsi varanalysis() digunakan.


\>x1=[109,111,98,119,91,118,109,99,115,109,94]; mean(x1),


    106.545454545

\>x2=[120,124,115,139,114,110,113,120,117]; mean(x2),


    119.111111111

\>x3=[120,112,115,110,105,134,105,130,121,111]; mean(x3)


    116.3

\>varanalysis(x1,x2,x3)


    0.0138048221371

Ini berarti, kami menolak hipotesis nilai rata-rata yang sama. Kami
melakukan ini dengan probabilitas kesalahan sebesar 1,3%.


Ada juga uji median, yang menolak sampel data dengan distribusi
rata-rata yang berbeda dengan menguji median dari sampel gabungan.


\>a=[56,66,68,49,61,53,45,58,54];

\>b=[72,81,51,73,69,78,59,67,65,71,68,71];

\>mediantest(a,b)


    0.0241724220052

Uji lain tentang kesetaraan adalah uji peringkat. Uji ini jauh lebih
tajam daripada uji median.


\>ranktest(a,b)


    0.00199969612469

Dalam contoh berikut ini, kedua distribusi memiliki rata-rata yang
sama.


\>ranktest(random(1,100),random(1,50)\*3-1)


    0.129608141484

Sekarang mari kita coba mensimulasikan dua perlakuan a dan b yang
diterapkan pada orang yang berbeda.


\>a=[8.0,7.4,5.9,9.4,8.6,8.2,7.6,8.1,6.2,8.9];

\>b=[6.8,7.1,6.8,8.3,7.9,7.2,7.4,6.8,6.8,8.1];


Uji signum memutuskan, apakah a lebih baik daripada b.


\>signtest(a,b)


    0.0546875

Ini adalah kesalahan yang terlalu besar. Kita tidak dapat menolak
bahwa a sama baiknya dengan b.


Uji Wilcoxon lebih tajam daripada uji ini, tetapi bergantung pada
nilai kuantitatif dari perbedaan.


\>wilcoxon(a,b)


    0.0296680599405

Mari kita coba dua pengujian lagi dengan menggunakan rangkaian yang
dihasilkan.


\>wilcoxon(normal(1,20),normal(1,20)-1)


    0.0068706451766

\>wilcoxon(normal(1,20),normal(1,20))


    0.275145971064

# Bilangan Acak

Berikut ini adalah tes untuk generator bilangan acak. Euler
menggunakan generator yang sangat bagus, jadi kita tidak perlu
mengharapkan adanya masalah.


Pertama, kita akan membangkitkan sepuluh juta bilangan acak dalam
[0,1].


\>n:=10000000; r:=random(1,n);


Selanjutnya, kami menghitung jarak antara dua angka yang kurang dari
0,05.


\>a:=0.05; d:=differences(nonzeros(r<a));


Terakhir, kami memplot beberapa kali, setiap interval jarak yang
terjadi, dan membandingkannya dengan nilai yang diharapkan.


\>m=getmultiplicities(1:100,d); plot2d(m); ...  
\>     plot2d("n\*(1-a)^(x-1)\*a^2",color=red,\>add):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1050.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1050.png)

Menghapus data.


\>remvalue n;


# Pengantar untuk Pengguna Proyek R

Jelas, EMT tidak bersaing dengan R sebagai sebuah paket statistik.
Namun, ada banyak prosedur dan fungsi statistik yang tersedia di EMT
juga. Jadi EMT dapat memenuhi kebutuhan dasar. Bagaimanapun, EMT hadir
dengan paket numerik dan sistem aljabar komputer.


Notebook ini diperuntukkan bagi Anda yang sudah terbiasa dengan R,
tetapi perlu mengetahui perbedaan sintaks EMT dan R. Kami mencoba
memberikan gambaran umum mengenai hal-hal yang jelas dan kurang jelas
yang perlu Anda ketahui.


Selain itu, kami juga membahas cara-cara untuk bertukar data di antara
kedua sistem tersebut.


Perhatikan bahwa ini adalah pekerjaan yang sedang berlangsung.


# Sintaks Dasar

Hal pertama yang Anda pelajari dalam R adalah membuat sebuah vektor.
Dalam EMT, perbedaan utamanya adalah operator : dapat mengambil ukuran
langkah. Selain itu, operator ini memiliki daya ikat yang rendah.


\>n=10; 0:n/20:n-1


    [0,  0.5,  1,  1.5,  2,  2.5,  3,  3.5,  4,  4.5,  5,  5.5,  6,  6.5,
    7,  7.5,  8,  8.5,  9]

Fungsi c() tidak ada. Anda dapat menggunakan vektor untuk
menggabungkan beberapa hal.


Contoh berikut ini, seperti banyak contoh lainnya, berasal dari "
Pengantar ke R" yang disertakan dengan proyek R. Jika Anda membaca PDF
ini, Anda akan menemukan bahwa saya mengikuti alurnya dalam tutorial
ini.


\>x=[10.4, 5.6, 3.1, 6.4, 21.7]; [x,0,x]


    [10.4,  5.6,  3.1,  6.4,  21.7,  0,  10.4,  5.6,  3.1,  6.4,  21.7]

Operator titik dua dengan ukuran langkah EMT digantikan oleh fungsi
seq() dalam R. Kita dapat menulis fungsi ini dalam EMT.


\>function seq(a,b,c) := a:b:c; ...  
\>   seq(0,-0.1,-1)


    [0,  -0.1,  -0.2,  -0.3,  -0.4,  -0.5,  -0.6,  -0.7,  -0.8,  -0.9,  -1]

Fungsi rep() dari R tidak ada dalam EMT. Untuk input vektor, dapat
dituliskan sebagai berikut.


\>function rep(x:vector,n:index) := flatten(dup(x,n)); ...  
\>   rep(x,2)


    [10.4,  5.6,  3.1,  6.4,  21.7,  10.4,  5.6,  3.1,  6.4,  21.7]

Perhatikan bahwa "=" atau ":=" digunakan untuk perintah. Operator "-&gt;"
digunakan untuk menggunakan unit dalam EMT.


\>125km -\> " miles"


    77.6713990297 miles

Operator "&lt;-" untuk penugasan menyesatkan, dan bukan ide yang baik
untuk R. Berikut ini akan membandingkan a dan -4 dalam EMT. 


\>a=2; a<-4


    0

Dalam R, "a&lt;-4&lt;3" bisa digunakan, tetapi "a&lt;-4&lt;-3" tidak. Saya juga
mengalami ambiguitas yang sama di EMT, tetapi saya mencoba untuk
menghilangkannya.


EMT dan R memiliki vektor dengan tipe boolean. Tetapi dalam EMT, angka
0 dan 1 digunakan untuk merepresentasikan salah dan benar. Dalam R,
nilai benar dan salah tetap dapat digunakan dalam aritmatika biasa
seperti dalam EMT.


\>x<5, %\*x


    [0,  0,  1,  0,  0]
    [0,  0,  3.1,  0,  0]

EMT melempar kesalahan atau menghasilkan NAN tergantung pada flag
"kesalahan".


\>errors off; 0/0, isNAN(sqrt(-1)), errors on;


    NAN
    1

String sama saja dalam R dan EMT. Keduanya berada di lingkup lokal
saat ini, bukan di Unicode.


Dalam R ada paket-paket untuk Unicode. Dalam EMT, sebuah string dapat
berupa string Unicode. Sebuah string Unicode dapat diterjemahkan ke
pengkodean lokal dan sebaliknya. Selain itu, u"..." dapat berisi
entitas HTML.


\>u"&#169; Ren&eacut; Grothmann"


    © René Grothmann

Berikut ini mungkin atau mungkin tidak ditampilkan dengan benar pada
sistem Anda sebagai A dengan titik dan tanda hubung di atasnya. Hal
ini tergantung pada jenis huruf yang Anda gunakan.


\>chartoutf([480])


    Ǡ

Penggabungan string dilakukan dengan "+" atau "|". Ini dapat
menyertakan angka, yang akan dicetak dalam format saat ini.


\>"pi = "+pi


    pi = 3.14159265359

# Pengindeksan

Sebagian besar waktu, ini akan bekerja seperti pada R.


Tetapi EMT akan menginterpretasikan indeks negatif dari bagian
belakang vektor, sementara R menginterpretasikan x[n] sebagai x tanpa
elemen ke-n.


\>x, x[1:3], x[-2]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [10.4,  5.6,  3.1]
    6.4

Perilaku R dapat dicapai dalam EMT dengan drop().


\>drop(x,2)


    [10.4,  3.1,  6.4,  21.7]

Vektor logika tidak diperlakukan secara berbeda dengan indeks di EMT,
berbeda dengan R. Anda harus mengekstrak elemen-elemen yang bukan nol
terlebih dahulu di EMT.


\>x, x\>5, x[nonzeros(x\>5)]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [1,  1,  0,  1,  1]
    [10.4,  5.6,  6.4,  21.7]

Sama seperti dalam R, vektor indeks dapat berisi pengulangan.


\>x[[1,2,2,1]]


    [10.4,  5.6,  5.6,  10.4]

Namun pemberian nama untuk indeks tidak dimungkinkan dalam EMT. Untuk
paket statistik, hal ini mungkin sering diperlukan untuk memudahkan
akses ke elemen-elemen vektor.


Untuk meniru perilaku ini, kita dapat mendefinisikan sebuah fungsi
sebagai berikut.


\>function sel (v,i,s) := v[indexof(s,i)]; ...  
\>   s=["first","second","third","fourth"]; sel(x,["first","third"],s)


    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    [10.4,  3.1]

# Tipe Data

EMT memiliki lebih banyak tipe data yang tetap dibandingkan R. Jelas,
dalam R terdapat vektor yang berkembang. Anda bisa mengatur sebuah
vektor numerik kosong v dan memberikan sebuah nilai pada elemen v[17].
Hal ini tidak mungkin dilakukan dalam EMT.


Hal berikut ini sedikit tidak efisien.


\>v=[]; for i=1 to 10000; v=v|i; end;


EMT sekarang akan membuat vektor dengan v dan i yang ditambahkan pada
tumpukan dan menyalin vektor tersebut kembali ke variabel global v.


Semakin efisien mendefinisikan vektor.


\>v=zeros(10000); for i=1 to 10000; v[i]=i; end;


Untuk mengubah jenis tanggal di EMT, Anda dapat menggunakan fungsi
seperti complex().


\>complex(1:4)


    [ 1+0i ,  2+0i ,  3+0i ,  4+0i  ]

Konversi ke string hanya dapat dilakukan untuk tipe data dasar. Format
saat ini digunakan untuk penggabungan string sederhana. Tetapi ada
fungsi-fungsi seperti print() atau frac().


Untuk vektor, Anda dapat dengan mudah menulis fungsi Anda sendiri.


\>function tostr (v) ...


    s="[";
    loop 1 to length(v);
       s=s+print(v[#],2,0);
       if #<length(v) then s=s+","; endif;
    end;
    return s+"]";
    endfunction
</pre>
\>tostr(linspace(0,1,10))


    [0.00,0.10,0.20,0.30,0.40,0.50,0.60,0.70,0.80,0.90,1.00]

Untuk komunikasi dengan Maxima, ada sebuah fungsi convertmxm(), yang
juga dapat digunakan untuk memformat vektor untuk output.


\>convertmxm(1:10)


    [1,2,3,4,5,6,7,8,9,10]

Untuk Latex, perintah tex dapat digunakan untuk mendapatkan perintah
Latex.


\>tex(&[1,2,3])


    \left[ 1 , 2 , 3 \right] 

# Faktor dan Tabel

Pada pengantar R terdapat sebuah contoh dengan apa yang disebut
faktor.


Berikut ini adalah daftar wilayah dari 30 negara bagian.


\>austates = ["tas", "sa", "qld", "nsw", "nsw", "nt", "wa", "wa", ...  
\>   "qld", "vic", "nsw", "vic", "qld", "qld", "sa", "tas", ...  
\>   "sa", "nt", "wa", "vic", "qld", "nsw", "nsw", "wa", ...  
\>   "sa", "act", "nsw", "vic", "vic", "act"];


Asumsikan, kita memiliki pendapatan yang sesuai di setiap negara
bagian.


\>incomes = [60, 49, 40, 61, 64, 60, 59, 54, 62, 69, 70, 42, 56, ...  
\>   61, 61, 61, 58, 51, 48, 65, 49, 49, 41, 48, 52, 46, ...  
\>   59, 46, 58, 43];


Sekarang, kita ingin menghitung rata-rata pendapatan di wilayah
tersebut. Sebagai sebuah program statistik, R memiliki fungsi factor()
dan tappy() untuk hal ini.


EMT dapat melakukan hal ini dengan mencari indeks dari wilayah-wilayah
di dalam daftar unik dari wilayah-wilayah tersebut.


\>auterr=sort(unique(austates)); f=indexofsorted(auterr,austates)


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Pada titik ini, kita dapat menulis fungsi perulangan kita sendiri
untuk melakukan berbagai hal untuk satu faktor saja.


Atau kita dapat meniru fungsi tapply() dengan cara berikut.


\>function map tappl (i; f$:call, cat, x) ...


    u=sort(unique(cat));
    f=indexof(u,cat);
    return f$(x[nonzeros(f==indexof(u,i))]);
    endfunction
</pre>
Ini sedikit tidak efisien, karena menghitung wilayah unik untuk setiap
i, tetapi berfungsi.


\>tappl(auterr,"mean",austates,incomes)


    [44.5,  57.3333333333,  55.5,  53.6,  55,  60.5,  56,  52.25]

Perhatikan bahwa ini bekerja untuk setiap vektor wilayah.


\>tappl(["act","nsw"],"mean",austates,incomes)


    [44.5,  57.3333333333]

Sekarang, paket statistik EMT mendefinisikan tabel seperti halnya di
R. Fungsi readtable() dan writetable() dapat digunakan untuk input dan
output.


Jadi kita dapat mencetak rata-rata pendapatan negara di wilayah dengan
cara yang ramah.


\>writetable(tappl(auterr,"mean",austates,incomes),labc=auterr,wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

Kita juga dapat mencoba meniru perilaku R sepenuhnya.


Faktor-faktor tersebut harus disimpan dengan jelas dalam sebuah
koleksi dengan jenis dan kategorinya (negara bagian dan wilayah dalam
contoh kita). Untuk EMT, kita menambahkan indeks yang telah dihitung
sebelumnya.


\>function makef (t) ...


    ## Factor data
    ## Returns a collection with data t, unique data, indices.
    ## See: tapply
    u=sort(unique(t));
    return {{t,u,indexofsorted(u,t)}};
    endfunction
</pre>
\>statef=makef(austates);


Sekarang elemen ketiga dari koleksi ini akan berisi indeks.


\>statef[3]


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Sekarang kita dapat meniru tapply() dengan cara berikut. Ini akan
mengembalikan sebuah tabel sebagai kumpulan data tabel dan judul
kolom.


\>function tapply (t:vector,tf,f$:call) ...


    ## Makes a table of data and factors
    ## tf : output of makef()
    ## See: makef
    uf=tf[2]; f=tf[3]; x=zeros(length(uf));
    for i=1 to length(uf);
       ind=nonzeros(f==i);
       if length(ind)==0 then x[i]=NAN;
       else x[i]=f$(t[ind]);
       endif;
    end;
    return {{x,uf}};
    endfunction
</pre>
Kami tidak menambahkan banyak pemeriksaan tipe di sini. Satu-satunya
tindakan pencegahan adalah kategori (faktor) yang tidak memiliki data.
Tetapi kita harus memeriksa panjang t yang benar dan kebenaran koleksi
tf.


Tabel ini bisa dicetak sebagai sebuah tabel dengan writetable().


\>writetable(tapply(incomes,statef,"mean"),wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

# Array

EMT hanya memiliki dua dimensi untuk array. Tipe data ini disebut
matriks. Akan lebih mudah untuk menulis fungsi untuk dimensi yang
lebih tinggi atau sebuah pustaka C untuk ini.


R memiliki lebih dari dua dimensi. Dalam R, larik adalah sebuah vektor
dengan sebuah bidang dimensi.


Dalam EMT, sebuah vektor adalah sebuah matriks dengan satu baris. Ini
bisa dibuat menjadi sebuah matriks dengan redim().


\>shortformat; X=redim(1:20,4,5)


            1         2         3         4         5 
            6         7         8         9        10 
           11        12        13        14        15 
           16        17        18        19        20 

Ekstraksi baris dan kolom, atau sub-matriks, sama seperti di R.


\>X[,2:3]


            2         3 
            7         8 
           12        13 
           17        18 

Namun, dalam R dimungkinkan untuk mengatur daftar indeks tertentu dari
vektor ke suatu nilai. Hal yang sama juga dapat dilakukan dalam EMT
hanya dengan sebuah perulangan.


\>function setmatrixvalue (M, i, j, v) ...


    loop 1 to max(length(i),length(j),length(v))
       M[i{#},j{#}] = v{#};
    end;
    endfunction
</pre>
Kami mendemonstrasikan hal ini untuk menunjukkan bahwa matriks
diteruskan dengan referensi dalam EMT. Jika Anda tidak ingin mengubah
matriks asli M, Anda perlu menyalinnya dalam fungsi.


\>setmatrixvalue(X,1:3,3:-1:1,0); X,


            1         2         0         4         5 
            6         0         8         9        10 
            0        12        13        14        15 
           16        17        18        19        20 

Hasil kali luar dalam EMT hanya dapat dilakukan di antara vektor. Hal
ini otomatis karena bahasa matriks. Satu vektor harus berupa vektor
kolom dan vektor baris.


\>(1:5)\*(1:5)'


            1         2         3         4         5 
            2         4         6         8        10 
            3         6         9        12        15 
            4         8        12        16        20 
            5        10        15        20        25 

Dalam pengantar PDF untuk R ada sebuah contoh, yang menghitung
distribusi ab-cd untuk a, b, c, d yang dipilih dari 0 sampai n secara
acak. Solusinya dalam R adalah membentuk sebuah matriks 4 dimensi dan
menjalankan table() di atasnya.


Tentu saja, ini bisa dicapai dengan sebuah perulangan. Tetapi
perulangan tidak efektif dalam EMT atau R. Dalam EMT, kita bisa
menulis perulangan dalam C dan itu adalah solusi tercepat.


Tetapi kita ingin meniru perilaku R. Untuk ini, kita perlu meratakan
perkalian ab dan membuat sebuah matriks ab-cd.


\>a=0:6; b=a'; p=flatten(a\*b); q=flatten(p-p'); ...  
\>   u=sort(unique(q)); f=getmultiplicities(u,q); ...  
\>   statplot(u,f,"h"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1051.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1051.png)

Selain kelipatan yang tepat, EMT dapat menghitung frekuensi dalam
vektor.


\>getfrequencies(q,-50:10:50)


    [0,  23,  132,  316,  602,  801,  333,  141,  53,  0]

Cara yang paling mudah untuk memplot ini sebagai distribusi adalah
sebagai berikut.


\>plot2d(q,distribution=11):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1052.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1052.png)

Tetapi juga memungkinkan untuk menghitung jumlah dalam interval yang
dipilih sebelumnya. Tentu saja, berikut ini menggunakan
getfrequencies() secara internal.


Karena fungsi histo() mengembalikan frekuensi, kita perlu
menskalakannya sehingga integral di bawah grafik batang adalah 1.


\>{x,y}=histo(q,v=-55:10:55); y=y/sum(y)/differences(x); ...  
\>   plot2d(x,y,\>bar,style="/"):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1053.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1053.png)

# List

EMT memiliki dua jenis list. Pertama adalah list global yang dapat
diubah, dan yang kedua adalah tipe list yang tidak dapat diubah. Kita
tidak peduli dengan daftar global di sini.


Tipe daftar yang tidak dapat diubah disebut koleksi dalam EMT. Ia
berperilaku seperti struktur dalam C, tetapi elemen-elemennya hanya
diberi nomor dan tidak diberi nama.


\>L={{"Fred","Flintstone",40,[1990,1992]}}


    Fred
    Flintstone
    40
    [1990,  1992]

Saat ini elemen-elemen tersebut tidak memiliki nama, meskipun nama
dapat ditetapkan untuk tujuan khusus. Elemen-elemen tersebut diakses
dengan angka.


\>(L[4])[2]


    1992

# Input dan Output File (Membaca dan Menulis Data)

Anda mungkin sering ingin mengimpor matriks data dari sumber lain ke
EMT. Tutorial ini akan menjelaskan kepada Anda tentang berbagai cara
untuk melakukan hal tersebut. Fungsi yang sederhana adalah
writematrix() dan readmatrix().


Mari kita tunjukkan bagaimana cara membaca dan menulis sebuah vektor
real ke sebuah file.


\>a=random(1,100); mean(a), dev(a),


    0.49815
    0.28037

Untuk menulis data ke sebuah berkas, kita menggunakan fungsi
writematrix().


Karena pengenalan ini kemungkinan besar berada di sebuah direktori, di
mana pengguna tidak memiliki akses tulis, kami menulis data ke
direktori home pengguna. Untuk notebook sendiri, hal ini tidak
diperlukan, karena file data akan ditulis ke dalam direktori yang
sama.


\>filename="test.dat";


Sekarang kita tuliskan vektor kolom a' ke dalam file. Hal ini akan
menghasilkan satu angka pada setiap baris file.


\>writematrix(a',filename);


Untuk membaca data, kita menggunakan readmatrix().


\>a=readmatrix(filename)';


Dan hapus file tersebut.


\>fileremove(filename);

\>mean(a), dev(a),


    0.49815
    0.28037

Fungsi writematrix() atau writetable() dapat dikonfigurasi untuk
bahasa lain.


Sebagai contoh, jika Anda memiliki sistem bahasa Indonesia (titik
desimal dengan koma), Excel Anda membutuhkan nilai dengan koma desimal
yang dipisahkan oleh titik koma dalam file csv (defaultnya adalah
nilai yang dipisahkan dengan koma). File "test.csv" berikut ini akan
muncul di folder cuurent Anda.


\>filename="test.csv"; ...  
\>   writematrix(random(5,3),file=filename,separator=",");


Anda sekarang dapat membuka file ini dengan Excel Indonesia secara
langsung.


\>fileremove(filename);


Terkadang kita memiliki string dengan token seperti berikut ini.


\>s1:="f m m f m m m f f f m m f";  ...  
\>   s2:="f f f m m f f";


Untuk menandai ini, kita mendefinisikan vektor token.


\>tok:=["f","m"]


    f
    m

Kemudian kita dapat menghitung berapa kali setiap token muncul dalam
string, dan memasukkan hasilnya ke dalam tabel.


\>M:=getmultiplicities(tok,strtokens(s1))\_ ...  
\>     getmultiplicities(tok,strtokens(s2));


Tulis tabel dengan tajuk token.


\>writetable(M,labc=tok,labr=1:2,wc=8)


                   f       m
           1       6       7
           2       5       2

Untuk statika, EMT dapat membaca dan menulis tabel.


\>file="test.dat"; open(file,"w"); ...  
\>   writeln("A,B,C"); writematrix(random(3,3)); ...  
\>   close();


File terlihat seperti ini.


\>printfile(file)


    A,B,C
    0.7003664386138074,0.1875530821001213,0.3262339279660414
    0.5926249243193858,0.1522927283984059,0.368140583062521
    0.8065535209872989,0.7265910840408142,0.7332619844597152
    

Fungsi readtable() dalam bentuknya yang paling sederhana dapat membaca
ini dan mengembalikan sebuah koleksi nilai dan baris judul.


\>L=readtable(file,\>list);


Koleksi ini dapat dicetak dengan writetable() ke buku catatan, atau ke
sebuah file.


\>writetable(L,wc=10,dc=5)


             A         B         C
       0.70037   0.18755   0.32623
       0.59262   0.15229   0.36814
       0.80655   0.72659   0.73326

Matriks nilai adalah elemen pertama dari L. Perhatikan bahwa mean()
dalam EMT menghitung nilai rata-rata dari baris-baris matriks.


\>mean(L[1])


      0.40472 
      0.37102 
      0.75547 

# File CSV

Pertama, mari kita tulis sebuah matriks ke dalam sebuah file. Untuk
keluarannya, kami membuat file di direktori kerja saat ini.


\>file="test.csv";  ...  
\>   M=random(3,3); writematrix(M,file);


Berikut ini adalah isi file ini.Berikut ini adalah isi file ini.


\>printfile(file)


    0.8221197733097619,0.821531098722547,0.7771240608094004
    0.8482947121863489,0.3237767724883862,0.6501422353377985
    0.1482301827518109,0.3297459716109594,0.6261901074210923
    

CVS ini dapat dibuka di sistem bahasa Inggris ke Excel dengan klik dua
kali. Jika Anda mendapatkan file seperti itu pada sistem Jerman, Anda
perlu mengimpor data ke Excel dengan memperhatikan titik desimal.


Namun, titik desimal juga merupakan format default untuk EMT. Anda
dapat membaca sebuah matriks dari sebuah file dengan readmatrix().


\>readmatrix(file)


      0.82212   0.82153   0.77712 
      0.84829   0.32378   0.65014 
      0.14823   0.32975   0.62619 

Dimungkinkan untuk menulis beberapa matriks ke dalam satu file.
Perintah open() dapat membuka file untuk menulis dengan parameter "w".
Standarnya adalah "r" untuk membaca.


\>open(file,"w"); writematrix(M); writematrix(M'); close();


Matriks-matriks tersebut dipisahkan oleh sebuah baris kosong. Untuk
membaca matriks, buka file dan panggil readmatrix() beberapa kali.


\>open(file); A=readmatrix(); B=readmatrix(); A==B, close();


            1         0         0 
            0         1         0 
            0         0         1 

Di Excel atau spreadsheet serupa, Anda dapat mengekspor matriks
sebagai CSV (nilai yang dipisahkan dengan koma). Pada Excel 2007,
gunakan "save as" dan "format lain", lalu pilih "CSV". Pastikan, tabel
saat ini hanya berisi data yang ingin Anda ekspor.


Berikut ini adalah contohnya.


\>printfile("excel-data.csv")


    0;1000;1000
    1;1051,271096;1072,508181
    2;1105,170918;1150,273799
    3;1161,834243;1233,67806
    4;1221,402758;1323,129812
    5;1284,025417;1419,067549
    6;1349,858808;1521,961556
    7;1419,067549;1632,31622
    8;1491,824698;1750,6725
    9;1568,312185;1877,610579
    10;1648,721271;2013,752707

Seperti yang Anda lihat, sistem Jerman saya menggunakan titik koma
sebagai pemisah dan koma desimal. Anda dapat mengubahnya di pengaturan
sistem atau di Excel, tetapi tidak perlu untuk membaca matriks ke
dalam EMT.


Cara termudah untuk membaca ini ke dalam Euler adalah readmatrix().
Semua koma digantikan oleh titik dengan parameter &gt;comma. Untuk CSV
bahasa Inggris, hilangkan saja parameter ini.


\>M=readmatrix("excel-data.csv",\>comma)


            0      1000      1000 
            1    1051.3    1072.5 
            2    1105.2    1150.3 
            3    1161.8    1233.7 
            4    1221.4    1323.1 
            5      1284    1419.1 
            6    1349.9      1522 
            7    1419.1    1632.3 
            8    1491.8    1750.7 
            9    1568.3    1877.6 
           10    1648.7    2013.8 

Mari kita plot ini.


\>plot2d(M'[1],M'[2:3],\>points,color=[red,green]'):


![images/EMT_Annisa%20Nur%20Rohmah_22305141031-1054.png](images/EMT_Annisa%20Nur%20Rohmah_22305141031-1054.png)

Ada beberapa cara yang lebih mendasar untuk membaca data dari file.
Anda dapat membuka file dan membaca angka baris demi baris. Fungsi
getvectorline() akan membaca angka dari sebuah baris data. Secara
default, fungsi ini mengharapkan sebuah titik desimal. Tetapi fungsi
ini juga dapat menggunakan koma desimal, jika Anda memanggil
setdecimaldot(",") sebelum menggunakan fungsi ini.


Fungsi berikut ini adalah contohnya. Fungsi ini akan berhenti pada
akhir file atau baris kosong.


\>function myload (file) ...


    open(file);
    M=[];
    repeat
       until eof();
       v=getvectorline(3);
       if length(v)>0 then M=M_v; else break; endif;
    end;
    return M;
    close(file);
    endfunction
</pre>
\>myload(file)


      0.82212   0.82153   0.77712 
      0.84829   0.32378   0.65014 
      0.14823   0.32975   0.62619 

Anda juga dapat membaca semua angka di dalam file tersebut dengan
getvector().


\>open(file); v=getvector(10000); close(); redim(v[1:9],3,3)


      0.82212   0.82153   0.77712 
      0.84829   0.32378   0.65014 
      0.14823   0.32975   0.62619 

Dengan demikian, sangat mudah untuk menyimpan vektor nilai, satu nilai
di setiap baris dan membaca kembali vektor ini.


\>v=random(1000); mean(v)


    0.50303

\>writematrix(v',file); mean(readmatrix(file)')


    0.50303

# Menggunakan Tabel

Tabel dapat digunakan untuk membaca atau menulis data numerik. Sebagai
contoh, kita menulis tabel dengan judul baris dan kolom ke file.


\>file="test.tab"; M=random(3,3);  ...  
\>   open(file,"w");  ...  
\>   writetable(M,separator=",",labc=["one","two","three"]);  ...  
\>   close(); ...  
\>   printfile(file)


    one,two,three
          0.09,      0.39,      0.86
          0.39,      0.86,      0.71
           0.2,      0.02,      0.83

File ini dapat diimpor ke Excel.


Untuk membaca file di EMT, kita menggunakan readtable().


\>{M,headings}=readtable(file,\>clabs); ...  
\>   writetable(M,labc=headings)


           one       two     three
          0.09      0.39      0.86
          0.39      0.86      0.71
           0.2      0.02      0.83

# Menganalisis Baris

Anda bahkan dapat mengevaluasi setiap baris dengan tangan. Misalkan,
kita memiliki baris dengan format berikut.


\>line="2020-11-03,Tue,1'114.05"


    2020-11-03,Tue,1'114.05

Pertama, kita dapat memberi tanda pada baris.


\>vt=strtokens(line)


    2020-11-03
    Tue
    1'114.05

Kemudian, kita dapat mengevaluasi setiap elemen baris dengan
menggunakan evaluasi yang sesuai.


\>day(vt[1]),  ...  
\>   indexof(["mon","tue","wed","thu","fri","sat","sun"],tolower(vt[2])),  ...  
\>   strrepl(vt[3],"'","")()


    7.3816e+05
    2
    1114

Dengan menggunakan ekspresi reguler, Anda dapat mengekstrak hampir
semua informasi dari sebuah baris data.


Anggaplah kita memiliki baris dokumen HTML berikut ini.


\>line="<tr\><td\>1145.45</td\><td\>5.6</td\><td\>-4.5</td\><tr\>"


    &lt;tr&gt;&lt;td&gt;1145.45&lt;/td&gt;&lt;td&gt;5.6&lt;/td&gt;&lt;td&gt;-4.5&lt;/td&gt;&lt;tr&gt;

Untuk mengekstrak ini, kita menggunakan ekspresi reguler, yang mencari


 - tanda kurung tutup &gt;,  
 - setiap string yang tidak mengandung tanda kurung dengan  

sub-pencocokan "(...)",


 - kurung pembuka dan kurung penutup menggunakan solusi terpendek,


 - sekali lagi, semua string yang tidak mengandung tanda kurung,


 - dan sebuah kurung pembuka &lt;.


Ekspresi reguler agak sulit untuk dipelajari tetapi sangat kuat.


\>{pos,s,vt}=strxfind(line,"\>([^<\>]+)<.+?\>([^<\>]+)<");


Hasilnya adalah posisi kecocokan, string yang cocok, dan vektor string
untuk pencocokan.


\>for k=1:length(vt); vt[k](), end;


    1145.5
    5.6

Berikut ini adalah fungsi yang membaca semua item numerik antara &lt;td&gt;
dan &lt;/td&gt;.


\>function readtd (line) ...


    v=[]; cp=0;
    repeat
       {pos,s,vt}=strxfind(line,"<td.*?>(.+?)</td>",cp);
       until pos==0;
       if length(vt)>0 then v=v|vt[1]; endif;
       cp=pos+strlen(s);
    end;
    return v;
    endfunction
</pre>
\>readtd(line+"<td\>non-numerical</td\>")


    1145.45
    5.6
    -4.5
    non-numerical

# Membaca dari Web

Situs web atau file dengan URL dapat dibuka di EMT dan dapat dibaca
baris demi baris.


Dalam contoh, kita membaca versi saat ini dari situs EMT. Kami
menggunakan ekspresi reguler untuk memindai " Version ... " dalam
sebuah judul.


\>function readversion () ...


    urlopen("http://www.euler-math-toolbox.de/Programs/Changes.html");
    repeat
      until urleof();
      s=urlgetline();
      k=strfind(s,"Version ",1);
      if k>0 then substring(s,k,strfind(s,"<",k)-1), break; endif;
    end;
    urlclose();
    endfunction
</pre>
\>readversion


    Version 2022-05-18

# Masukan dan Keluaran Variabel

Anda dapat menulis variabel dalam bentuk definisi Euler ke file atau
ke baris perintah.


\>writevar(pi,"mypi");


    mypi = 3.141592653589793;

Untuk pengujian, kami membuat file Euler di direktori kerja EMT.


\>file="test.e"; ...  
\>   writevar(random(2,2),"M",file); ...  
\>   printfile(file,3)


    M = [ ..
    0.5991820585590205, 0.7960280262224293;
    0.5167243983231363, 0.2996684599070898];

Sekarang kita dapat memuat file tersebut. Ini akan mendefinisikan
matriks M.


\>load(file); show M,


    M = 
      0.59918   0.79603 
      0.51672   0.29967 

Sebagai catatan, jika writevar() digunakan pada sebuah variabel, maka
ia akan mencetak definisi variabel dengan nama variabel tersebut.


\>writevar(M); writevar(inch$)


    M = [ ..
    0.5991820585590205, 0.7960280262224293;
    0.5167243983231363, 0.2996684599070898];
    inch$ = 0.0254;

Kita juga dapat membuka file baru atau menambahkan ke file yang sudah
ada. Dalam contoh ini, kami menambahkan ke file yang telah dibuat
sebelumnya.


\>open(file,"a"); ...  
\>   writevar(random(2,2),"M1"); ...  
\>   writevar(random(3,1),"M2"); ...  
\>   close();

\>load(file); show M1; show M2;


    M1 = 
      0.30287   0.15372 
       0.7504   0.75401 
    M2 = 
      0.27213 
     0.053211 
      0.70249 

Untuk menghapus file, gunakan fileremove().


\>fileremove(file);


Sebuah vektor baris dalam sebuah file tidak membutuhkan koma, jika
setiap angka berada dalam baris baru. Mari kita buat file seperti itu,
menulis setiap baris satu per satu dengan writeln().


\>open(file,"w"); writeln("M = ["); ...  
\>   for i=1 to 5; writeln(""+random()); end; ...  
\>   writeln("];"); close(); ...  
\>   printfile(file)


    M = [
    0.344851384551
    0.0807510017715
    0.876519562911
    0.754157709472
    0.688392638934
    ];

\>load(file); M


    [0.34485,  0.080751,  0.87652,  0.75416,  0.68839]

