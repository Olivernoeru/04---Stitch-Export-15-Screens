# 02 — User Persona 

_Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan_ 

Dokumen 02 dari 06 · Versi Final · 4 November 2026 

## **1. Dasar Penyusunan Persona** 

Dokumen ini menyusun dua arketipe kebutuhan pengguna berdasarkan 20 respons kuesioner yang tersedia dan konteks penggunaan pada Topik Proyek UI UJIAN. Kuesioner tidak mengumpulkan jenis kelamin, wilayah, pengalaman pribadi, pekerjaan, atau kebiasaan penggunaan aplikasi. Karena itu, atribut tersebut tidak diisi atau direka. Persona pada dokumen ini merupakan proto-persona berbasis kebutuhan agregat, bukan profil individu yang diwawancarai. 

Tiga partisipan wawancara yang telah ditentukan adalah Lili, RA (Riska Amalia), dan Syifa. Dua persona berbasis hasil wawancara akan disajikan secara terpisah dalam slide presentasi setelah catatan wawancara tersedia. Dokumen ini tetap menggunakan hasil kuesioner sebagai dasar arketipe kebutuhan. 

Seluruh angka menggunakan 20 respons aktual pada CSV. Hasil menggambarkan kelompok responden kuesioner dan tidak dapat digeneralisasi sebagai representasi seluruh korban kekerasan atau masyarakat. 

## **2. Persona A — Pengguna yang Membutuhkan Panduan Awal** 

|**Aspek**|**Gambaran berbasis data**|**Dasar**|
|---|---|---|
|**Tujuan utama**|Memahami langkah pertama yang<br>dapat dilakukan dan merasa<br>cukup aman untuk mencari<br>bantuan.|Q4: 7/20 memilih langkah awal,<br>Q3: 16/20 memilih takut melapor.|
|**Kebutuhan**|Panduan singkat, bertahap, tidak<br>menghakimi, serta akses cepat<br>untuk menyembunyikan tampilan<br>sensitif.|Q7: 18/20 memilih tombol bantuan<br>cepat, Q9: 15/20 memilih teks<br>singkat atau langkah bertahap,<br>Q8: 19/20 menilai privasi sangat<br>penting.|
|**Hambatan**|Rasa takut melapor, kekhawatiran<br>privasi, dan ketidakpastian<br>prosedur.|Q3: takut 16/20, privasi 11/20,<br>prosedur 9/20.|
|**Preferensi informasi**|Penjelasan singkat dengan<br>bahasa sederhana atau panduan<br>langkah demi langkah.|Q9: 9/20 dan 6/20.|
|**Implikasi desain**|Onboarding yang jelas, Quick Exit<br>yang mudah ditemukan, Panduan<br>Langkah Awal, danChecklist.|KK-2, KK-3, KK-11, layar 2, 3, 7,<br>dan 8.|



## **3. Persona B — Pengguna yang Membutuhkan Akses Layanan** 

|**Aspek**|**Gambaran berbasis data**|**Dasar**|
|---|---|---|
|**Tujuan utama**|Menemukan pihak atau layanan<br>yang tepat, memahami pilihan<br>bantuan, dan mengetahui<br>informasi penting sebelum<br>menghubungi layanan.|Q3: 9/20 tidak tahu harus<br>menghubungi siapa, Q4: 5/20<br>memilih tempat atau layanan<br>pelaporan.|
|**Kebutuhan**|Kategori layanan yang jelas,<br>pencarian dan filter, informasi<br>biaya serta jam layanan, dan detail|Q3: biaya 8/20, Q7: pencarian<br>layanan 8/20, keputusan empat<br>kategori KK-9.|



||kontak yang bersumber.||
|---|---|---|
|**Hambatan**|Ketidakpastian kontak, prosedur,<br>dan biaya. Sebagian responden<br>juga menilai informasi hukum sulit<br>dipahami.|Q3: kontak 9/20, prosedur 9/20,<br>biaya 8/20, Q6: 9/20 menilai<br>informasi cukup sulit dipahami.|
|**Preferensi informasi**|Informasi ringkas, terstruktur, dan<br>disajikan dengan bahasa<br>sederhana.|Q9: teks singkat 9/20, panduan<br>bertahap 6/20.|
|**Implikasi desain**|Cari Layanan, Daftar Layanan,<br>Peta Layanan, Detail Layanan,<br>Informasi Bantuan Hukum, dan<br>Kenali Hakmu.|KK-1, KK-6, KK-9, KK-10, layar 9–<br>13.|



## **4. Kebutuhan Bersama** 

|**Kebutuhan**|**Temuan kuesioner**|**Respons dalam Ruang Aman**|
|---|---|---|
|**Privasi dan kendali tampilan**|19/20 menilai privasi sangat<br>penting.|Tanpa login, Quick Exit, layar<br>netral, PIN opsional.|
|**Bantuan cepat**|18/20 memilih tombol bantuan<br>cepat.|Quick Help pada Beranda menuju<br>Bantuan Darurat.|
|**Panduan awal**|7/20 memilih informasi langkah<br>awal sebagai kebutuhan pertama.|Panduan Langkah Awal dan<br>Checklist.|
|**Akses layanan**|9/20 tidak tahu harus<br>menghubungi siapa.|Empat kategori, pencarian, daftar,<br>peta, detail layanan.|
|**Informasi hukum yang mudah**<br>**dipahami**|9/20 menilai informasi hukum<br>cukup sulit dipahami.|Informasi Bantuan Hukum dan<br>Kenali Hakmu menggunakan<br>materi sumber dengan bahasa<br>sederhana.|



## **5. Batasan Interpretasi** 

- Kuesioner tidak mengidentifikasi responden sebagai korban, pendamping, atau pengamat. Persona tidak boleh diberi pengalaman pribadi yang tidak tercatat. 

- Dua arketipe dibedakan berdasarkan kebutuhan dominan, bukan berdasarkan kelompok responden yang terpisah. Satu responden dapat memiliki kebutuhan yang tercermin pada kedua arketipe. 

- Nama, usia individual, pekerjaan, kutipan, kebiasaan digital, motivasi personal, dan latar belakang tidak dicantumkan karena tidak tersedia sebagai data yang dapat mendukung atribut tersebut. 

- Hasil wawancara Lili, RA (Riska Amalia), dan Syifa digunakan secara terpisah pada slide presentasi setelah tersedia. Hasil usability testing digunakan untuk evaluasi prototype, bukan untuk mengubah data kuesioner. 

## **6. Implikasi terhadap Desain** 

Ruang Aman harus membantu pengguna bergerak dari kebutuhan awal menuju informasi dan layanan tanpa memaksa login, tanpa bahasa yang menghakimi, dan tanpa menampilkan data layanan yang belum tersedia. Quick Exit harus tersedia sejak Onboarding dan Masuk/Mulai serta tetap tersedia pada seluruh halaman utama. Ketika ditekan, aplikasi langsung berpindah ke tampilan netral tanpa konfirmasi. PIN merupakan pilihan keamanan tambahan. 

