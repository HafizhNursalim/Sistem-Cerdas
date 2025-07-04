# Pengenalan Derajat Kebenaran (Degree of Truth)

Komputer umumnya bekerja dengan sistem biner yaitu:
1.   0 : Off jika tidak terdapat arus listrik
2.   1 : On jika terdapat arus listrik

Semua informasi yang disimpan oleh komputer disimpan dalam susunan biner atau disebut juga dengan bilangan biner. Dalam menjalankan program komputer, semua informasi akan diolah sehingga menghasilkan nilai kebenaran / derajat kebenaran:
1.   0 : Jika logika bernilai salah
2.   1 : Jika logika bernilai benar

     **Derajat kebenaran tersebut merupakan derajat kebenaran boolean**
     
Namun pada nyatanya, dalam kehidupan sehari-hari, nilai kebenaran ini bernilai relatif tergantung kondisi yang terjadi dari rentang 0 - 1 (**Derajat Kebenaran Fuzzy**). Sebagai contohnya ketika teman-teman yang berasal dari daerah pegunungan yang memiliki suhu 20 derajat Celcius pergi ke daerah perkotaan, teman-teman akan merasa bahwa:
1.   Suhu lingkungan 28 derajat Celcius merupakan suhu yang sangat panas (Derajat Kebenaran = 0.85)
2.   Suhu 26 derajat Celcius merupakan suhu yang panas (Derajat Kebenaran = 0.75)
3.   Suhu 18 derajat Celcius merupakan suhu yang sedikit dingin (Derajat Kebenaran = 0.55)
4.   Suhu 22 derajat Celcius merupakan suhu yang lumayan hangat (Derajat Kebenaran = 0.45)

Respon tubuh yang dihasilkan manusia terhadap suhu dalam bentuk rasa panas dan dingin ini relatif tergantung setiap orang.
1.   Semakin dekat nilai derajat kebenaran dengan 0 maka kondisi yang terjadi semakin mendekati nilai kesalahan (Jika ia 0 maka ia sudah pasti salah).
2.   Semakin dekat nilai derajat kebenaran dengan 1 maka kondisi yang terjadi semakin mendekati nilai kebenaran (Jika ia 1 maka ia sudah pasti benar).
3.   Jika derajat kebenaran bernilai 0.5 maka kondisi yang terjadi dalam keadan di tengah-tengah antara nilai benar dan salah.

      **Begitu juga dengan robot atau sistem otomatis. Robot atau sistem otomatis juga dapat mengkategorikan hal tersebut umumnya dalam derajat kebenaran fuzzy untuk menghadapi berbagai ketidakpastian dalam dunia nyata**

# Rule / Aturan

Dalam logika fuzzy, perlu diketahui terlebih dahulu bahwa apa yang dimaksud dengan rule / aturan, yaitu bagaimana kategori output yang keluar berdasarkan kategori variable inputnya. Pada program pemadam kebakaran ruangan tertutup, kita dapat menggunakan variabel input:
1.   Suhu dengan derajat kebenaran : Dingin, Normal, Panas
2.   Jarak Api dengan derajat kebenaran : Dekat, Sedikit Jauh, Jauh, Tidak Ada
3.   Asap dengan derajat kebenaran: Tipis, Sedang, Tebal

Sedangkan variable outputnya yaitu apa yang akan dilakukan oleh sistem terhadap kombinasi kondisi yang terjadi seperti:
1.   Kipas dengan derajat kebenaran : Lambat, Sedang, Cepat
2.   Pompa dengan derajat kebenaran : Singkat, Sedikit Lama, Lama

Ketika nilai ke3 variable tersebut dimasukkan maka setiap variable akan menentukan kategori derajat kebenarannya (sehingga diperoleh 3 kategori untuk 3 variable). Untuk mengetahui bagaimana kipas bergerak dan berapa lama pompa mengalir, maka diperlukan aturan. Salah satu contoh aturan pada program yang dibuat yaitu:

  Jika suhu panas dan asap tebal dan jarak api agak dekat maka kipas berputar cepat dan pompa air mengalir agak lama

# Logika Fuzzy (Fuzzy Logic)

Logika fuzzy merupakan logika yang melakukan penalaran terhadap setiap variable/anggotanya dengan derajat kebenaran anggota fuzzy (nilainya berada di antara 0 hingga 1) berdasarkan rule/aturan yang diberikan.

# Cara menggunakan program Matlab

Adapun cara menggunakan program yang diberikan pada Matlab (versi yang saya gunakan yaitu R2017a) sebagai berikut ini:
1.   Pergi ke bagian menu APP dan klik "fuzzy logic designer"

<img width="959" alt="image" src="https://github.com/user-attachments/assets/95805f3b-1d1b-4da8-9e4a-b2484e4f599b" />

2.   Kemudian klik file -> Import -> From File -> Kemudian Masukkan File

<img width="418" alt="image" src="https://github.com/user-attachments/assets/a5cb807f-7d0f-45f9-8d79-7b834c931419" />

3.   Setelah file dimasukkan, untuk menjalankannya klik bagian view -> Rules
4.   Untuk mengetahui hasil output  apa yang akan sistem lakukan bisa dengan memasukkan nilai pada variable input atau dengan menggeser garis merah pada variable input

<img width="418" alt="image" src="https://github.com/user-attachments/assets/a2890201-21a2-4f5c-8315-53a74fd94702" />

