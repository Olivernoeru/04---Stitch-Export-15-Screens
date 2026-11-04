# **06 — User Flow, Flowchart & Customer Journey Map** 

Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan 

Dokumen 06 dari 06 · Versi Final · 4 November 2026 

**Keterangan sumber. KK-n adalah jawaban klarifikasi proyek pada klarifikasi nomor n, Qn adalah pertanyaan kuesioner (20 responden), PDF adalah dokumen Topik Proyek UI UJIAN, spesifikasi desain adalah ketentuan desain yang ditetapkan dalam spesifikasi dokumen. Nomor layar mengacu pada 15 layar prototype: 1 Splash Screen, 2 Onboarding, 3 Masuk/Mulai, 4 Beranda, 5 Butuh Bantuan, 6 Pilih Jenis Kebutuhan, 7 Panduan Langkah Awal, 8 Checklist Panduan, 9 Cari Layanan, 10 Daftar Layanan, 11 Detail Layanan, 12 Informasi Bantuan Hukum, 13 Kenali Hakmu, 14 FAQ, 15 Profil & Pengaturan Privasi.** 

## **1. User Flow Utama** 

Alur utama yang ditetapkan dalam keputusan proyek adalah Beranda → Butuh Bantuan → Pilih Jenis Kebutuhan → Panduan Langkah Awal → Checklist Panduan → Cari Layanan → Daftar Layanan → Detail Layanan → Hubungi Layanan. Pengguna masuk ke Beranda langsung dari Masuk/Mulai tanpa login (KK-2), dan tombol Quick Exit tersedia di seluruh halaman utama sejak Onboarding (KK-3, KK-11). 



<!-- Start of picture text -->
Satu jalur utama dari Beranda sampai Hubungi Layanan<br>Beranda Butuh Bantuan Pilih Jenis Kebutuhan<br>halaman 4 halaman 5 halaman 6<br>Panduan Langkah Awal Checklist Panduan CariLayanan<br>halaman7 halaman 8 halaman9<br>Daftar Layanan Detail Layanan Hubungi Layanan<br>halaman 10 halaman 11 lembar pilihan kanal<br>Quick Exit tersedia di seluruh halaman utama, termasuk Onboarding dan Masuk/Mulai.<br><!-- End of picture text -->

user flow utama · 9 langkah dari Beranda ke Hubungi Layanan 

|Langkah|Layar|Tindakan pengguna|Respons aplikasi|
|---|---|---|---|
|1|4 Beranda|Membuka Beranda lalu memilih|Membuka Butuh Bantuan|
|||"Butuh Bantuan"||
|2|5 Butuh|Memilih "Ceritakan kebutuhanmu"|Membuka Pilih Jenis|



|Langkah|Layar|Tindakan pengguna|Respons aplikasi|
|---|---|---|---|
||Bantuan||Kebutuhan|
|3|6 Pilih Jenis<br>Kebutuhan|Memilih satu dari empat kategori lalu<br>"Lanjut"|Membuka Panduan sesuai<br>kategori|
|4|7 Panduan<br>Langkah Awal|Membaca langkah, lalu "Lanjut ke<br>Checklist"|Membuka Checklist|
|5|8 Checklist<br>Panduan|Mencentang langkah, lalu "Cari<br>Layanan"|Menyimpan progres di<br>perangkat dan membuka Cari<br>Layanan|
|6|9 Cari Layanan|Menulis kata kunci atau memilih<br>filter, lalu "Cari"|Membuka Daftar Layanan<br>dengan filter terisi|
|7|10 Daftar<br>Layanan|Memilih layanan dari mode Daftar<br>atau Peta|Membuka Detail Layanan|
|8|11 Detail<br>Layanan|Membaca informasi lalu menekan<br>"Hubungi Layanan"|Membuka lembar pilihan kanal|
|9|Lembar<br>Hubungi|Memilih kanal yang tersedia|Membuka aplikasi telepon<br>atau pesan perangkat|



**Alur pendukung.** Dari Beranda pengguna dapat membuka Informasi Bantuan Hukum (12), Kenali Hakmu (13), FAQ (14), dan pintasan Tersimpan (15). Aksi simpan tersedia pada layar 7, 11, 12, dan 13. Tab bawah menghubungkan Beranda (4), Bantuan (5), Layanan (9), dan Profil (15). Quick Help pada Beranda membuka lembar Bantuan Darurat tanpa melalui langkah 1 sampai 3. 

## **2. User Flow Empat Kategori Kebutuhan** 

Empat kategori ditetapkan dalam keputusan proyek sebagai kategori resmi aplikasi (KK-9). Semua kategori dimulai dari layar 6 dan mengikuti alur yang sama hingga Hubungi Layanan. Perbedaannya terletak pada isi panduan dan filter layanan. 

|Kategori|Pintu<br>masuk|Jalur|Isi panduan|Filter layanan|Tujuan akhir|
|---|---|---|---|---|---|
|K1 Bantuan<br>Hukum|Layar 6|6 → 7 → 8 → 9 →<br>10 → 11 →<br>Hubungi|Materi proyek<br>untuk bantuan<br>hukum, tautan<br>ke layar 12 dan<br>13|Bantuan<br>Hukum|Menghubungi<br>layanan<br>bantuan<br>hukum|
|K2<br>Pendampingan|Layar 6|6 → 7 → 8 → 9 →<br>10 → 11 →<br>Hubungi|Materi proyek<br>untuk<br>pendampingan|Pendampingan|Menghubungi<br>layanan<br>pendampingan|



|Kategori|Pintu<br>masuk|Jalur|Isi panduan|Filter layanan|Tujuan akhir|
|---|---|---|---|---|---|
|K3 Informasi<br>Pelaporan|Layar 6|6 → 7 → 8 → 9 →<br>10 → 11 →<br>Hubungi|Materi proyek<br>tentang<br>informasi dan<br>tempat<br>pelaporan|Informasi<br>Pelaporan|Menghubungi<br>layanan atau<br>tempat<br>pelaporan|
|K4 Bantuan<br>Darurat|Layar 6,<br>dan<br>Quick<br>Help di<br>Beranda|6 → 7 → 8 → 9 →<br>10 → 11 →<br>Hubungi. Quick<br>Help di Beranda<br>menjadi pintasan<br>menuju akses<br>Bantuan Darurat<br>(K4).|Panduan<br>Bantuan<br>Darurat sesuai<br>materi sumber<br>proyek.|Bantuan<br>Darurat|Menghubungi<br>bantuan<br>darurat<br>secepat<br>mungkin|



Keempat kategori menggunakan alur utama yang konsisten. Quick Help pada Beranda menjadi pintasan untuk mengakses Bantuan Darurat (K4). Seluruh isi panduan mengikuti materi sumber proyek, sedangkan data layanan hanya ditampilkan setelah tersedia (KK-6, KK-10). 

Pengguna yang membantu orang terdekat tetap dapat menggunakan aplikasi melalui empat kategori kebutuhan yang tersedia. Tidak ada kategori kelima atau jalur tambahan pada layar 6. 

## **3. Flowchart** 

### **3.1 Flowchart jalur kategori** 

Flowchart berikut memperlihatkan percabangan pada layar 6 dan penggabungannya hingga Hubungi Layanan. Quick Help tidak digambar karena langsung masuk ke jalur K4 dari Beranda. 



<!-- Start of picture text -->
Empat kategori, satu alur layanan<br>Pilih Jenis Kebutuhan<br>halaman 6<br>_—— —~—<br>—_ ee—<br>Bantuan Hukum Pendampingan Informasi Pelaporan Bantuan Darurat<br>KL K2 K3, Ka<br>Panduan Langkah Awal<br>halaman 7<br>Checklist Panduan<br>halaman 8<br>Cari Layanan<br>halaman 9<br>Daftar/ Peta Layanan<br>halaman 10<br>Detail Layanan<br>halaman 11<br>Hubungi Layanan<br>lembar phan kanal<br>Quick Help pada Beranda membuka akses Bantuan Darurat (KA). Alur kategortetap menggunakan empat pilhan resmi<br><!-- End of picture text -->

flowchart jalur empat kategori kebutuhan 

### **3.2 Flowchart Quick Exit** 

Flowchart ini mewujudkan keputusan proyek pada KK-11: perpindahan ke layar netral terjadi seketika tanpa konfirmasi, data tidak dihapus, dan kembali ke aplikasi bergantung pada PIN opsional. Jika PIN diaktifkan, pengguna memasukkan PIN sebelum konten aplikasi ditampilkan kembali. Jika PIN tidak diaktifkan, pengguna dapat kembali melalui mekanisme kembali pada tampilan netral. 



<!-- Start of picture text -->
Quick Exit: seketika, tanpa konfirmasi, tanpa menghapus data<br>Pengguna menekan Quick Exit<br>tersedia sejak Onboarding dan Masuk/Mulai<br>Halaman netral tampil seketika<br>tanpa dialog konfirmasi<br>Tidak= PIN aktif? ]¥<br>Masukkan PIN<br>PIN benar<br>Kembali ke aplikasi Checklist, Tersimpan, dan pengaturan<br>tanpa PIN tidak dihapus oleh Quick Exit.<br>Kembali ke layar terakhir<br>data tetap utuh<br><!-- End of picture text -->

flowchart Quick Exit dan kembali ke aplikasi 

### **3.3 Titik keputusan** 

|Keputusan|Kondisi|Hasil|
|---|---|---|
|Quick Help ditekan?|Pengguna menekan<br>tombol di Beranda|Lembar Bantuan Darurat (K4) terbuka|
|Kategori dipilih|Pengguna memilih<br>satu dari K1–K4 di<br>layar 6|Panduan sesuai kategori, filter layanan terisi|
|Data layanan tersedia?|Data proyek sudah<br>dimuat|Ya: daftar, peta, dan detail ditampilkan.<br>Tidak: keterangan data belum tersedia,<br>tanpa data buatan (KK-6)|
|Ada layanan yang sesuai?|Hasil pencarian tidak<br>kosong|Ya: Detail Layanan. Tidak: saran mengubah<br>kata kunci atau filter|
|Izin lokasi diberikan?|Hanya ditanyakan saat|Ya: peta menampilkan lokasi pengguna.<br>Tidak:peta tetaptampil tanpa lokasi|



|Keputusan|Kondisi|Hasil|
|---|---|---|
||mode Peta dibuka|pengguna|
|PIN aktif?|Pengaturan di layar 15|Ya: papan PIN. Tidak: kembali langsung|
|PIN benar?|Masukan pengguna|Ya: kembali ke layar terakhir. Tidak: tetap di<br>layar netral|



## **4. Customer Journey Map** 

### **4.1 Dasar penyusunan** 

Customer Journey Map ini menggambarkan perjalanan Persona 1 (Pencari Bantuan) dari membuka aplikasi hingga menghubungi layanan. Penyusunannya berdasarkan tiga sumber: kuesioner 20 responden (hambatan dan kebutuhan), alur produk dari PDF dan keputusan proyek, dan kerangka persona pada Dokumen 02. Peta ini disusun dari hasil kuesioner dan alur produk. Kolom "perasaan yang diperkirakan" merupakan interpretasi dari data kuesioner, bukan pengamatan langsung. Hasil wawancara dan usability testing bersama Lili, RA (Riska Amalia), dan Syifa dicatat terpisah untuk kebutuhan slide presentasi dan evaluasi prototype. Angka dalam dokumen berasal dari 20 responden dan tidak digeneralisasi. 

### **4.2 Ringkasan tahap perjalanan** 

|Tahap|Tujuan pengguna|Layar|Perasaan yang<br>diperkirakan|
|---|---|---|---|
|1. Membuka dan<br>memahami aplikasi|Merasa aman dan paham fungsi<br>aplikasi|1, 2, 3, 4|Waspada dan ragu|
|2. Menyatakan<br>kebutuhan|Menemukan jalur yang sesuai|4, 5, 6|Cemas, kadang terdesak|
|3. Memahami langkah|Mengetahui apa yang harus<br>dilakukan|7, 8, 12, 13,<br>14|Mulai lega bila langkah<br>kecil dan jelas|
|4. Mencari layanan|Menemukan layanan yang sesuai|9, 10, 11|Fokus, sebagian bingung<br>memilih|
|5. Menghubungi<br>layanan|Memulai kontak dengan layanan|11 dan<br>lembar<br>Hubungi|Takut sekaligus siap|
|6. Menyimpan dan<br>menjaga privasi|Dapat kembali ke informasi dan<br>merasa terlindungi|15, layar<br>netral|Perlu merasa terlindungi|



## **5. Pain Points** 

|Tahap|Pain point|Dasar|Kekuatan bukti|
|---|---|---|---|
|1|Khawatir identitas dan layar terlihat orang lain,<br>belum tahu cara keluar cepat|Q3: privasi 11/20,<br>Q8: 19/20|Kuat|
|2|Rasa takut melapor, bingung memilih jenis bantuan|Q3: takut 16/20|Kuat|
|3|Tidak paham prosedur, bahasa hukum sulit<br>dipahami|Q3: prosedur<br>9/20, Q6: 9/20|Sedang|
|4|Tidak tahu harus menghubungi siapa, khawatir<br>biaya|Q3: kontak 9/20,<br>biaya 8/20|Sedang|
|5|Keraguan sebelum menghubungi (tidak ada<br>pertanyaan kuesioner yang mengukurnya langsung,<br>diturunkan dari rasa takut melapor)|Q3: takut 16/20|Hipotesis|
|6|Orang lain dapat melihat layar atau cuplikan aplikasi|Q3: privasi 11/20,<br>KK-11|Sedang|



## **6. User Actions** 

|Tahap|Tindakan pengguna|Respons aplikasi|
|---|---|---|
|1|Membuka aplikasi, membaca Onboarding, menekan<br>"Mulai"|Menampilkan Beranda tanpa login|
|2|Menekan Quick Help atau "Butuh Bantuan",<br>memilih kategori|Membuka lembar Bantuan Darurat<br>atau Panduan sesuai kategori|
|3|Membaca panduan, mencentang checklist,<br>membuka Informasi Bantuan Hukum, Kenali Hakmu,<br>atau FAQ, menyimpan informasi|Menyimpan progres dan item<br>Tersimpan di perangkat|
|4|Menulis kata kunci, memilih filter, membandingkan<br>layanan di mode Daftar atau Peta, membuka detail|Menampilkan hasil dari data layanan<br>proyek|
|5|Menekan "Hubungi Layanan" dan memilih kanal|Membuka aplikasi telepon atau<br>pesan perangkat|
|6|Menekan Quick Exit bila perlu, membuka<br>Tersimpan, mengatur PIN opsional|Berpindah ke layar netral tanpa<br>konfirmasi, data tidak dihapus|



## **7. Touchpoints** 

|Tahap|Touchpoint di aplikasi|Touchpoint di luar aplikasi|
|---|---|---|
|1|Splash,Onboarding,Masuk/Mulai,Beranda|Tidak ada|



|Tahap|Touchpoint di aplikasi|Touchpoint di luar aplikasi|
|---|---|---|
|2|Quick Help, Butuh Bantuan, Pilih Jenis Kebutuhan|Tidak ada|
|3|Panduan, Checklist, Informasi Bantuan Hukum,<br>Kenali Hakmu, FAQ|Tidak ada|
|4|Cari Layanan, Daftar atau Peta Layanan, Detail<br>Layanan|Layanan nyata dari data layanan<br>yang tersedia|
|5|Lembar Hubungi|Aplikasi telepon atau pesan<br>perangkat, layanan|
|6|Tombol Quick Exit, layar netral, Profil & Pengaturan<br>Privasi, Tersimpan|Daftar aplikasi terbuka (app switcher)<br>pada perangkat|



## **8. Opportunities** 

|Tahap|Peluang|Wujud pada rancangan|
|---|---|---|
|1|Menurunkan kecemasan dan<br>menjamin privasi sejak awal|Onboarding tentang tanpa login dan Quick Exit,<br>Quick Exit sejak layar 2|
|2|Mempercepat akses bantuan dan<br>menyederhanakan keputusan|Quick Help, empat kategori pada satu layar, bahasa<br>tidak menghakimi|
|3|Membuat langkah kecil dan jelas|Panduan bernomor, checklist, aksi simpan|
|4|Memperjelas pilihan dan menjawab<br>kekhawatiran biaya|Filter kategori, mode Peta, informasi biaya pada<br>data layanan|
|5|Menurunkan keraguan sebelum<br>menghubungi|Lembar kanal yang jelas, informasi jam dan biaya<br>tampil sebelum kontak|
|6|Memberi rasa terlindungi dan<br>kendali|Quick Exit tanpa konfirmasi, PIN opsional, tampilan<br>aman pada app switcher, data tidak terhapus oleh<br>Quick Exit|



