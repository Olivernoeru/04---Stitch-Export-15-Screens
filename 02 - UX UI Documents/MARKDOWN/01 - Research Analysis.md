# **01 — Research Analysis** 

Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan 

**Keterangan sumber.** Dasar setiap pernyataan ditulis dengan kode berikut: **Q1–Q10** untuk pertanyaan kuesioner, **PDF** untuk dokumen Topik Proyek UI UJIAN, dan **Analisis** untuk kesimpulan yang ditarik dari data tersebut. 

## **1. Latar Belakang** 

Kekerasan dapat menempatkan korban dan orang di sekitarnya dalam situasi yang membingungkan. Mereka mungkin tidak mengetahui apa yang harus dilakukan lebih dahulu, ke mana mencari pertolongan, bagaimana memperoleh pendampingan atau bantuan hukum, layanan mana yang dapat dipercaya, dan hak apa yang dimiliki korban. Topik proyek ini berkaitan dengan dua Tujuan Pembangunan Berkelanjutan, yaitu SDG 5 tentang upaya mengurangi kekerasan terhadap perempuan dan anak perempuan, serta SDG 16 tentang akses masyarakat terhadap keadilan dan bantuan hukum. 

Masalah yang menjadi fokus dirumuskan dalam dokumen proyek sebagai berikut: kurangnya akses informasi yang sederhana dan terpusat mengenai langkah awal, layanan pendampingan, dan bantuan hukum bagi korban kekerasan. Solusi yang dirancang adalah aplikasi mobile bernama **Ruang Aman** (KK-4) yang mengumpulkan informasi dan akses layanan tersebut dalam satu tempat. 

Sebelum perancangan antarmuka dimulai, kuesioner disebarkan untuk memahami sejauh mana masyarakat mengetahui tempat mencari bantuan, hambatan apa yang dirasakan, informasi apa yang paling dibutuhkan, dan fitur apa yang diharapkan. Dokumen ini merangkum analisis data tersebut sebagai dasar bagi dokumen persona, kebutuhan, dan rancangan antarmuka. 

## **2. Tujuan Penelitian** 

Penelitian ini bertujuan untuk: 

1. Mengetahui tingkat pengetahuan responden tentang tempat mencari bantuan dan layanan bantuan hukum. 

2. Mengidentifikasi hambatan yang dirasakan ketika seseorang hendak mencari bantuan atas kasus kekerasan. 

3. Menentukan jenis informasi dan fitur yang paling dibutuhkan pada aplikasi. 

4. Mengetahui kebutuhan terhadap privasi serta preferensi cara penyajian informasi. 

5. Menyediakan dasar data bagi penyusunan persona, user stories, requirements, dan rancangan UX/UI Ruang Aman. 

## **3. Metode Penelitian** 

### **3.1 Kuesioner** 

Data kuantitatif dikumpulkan melalui kuesioner daring (Google Forms) yang disusun dan disebarkan. Instrumen memuat satu pertanyaan rentang usia, sepuluh pertanyaan inti (Q1–Q10), dan satu kolom pendapat atau komentar lain. Sebagian pertanyaan berformat pilihan tunggal (Q1, Q2, Q4–Q6, Q8–Q10) dan sebagian berformat pilihan ganda (Q3 dan Q7). Pertanyaan dirumuskan untuk masyarakat umum yang "mengalami atau mengetahui" adanya kekerasan, sehingga hasilnya menggambarkan **persepsi responden terhadap hambatan dan kebutuhan** , bukan catatan pengalaman pribadi korban. 

### **3.2 Wawancara** 

Wawancara melibatkan tiga partisipan yang telah ditentukan, yaitu Lili, RA (Riska Amalia), dan Syifa. Hasil wawancara digunakan untuk dua persona yang akan disajikan secara terpisah dalam slide presentasi. Dokumen User Persona pada knowledge base ini disusun berdasarkan pola kebutuhan dari kuesioner, sesuai keputusan proyek. Catatan wawancara tidak terdapat dalam ZIP yang diaudit sehingga tidak digunakan untuk mengisi atribut persona. 

### **3.3 Usability testing** 

Usability testing menggunakan partisipan yang telah ditentukan, yaitu Lili, RA (Riska Amalia), dan Syifa. Tujuannya mengevaluasi prototype, termasuk kemampuan menyelesaikan alur utama, menemukan tombol penting, dan memahami teks. Hasil pengujian belum terdapat dalam ZIP yang diaudit dan tidak direka dalam dokumen ini. 

### **3.4 Pengolahan data kuesioner** 

Jawaban dihitung ulang dari berkas spreadsheet asli yang memuat 20 respons lengkap. Analisis bersifat deskriptif, menggunakan frekuensi dan persentase terhadap 20 responden. Tabulasi silang sederhana dilakukan antara hambatan (Q3) dan pengetahuan tempat mencari bantuan (Q1). Persentase dibulatkan satu desimal. Pada pertanyaan pilihan ganda, jumlah pilihan dapat melebihi 20 sehingga persentase tidak dijumlahkan. 

## **4. Sumber Data** 

|Sumber|Bentuk|Status|Penggunaan|
|---|---|---|---|
|Kuesioner Akses Informasi|Spreadsheet, 20|Tersedia|Dasar analisis pada|
|dan Bantuan bagi Korban<br>Kekerasan|respons, 10<br>pertanyaan inti + usia +<br>komentar||dokumen ini|
|Topik Proyek UI UJIAN (PDF)|Rumusan masalah, use<br>case, 8 fitur usulan,|Tersedia|Konteks masalah,<br>lingkup, dan fitur|



|Sumber|Bentuk|Status|Penggunaan|
|---|---|---|---|
||daftar 15 halaman|||
|Wawancara (Lili, RA/Riska<br>Amalia, Syifa)|Hasil wawancara|Belum tersedia<br>dalam sumber<br>yang diaudit|Bahan terpisah untuk<br>slide presentasi setelah<br>wawancara|
|Usability testing (partisipan<br>yang sama)|Hasil pengujian|Belum tersedia<br>dalam sumber<br>yang diaudit|Evaluasi prototype<br>(Dokumen 06)|
|Data layanan (nama lembaga,<br>kontak, lokasi)|Data layanan|Belum tersedia<br>dalam ZIP|Konten Cari Layanan,<br>Peta, dan Detail Layanan|



## **5. Analisis Data Kuesioner** 

### **5.1 Profil responden** 

|Rentang usia|Jumlah|Persentase|
|---|---|---|
|23–27 tahun|12|60,0%|
|18–22 tahun|5|25,0%|
|Di atas 27 tahun|2|10,0%|
|Di bawah 18 tahun|1|5,0%|
|Total|20|100%|



Kuesioner tidak menanyakan jenis kelamin, wilayah, maupun pengalaman pribadi responden, sehingga profil responden hanya dapat digambarkan dari usia. 

### **5.2 Pengetahuan dan kemudahan akses informasi** 

|Pertanyaan|Jawaban|Jumlah|%|
|---|---|---|---|
|Q1. Mengetahui ke mana mencari bantuan|Ya, mengetahui|18|90,0|
||Kurang mengetahui|1|5,0|
||Tidak mengetahui|1|5,0|
|Q2. Informasi tempat pelaporan dan bantuan<br>mudah ditemukan|Mudah|12|60,0|
||Sangat mudah|2|10,0|
||Cukup sulit|5|25,0|



|Pertanyaan|Jawaban|Jumlah|%|
|---|---|---|---|
||Sulit|1|5,0|
|Q5. Masyarakat mengetahui layanan bantuan<br>hukum|Cukup mengetahui|9|45,0|
||Sangat mengetahui|2|10,0|
||Kurang mengetahui|8|40,0|
||Tidak mengetahui|1|5,0|
|Q6. Informasi hukum mudah dipahami|Mudah dipahami|9|45,0|
||Sangat mudah dipahami|2|10,0|
||Cukup sulit dipahami|9|45,0|



### **5.3 Hambatan (Q3, pilihan ganda)** 

|Hambatan|Jumlah|% dari 20 responden|
|---|---|---|
|Takut untuk melapor|16|80,0|
|Khawatir privasi atau identitas tidak terjaga|11|55,0|
|Tidak tahu harus menghubungi siapa|9|45,0|
|Tidak memahami prosedur|9|45,0|
|Khawatir mengenai biaya|8|40,0|
|Informasi sulit ditemukan|5|25,0|



Sebanyak 15 dari 20 responden memilih dua hambatan atau lebih, dan 9 responden memilih tiga hambatan atau lebih. Hambatan cenderung saling berlapis, bukan berdiri sendiri. 

### **5.4 Kebutuhan informasi dan fitur** 

|Pertanyaan|Jawaban|Jumlah|%|
|---|---|---|---|
|Q4. Informasi yang paling|Layanan pendampingan|6|30,0|
|dibutuhkan lebih dahulu||||
||Langkah awal yang harus dilakukan|7|35,0|
||Tempat atau layanan untuk melapor|5|25,0|
||Hak-hak korban|1|5,0|
||Bantuan hukum|1|5,0|



|Pertanyaan|Jawaban|Jumlah|%|
|---|---|---|---|
|Q7. Fitur yang paling<br>dibutuhkan (pilihan ganda)|Tombol bantuan cepat|18|90,0|
||Panduan langkah awal|8|40,0|
||Informasi bantuan hukum|8|40,0|
||Pencarian layanan bantuan|8|40,0|
||Informasi hak-hak korban|7|35,0|
|Q9. Penyajian informasi<br>paling mudah dipahami|Penjelasan singkat dengan bahasa sederhana|9|45,0|
||Panduan langkah demi langkah|6|30,0|
||Infografis atau ilustrasi|3|15,0|
||Video singkat|2|10,0|



### **5.5 Privasi dan penilaian aplikasi** 

|Pertanyaan|Jawaban|Jumlah|%|
|---|---|---|---|
|Q8. Pentingnya privasi dan keamanan data|Sangat penting|19|95,0|
||Cukup penting|1|5,0|
|Q10. Manfaat aplikasi sejenis|Sangat bermanfaat|18|90,0|
||Bermanfaat|2|10,0|



Pada kolom komentar, tiga responden memberikan masukan substantif. Masukan tersebut menekankan pentingnya informasi mengenai kekerasan di sekitar masyarakat, edukasi tentang layanan pengaduan bagi masyarakat berpenghasilan menengah ke bawah, serta penyediaan informasi dan akses bantuan yang mudah dipahami dengan privasi sebagai prioritas. 

### **5.6 Analisis silang** 

- Dari 16 responden yang menyebut rasa takut melapor, 15 di antaranya menjawab mengetahui ke mana harus mencari bantuan (Q1). Mengetahui tempat bantuan tidak otomatis menghilangkan rasa takut. 

- Sebanyak 10 dari 11 responden yang mengkhawatirkan privasi (Q3) juga menyebut rasa takut melapor. Kedua hambatan tersebut sering muncul bersamaan. 

- Sebanyak 6 responden menilai informasi sulit atau cukup sulit ditemukan (Q2). Lima responden juga memilih "informasi sulit ditemukan" sebagai hambatan pada Q3. 

## **6. Temuan Penelitian** 

|Kode|Temuan|Dasar|
|---|---|---|
|T1|Mayoritas responden mengetahui tempat mencari<br>bantuan dan menilai informasi cukup mudah<br>ditemukan.|Q1: 18/20 - Q2: 14/20|
|T2|Rasa takut melapor adalah hambatan yang paling<br>banyak dipilih, jauh di atas hambatan lain.|Q3: 16/20|
|T3|Kekhawatiran terhadap privasi dan identitas<br>dirasakan separuh responden, dan privasi dinilai<br>sangat penting oleh hampir seluruh responden.|Q3: 11/20 - Q8: 19/20|
|T4|Sebagian responden belum tahu siapa yang harus<br>dihubungi dan belum memahami prosedur.|Q3: masing-masing 9/20|
|T5|Biaya menjadi kekhawatiran bagi sebagian<br>responden, dan informasi hukum dinilai cukup sulit<br>dipahami oleh sebagian responden.|Q3: 8/20 - Q6: 9/20|
|T6|Tombol bantuan cepat adalah fitur yang paling<br>banyak dipilih. Fitur lain dipilih oleh 6–7 responden.|Q7: 18/20 vs 7–8/20|
|T7|Informasi lebih mudah dipahami bila singkat,<br>berbahasa sederhana, dan bertahap. Video kurang<br>diminati.|Q9: 15/20 memilih teks singkat atau<br>langkah demi langkah - 2/20 memilih<br>video|
|T8|Seluruh responden menilai aplikasi serupa<br>bermanfaat.|Q10: 20/20|



## **7. Identifikasi Permasalahan Pengguna** 

Permasalahan berikut diturunkan dari temuan. Kekuatan bukti dinilai dari jumlah responden yang mendukungnya. 

|Kode|Permasalahan|Dasar data|Kekuatan bukti|
|---|---|---|---|
|PM-01|Rasa takut melapor menghambat pengguna<br>mencari bantuan.|Q3: 16/20|Kuat|
|PM-02|Kekhawatiran identitas dan data tidak terjaga.|Q3: 11/20 - Q8: 19/20|Kuat|
|PM-03|Ketidakpastian mengenai pihak yang harus<br>dihubungi.|Q3: 9/20 - Q7:<br>pencarian layanan<br>8/20|Sedang|
|PM-04|Ketidakpastian mengenai prosedur dan|Q3: 9/20 - Q4: 7/20 -|Sedang|



|Kode|Permasalahan|Dasar data|Kekuatan bukti|
|---|---|---|---|
||langkah awal.|Q7: 8/20||
|PM-05|Kekhawatiran biaya.|Q3: 8/20|Sedang|
|PM-06|Bahasa informasi hukum dirasa sulit dipahami.|Q6: 9/20|Sedang|
|PM-07|Kesadaran terhadap layanan bantuan hukum<br>belum merata.|Q5: 9/20 kurang atau<br>tidak mengetahui|Sedang|
|PM-08|Informasi sulit ditemukan.|Q2: 6/20 - Q3: 5/20|Lemah|



Perumusan masalah dalam dokumen proyek menekankan kurangnya akses informasi. Data kuesioner mendukung hal itu sebagian: kendala dominan responden bukan pada letak informasi, melainkan pada rasa takut, privasi, ketidakpastian kontak, dan ketidakpastian prosedur (PM-01 sampai PM-04). Rumusan masalah pada tahap perancangan sebaiknya mencerminkan keseimbangan ini. 

## **8. Kebutuhan Pengguna** 

|Kode|Kebutuhan pengguna|Dasar|Respons produk|
|---|---|---|---|
|KP-01|Mendapat bantuan segera tanpa<br>mencari menu|Q7: 18/20 -<br>PDF fitur 1|Quick Help yang mengarah ke<br>kategori Bantuan Darurat|
|KP-02|Menjaga privasi dan dapat<br>menyembunyikan layar dengan cepat|Q8: 19/20 -<br>PM-02 - KK-3,<br>KK-11|Tanpa login (KK-2), Quick Exit, PIN<br>opsional|
|KP-03|Mengetahui langkah awal secara<br>terstruktur dan tidak terburu-buru|Q4: 7/20 - Q7:<br>8/20 - PM-04|Panduan Langkah Awal dan<br>Checklist Panduan|
|KP-04|Mengetahui pihak yang dapat<br>dihubungi dan memilih layanan yang<br>sesuai|PM-03 - Q4:<br>7/20 - Q7:<br>8/20|Cari Layanan, Daftar, Peta Layanan,<br>Detail Layanan (KK-1)|
|KP-05|Menyimpan informasi untuk dibuka<br>kembali|PDF fitur 5 -<br>KK-1|Tersimpan|
|KP-06|Memahami bantuan hukum dan hak<br>korban dalam bahasa sederhana|PM-06,<br>PM-07 - Q7: 7<br>–8/20|Informasi Bantuan Hukum, Kenali<br>Hakmu, FAQ|
|KP-07|Mengetahui apakah layanan berbayar|PM-05|Informasi biaya pada layanan, bila<br>datanya tersedia|
|KP-08|Memilih jenis bantuan sesuai<br>kebutuhan|KK-9|Empat kategori: Bantuan Hukum,<br>Pendampingan, Informasi<br>Pelaporan, Bantuan Darurat|



|Kode|Kebutuhan pengguna|Dasar|Respons produk|
|---|---|---|---|
|KP-09|Menerima informasi yang singkat dan|Q9: 15/20|Teks singkat, langkah bernomor,|
||bertahap||ikon pendukung|



## **9. Kesimpulan Penelitian** 

### **9.1 Kesimpulan** 

Sebagian besar responden mengetahui ke mana harus mencari bantuan (18/20) dan menilai informasi relatif mudah ditemukan (14/20), tetapi hambatan psikologis dan keamanan tetap menonjol. Rasa takut melapor dipilih oleh 16/20 responden. Privasi dinilai sangat penting oleh 19/20 responden. Ketidakpastian mengenai pihak yang harus dihubungi dan prosedur masing-masing dipilih oleh 9/20 responden. 

Implikasinya bagi Ruang Aman, aplikasi tidak cukup berfungsi sebagai direktori informasi. Aplikasi perlu menggunakan bahasa yang tenang dan tidak menghakimi, menjaga privasi sejak penggunaan pertama tanpa login, menyediakan Quick Exit untuk segera menyembunyikan tampilan sensitif, memberi akses cepat ke bantuan darurat, serta menuntun pengguna menuju layanan yang sesuai. Hal tersebut selaras dengan keputusan proyek mengenai empat kategori kebutuhan, penggunaan tanpa login, dan mekanisme Quick Exit. 

### **9.2 Keterbatasan penelitian** 

1. Jumlah responden adalah 20 orang, 12 di antaranya berusia 23–27 tahun. Hasil menggambarkan kelompok responden ini dan tidak dapat digeneralisasi sebagai representasi seluruh korban kekerasan atau seluruh masyarakat. 

2. Kuesioner tidak membedakan responden yang pernah mengalami kekerasan dari yang hanya mengetahuinya, dan tidak memuat data jenis kelamin maupun wilayah. 

3. Pertanyaan hambatan dan kebutuhan dirumuskan dalam bentuk persepsi, sehingga hasilnya perlu dilengkapi data wawancara. 

4. Hasil wawancara dan usability testing belum termasuk dalam dokumen ini. 

5. Data layanan belum tersedia sehingga kecocokan antara kebutuhan dan layanan nyata belum dapat dievaluasi. 

