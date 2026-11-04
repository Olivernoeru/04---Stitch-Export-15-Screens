# **04 — UX PRD** 

Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan 

Dokumen 04 dari 06 · Versi Final · 4 November 2026 

**Klasifikasi. Setiap fitur dan keputusan diberi salah satu klasifikasi: Wajib (tercantum dalam brief atau PDF Topik Proyek), Keputusan Proyek (jawaban klarifikasi proyek pada klarifikasi nomor n, ditulis KKn), atau Spesifikasi antarmuka (ketentuan visual dan interaksi yang digunakan sebagai acuan implementasi). Angka berasal dari kuesioner 20 responden (Qn), analisis lengkap ada pada Dokumen 01.** 

## **1. Product Overview** 

**Ruang Aman** adalah aplikasi mobile yang membantu pengguna memperoleh informasi dan akses bantuan terkait kekerasan dalam satu tempat: dari mengetahui langkah awal, memilih jenis bantuan, mencari layanan, hingga menghubungi layanan tersebut. Aplikasi dapat langsung dipakai tanpa login (KK-2) dan dilengkapi Quick Exit untuk menyembunyikan tampilan sensitif secara cepat (KK-3, KK-11). 

|Aspek|Keterangan|
|---|---|
|Nama produk|Ruang Aman (KK-4)|
|Platform|Aplikasi mobile (Android dan iOS)|
|Pengguna|Orang yang mencari bantuan, dan orang yang ingin membantu orang<br>terdekat (PDF)|
|Nilai utama|Langkah dan layanan yang jelas, dalam suasana yang tenang dan<br>privat|
|Cakupan prototype|15 layar dengan alur utama Beranda sampai Hubungi Layanan|



## **2. Product Background** 

Topik proyek berkaitan dengan SDG 5 (mengurangi kekerasan terhadap perempuan dan anak perempuan) dan SDG 16 (akses keadilan dan bantuan hukum). Orang yang mengalami atau mengetahui kekerasan sering tidak mengetahui apa yang harus dilakukan lebih dahulu, ke mana mencari pertolongan, bagaimana memperoleh pendampingan atau bantuan hukum, layanan mana yang tepercaya, dan hak apa yang dimiliki korban (PDF). 

Kuesioner terhadap 20 responden memperlihatkan bahwa sebagian besar responden mengetahui tempat mencari bantuan (18/20) dan menilai informasi cukup mudah ditemukan (14/20), tetapi 16/20 menyebut rasa takut melapor sebagai hambatan dan 19/20 menilai privasi sangat penting. Latar ini menempatkan Ruang Aman bukan sekadar direktori, melainkan sarana yang menurunkan rasa takut dan menjaga privasi saat pengguna mencari bantuan. 

## **3. Problem Statement** 

Rumusan dari proyek: kurangnya akses informasi yang sederhana dan terpusat mengenai langkah awal, layanan pendampingan, dan bantuan hukum bagi korban kekerasan. 

Berdasarkan data kuesioner, rumusan tersebut diperjelas pada tahap perancangan: pengguna menghadapi hambatan berlapis berupa rasa takut melapor (16/20), kekhawatiran privasi (11/20), ketidakpastian mengenai pihak yang dihubungi (9/20), dan ketidakpastian mengenai prosedur (9/20). Hambatan informasi sulit ditemukan dipilih oleh 5/20 responden pada Q3. Pada Q2, 6/20 responden menilai informasi sulit atau cukup sulit ditemukan. Masalah yang dipecahkan produk dengan demikian adalah kesulitan pengguna untuk beralih dari kebingungan dan rasa takut menuju langkah dan layanan yang jelas, tanpa mengorbankan privasi. Temuan ini berasal dari 20 responden dan tidak digeneralisasi. 

## **4. Product Goals** 

|Tujuan|Indikator evaluasi|Dasar|
|---|---|---|
|Pengguna dapat memperoleh<br>akses bantuan segera|Tombol Quick Help ditemukan dan<br>dipahami pada usability testing|Q7: 18/20|
|Pengguna merasa aman dan<br>privasinya terlindungi|Quick Exit ditemukan, dipahami, dan<br>berfungsi sesuai keputusan proyek,<br>persepsi rasa aman pada pengujian|Q8: 19/20, KK-3, KK-11|
|Pengguna mengetahui langkah<br>awal yang harus dilakukan|Pengguna dapat menjelaskan<br>langkah berikutnya setelah membaca<br>Panduan|Q3: 9/20, Q4|
|Pengguna menemukan layanan<br>yang sesuai kategori dan<br>menghubunginya|Alur utama selesai tanpa bantuan|PDF: alur utama, KK-9|
|Pengguna memahami<br>informasi hukum dan haknya|Teks dipahami tanpa penjelasan<br>tambahan|Q6: 9/20|



Indikator dievaluasi pada usability testing bersama Lili, RA (Riska Amalia), dan Syifa (KK-7). Ambang keberhasilan angka belum ditetapkan dalam keputusan proyek. 

## **5. Target Users** 

Target pengguna mencakup orang yang mencari informasi atau bantuan terkait kekerasan, termasuk orang yang membantu orang terdekat, sebagaimana konteks pada PDF. Dua arketipe kebutuhan dalam Dokumen 02 disusun dari hasil kuesioner, bukan dari identitas individu. Kuesioner menunjukkan 12 dari 20 responden berusia 23–27 tahun dan 1 responden di bawah 18 tahun. Data demografis yang tersedia belum cukup untuk menetapkan segmen usia khusus. 

## **6. User Needs** 

|Kode|Kebutuhan|Dasar|
|---|---|---|
|KP-01|Bantuan segera tanpa mencari menu|Q7: 18/20|
|KP-02|Privasi dan kemampuan menyembunyikan layar dengan<br>cepat|Q8: 19/20, KK-11|
|KP-03|Langkah awal yang terstruktur|Q4: 7/20, Q7: 8/20|
|KP-04|Mengetahui pihak yang dihubungi dan memilih layanan<br>sesuai kategori|Q3: 9/20, KK-9|
|KP-05|Menyimpan informasi untuk dibuka kembali|PDF fitur 5, KK-1|
|KP-06|Memahami bantuan hukum dan hak dalam bahasa<br>sederhana|Q6: 9/20, Q7: 7–8/20|
|KP-07|Mengetahui apakah layanan berbayar|Q3: 8/20|
|KP-08|Memilih jenis bantuan sesuai kebutuhan|KK-9|
|KP-09|Informasi singkat dan bertahap|Q9: 15/20|



## **7. Product Scope** 

### **7.1 Dalam lingkup** 

- Prototype 15 layar: Splash Screen, Onboarding, Masuk/Mulai, Beranda, Butuh Bantuan, Pilih Jenis Kebutuhan, Panduan Langkah Awal, Checklist Panduan, Cari Layanan, Daftar Layanan, Detail Layanan, Informasi Bantuan Hukum, Kenali Hakmu, FAQ, Profil & Pengaturan Privasi. 

- Empat kategori kebutuhan resmi: Bantuan Hukum (K1), Pendampingan (K2), Informasi Pelaporan (K3), Bantuan Darurat (K4) (KK-9). 

- Penggunaan tanpa login (KK-2), Quick Exit sejak Onboarding (KK-3, KK-11), PIN opsional (KK-11), Peta Layanan dan Tersimpan (KK-1). 

### **7.2 Penempatan fitur pada 15 layar** 

|Fitur|Penempatan|Klasifikasi|
|---|---|---|
|Peta Layanan|Mode "Peta" pada Daftar Layanan (10),<br>berdampingan dengan mode "Daftar",<br>tombol "Lihat di Peta" pada Detail<br>Layanan (11)|Keputusan Proyek<br>(KK-1), penempatan:<br>Ketentuan desain|
|Tersimpan|Aksi simpan pada layar 7, 11, 12, 13,<br>koleksi di Profil & Pengaturan Privasi (15),<br>pintasan di Beranda (4)|Keputusan Proyek<br>(KK-1), penempatan:<br>Ketentuan desain|



|Fitur|Penempatan|Klasifikasi|
|---|---|---|
|Layar netral dan layar PIN|State khusus Quick Exit, di luar hitungan<br>15 layar|Ketentuan desain|
|Hubungi Layanan|Lembar pilihan kanal pada Detail Layanan<br>(11)|Wajib (alur utama),<br>bentuk: Ketentuan<br>desain|



### **7.3 Di luar lingkup** 

Hal berikut tidak memiliki dasar dalam sumber proyek atau keputusan proyek sehingga tidak dirancang: pembuatan akun atau login, pelaporan kasus langsung dari dalam aplikasi, percakapan dengan petugas, verifikasi identitas, dan sinkronisasi data lintas perangkat. 

## **8. Product Features** 

|Kode|Fitur|Tujuan|Fungsi|Layar|Klasifikasi|
|---|---|---|---|---|---|
|F-01|Quick Help|Memberi akses<br>bantuan tanpa<br>mencari menu|Satu ketukan dari Beranda<br>membuka jalur Bantuan<br>Darurat|4|Wajib (PDF<br>fitur 1),<br>didukung Q7|
|F-02|Quick Exit|Menyembunyikan<br>tampilan sensitif<br>seketika|Berpindah ke halaman<br>netral tanpa konfirmasi,<br>tidak menghapus data|2–15|Keputusan<br>Proyek (KK-3,<br>KK-11)|
|F-03|PIN opsional|Menambah<br>keamanan saat<br>kembali ke aplikasi|PIN dapat diaktifkan di<br>Pengaturan Privasi, bila<br>aktif, kembali dari<br>halaman netral<br>memerlukan PIN|15|Keputusan<br>Proyek<br>(KK-11)|
|F-04|Penggunaan<br>tanpa login|Menurunkan<br>hambatan masuk dan<br>melindungi identitas|Pengguna langsung masuk<br>ke Beranda|3|Keputusan<br>Proyek (KK-2)|
|F-05|Empat<br>kategori<br>kebutuhan|Mengarahkan<br>pengguna sesuai jenis<br>bantuan|Pilih K1–K4 pada satu<br>layar|6|Keputusan<br>Proyek (KK-9),<br>Wajib (layar 6)|
|F-06|Panduan<br>Langkah Awal|Menjawab "apa yang<br>dilakukan lebih<br>dahulu"|Langkah bernomor sesuai<br>kategori dari materi<br>sumber|7|Wajib (layar<br>7), konten<br>KK-10|
|F-07|Checklist<br>Panduan|Membuat langkah<br>terstruktur dan|Butir dapat dicentang, ada<br>penanda progres|8|Wajib (PDF<br>fitur 4)|



|Kode|Fitur|Tujuan|Fungsi|Layar|Klasifikasi|
|---|---|---|---|---|---|
|||terlacak||||
|F-08|Cari Layanan,<br>Daftar, Detail,<br>dan Hubungi|Menemukan dan<br>menghubungi<br>layanan yang sesuai|Pencarian dan filter,<br>daftar, detail, lembar<br>kanal|9, 10,<br>11|Wajib (alur<br>utama)|
|F-09|Peta Layanan|Membantu pengguna<br>melihat lokasi<br>layanan|Mode Peta pada Daftar<br>Layanan, lokasi hanya dari<br>data nyata|10|Keputusan<br>Proyek (KK-1)|
|F-10|Tersimpan|Membuka kembali<br>informasi penting<br>tanpa akun|Simpan panduan, layanan,<br>informasi, koleksi di Profil|4, 7,<br>11, 12,<br>13, 15|Keputusan<br>Proyek (KK-1)|
|F-11|Informasi<br>Bantuan<br>Hukum|Menjelaskan bantuan<br>hukum|Penjelasan dari materi<br>sumber|12|Wajib (layar<br>12)|
|F-12|Kenali Hakmu|Menyampaikan hak<br>korban|Kartu hak dari materi<br>sumber|13|Wajib (layar<br>13)|
|F-13|FAQ|Menjawab keraguan<br>awal|Akordeon pertanyaan<br>umum|14|Wajib (PDF<br>fitur 3)|
|F-14|Profil &<br>Pengaturan<br>Privasi|Memberi kendali<br>privasi tanpa akun|Tersimpan, pengaturan<br>Quick Exit, PIN,<br>pengelolaan data<br>perangkat|15|Wajib (layar<br>15), isi:<br>Keputusan<br>Proyek (KK-2)|



### **8.1 Spesifikasi Quick Exit** 

Sembilan butir keputusan proyek (KK-11) diterjemahkan menjadi kebutuhan perilaku berikut. 

|Butir keputusan|Konsekuensi bagi pengalaman pengguna|
|---|---|
|Menyembunyikan tampilan Ruang Aman dan<br>mengalihkan ke halaman netral|Fungsi utama adalah menyembunyikan, bukan<br>menutup aplikasi|
|Perpindahan langsung setelah tombol ditekan,<br>tanpa dialog konfirmasi|Satu ketukan, tidak ada langkah tambahan|
|Halaman netral tampak biasa, tanpa informasi<br>sensitif dan identitas Ruang Aman|Tidak ada logo, nama, atau warna merek pada<br>halaman netral|
|Tersedia di seluruh halaman utama, termasuk<br>Onboarding dan Masuk/Mulai|Tombol Quick Exit tersedia pada Onboarding,<br>Masuk/Mulai, dan seluruh halaman utama aplikasi.|
|Tidak menghapus data atau progres|Pengguna kembali ke layar terakhir dengan checklist|



|Butir keputusan|Konsekuensi bagi pengalaman pengguna|
|---|---|
||dan Tersimpan utuh|
|PIN opsional|Pengguna memutuskan sendiri, ditawarkan di<br>Pengaturan Privasi|
|Mekanisme kembali mempertimbangkan PIN|Jika PIN diaktifkan, pengguna memasukkan PIN<br>sebelum konten ditampilkan kembali. Jika PIN tidak<br>aktif, pengguna dapat kembali melalui mekanisme<br>pada tampilan netral.|
|Pertimbangkan tampilan di app switcher|Konten sensitif tidak terlihat pada daftar aplikasi<br>terbuka|



**Quick Exit langsung menampilkan halaman netral tanpa konfirmasi. Jika PIN diaktifkan, pengguna memasukkan PIN sebelum konten aplikasi ditampilkan kembali. Jika PIN tidak diaktifkan, pengguna dapat kembali ke aplikasi tanpa PIN.** 

## **9. User Journey (Konseptual)** 

Perjalanan pengguna Pencari Bantuan secara konseptual melewati enam tahap: lima tahap pertama pada tabel berikut, dan tahap keenam (menyimpan dan menjaga privasi, pada layar 15 dan layar netral) ketika pengguna memakai Tersimpan, Quick Exit, atau PIN. Penyusunan rinci, termasuk Customer Journey Map, ada pada Dokumen 06, seluruhnya disusun dari kuesioner, PDF, dan keputusan proyek, bukan dari hasil usability testing. 

|Tahap|Tujuan pengguna|Layar|Tantangan UX|
|---|---|---|---|
|1. Membuka<br>aplikasi|Merasa aman dan<br>memahami aplikasi|1–4|Kekhawatiran privasi, harus<br>tahu cara keluar cepat|
|2. Menyatakan<br>kebutuhan|Memilih jenis bantuan|4–6|Rasa takut, banyak pilihan|
|3. Memahami<br>langkah|Mengetahui apa yang<br>dilakukan|7, 8, 12, 13, 14|Bahasa hukum, ketidakpastian<br>prosedur|
|4. Mencari<br>layanan|Menemukan layanan<br>sesuai kategori|9, 10|Ketidakpastian pihak yang<br>dihubungi, biaya|
|5. Menghubungi<br>layanan|Mulai berkomunikasi<br>dengan layanan|11|Keraguan sebelum<br>menghubungi|



## **10. Product Constraints** 

|Batasan|Dampak|
|---|---|
|Data layanan baru tersedia setelah|Data layanan tidak tercantum dalam ZIPyang|



|Batasan|Dampak|
|---|---|
|pengumpulan kuesioner (KK-6)|diaudit. Nama lembaga, alamat, kontak, dan lokasi<br>tidak dibuat, layar layanan dan peta menampilkan<br>keterangan sampai data layanan tersedia.|
|Konten panduan terbatas pada materi sumber<br>proyek (KK-10)|Tidak ada prosedur hukum yang ditambahkan, teks<br>hanya disusun ulang agar singkat dan sederhana|
|Jumlah layar tetap 15|Peta Layanan, Tersimpan, layar netral, dan layar PIN<br>ditempatkan sebagai mode atau state|
|Penggunaan tanpa login (KK-2)|Data tersimpan berada di perangkat, tidak ada<br>sinkronisasi lintas perangkat|
|Hasil wawancara dan usability testing belum<br>tersedia|Persona dan Customer Journey Map belum memuat<br>data dari kedua kegiatan tersebut|
|Sampel kuesioner 20 responden|Temuan tidak digeneralisasi|
|Tenggat Jumat, 6 November 2026, termasuk<br>revisi proyek|Cakupan dikunci pada 15 layar|



## **11. UX Principles** 

|Prinsip|Penerapan|Dasar|
|---|---|---|
|Privasi lebih dahulu|Tanpa login, Quick Exit di seluruh halaman utama,<br>PIN opsional, tampilan aman pada app switcher|Q8: 19/20, KK-2,<br>KK-3, KK-11|
|Bantuan terdekat dari<br>jangkauan|Quick Help tampil di Beranda tanpa menggulir|Q7: 18/20|
|Satu layar, satu tujuan|Satu tindakan utama per layar untuk mengurangi<br>beban keputusan|Q3: 16/20|
|Tenang dan tidak<br>menghakimi|Bahasa sederhana, tanpa tekanan untuk melapor|Q3: 16/20, Q6|
|Bertahap|Panduan bernomor dan checklist|Q9: 15/20|
|Tidak bergantung pada<br>data fiktif|Konten hanya dari materi sumber dan data layanan<br>yang tersedia|KK-6, KK-10|
|Konsisten dan mudah<br>dikenali|Lokasi tombol dan pola komponen sama di seluruh<br>layar|Ketentuan desain|
|Dapat diuji|Setiap fitur utama memiliki indikator evaluasi pada<br>usability testing|Soal nomor 9|



