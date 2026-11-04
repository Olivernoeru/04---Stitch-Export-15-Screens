# **03 — User Stories & Requirements** 

Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan Dokumen 03 dari 06 · Versi Final · 4 November 2026 

**Keterangan sumber. Kolom "Dasar" memakai kode berikut: KK-n (jawaban klarifikasi proyek pada pertanyaan klarifikasi nomor n), Qn (pertanyaan kuesioner, 20 responden), PDF (Topik Proyek UI UJIAN), dan spesifikasi desain (ketentuan desain yang ditetapkan dalam spesifikasi dokumen).** 

## **1. Pendahuluan** 

### **1.1 Tujuan dokumen** 

Dokumen ini menetapkan kebutuhan produk Ruang Aman dalam bentuk user stories, functional requirements, dan non-functional requirements, serta menghubungkannya dengan 15 layar prototype. Dokumen ini menjadi acuan bagi UX PRD (Dokumen 04), UI PRD (Dokumen 05), serta user flow dan flowchart (Dokumen 06). 

### **1.2 Keputusan proyek yang menjadi dasar** 

|Kode|Keputusan proyek|
|---|---|
|KK-1|Peta Layanan dan Tersimpan tetap dimasukkan sebagai fitur.|
|KK-2|Aplikasi dapat dipakai langsung tanpa login atau registrasi.|
|KK-3|Quick Exit tersedia sejak Onboarding dan Masuk/Mulai.|
|KK-4|Nama aplikasi: Ruang Aman.|
|KK-6|Data layanan tersedia setelah pengumpulan kuesioner, tidak boleh ada informasi<br>layanan fiktif.|
|KK-9|Empat kategori kebutuhan: Bantuan Hukum, Pendampingan, Informasi Pelaporan,<br>Bantuan Darurat.|
|KK-10|Konten panduan tersedia dan dipakai apa adanya dari sumber proyek, tidak ada<br>prosedur hukum yang ditambahkan.|
|KK-11|Quick Exit mengalihkan langsung ke halaman netral, tanpa konfirmasi, tanpa<br>menghapus data, PIN bersifat opsional.|



### **1.3 Ruang lingkup dan penempatan fitur** 

Jumlah layar tetap 15. Fitur yang diputuskan proyek ditempatkan pada layar yang sudah ada: 

- **Peta Layanan** menjadi mode tampilan "Peta" pada Daftar Layanan (layar 10), berdampingan dengan mode "Daftar". Tombol "Lihat di Peta" pada Detail Layanan (layar 11) membuka mode tersebut. 

- **Tersimpan** berupa aksi simpan pada Panduan (7), Detail Layanan (11), Informasi Bantuan Hukum (12), dan Kenali Hakmu (13). Koleksinya berada di Profil & Pengaturan Privasi (15) dengan pintasan pada Beranda (4). 

- **Layar netral** dan **layar PIN** pada mekanisme Quick Exit diperlakukan sebagai state khusus, bukan layar tambahan di luar 15 layar. 

- Tombol **Hubungi Layanan** berupa lembar pilihan di Detail Layanan (layar 11). 

### **1.4 Kategori kebutuhan** 

|Kode|Kategori|Sasaran|
|---|---|---|
|K1|Bantuan Hukum|Informasi dan layanan bantuan hukum|
|K2|Pendampingan|Layanan pendampingan korban|
|K3|Informasi Pelaporan|Informasi dan tempat pelaporan|
|K4|Bantuan Darurat|Akses bantuan segera, ditautkan dengan tombol Quick Help|



## **2. User Stories** 

Pengguna dalam dokumen ini adalah pengguna Ruang Aman, yaitu seseorang yang mencari bantuan atau membantu orang lain. Kriteria penerimaan menjadi dasar pemeriksaan prototype. 

|ID|Sebagai|Saya ingin|Agar|Kriteria penerimaan|Dasar|
|---|---|---|---|---|---|
|US-01|Pengguna|menekan<br>tombol bantuan<br>cepat di<br>Beranda|segera<br>memperoleh<br>akses bantuan<br>tanpa mencari<br>menu|Tombol terlihat tanpa<br>menggulir, satu ketukan<br>membuka jalur Bantuan<br>Darurat (K4)|Q7: 18/20,<br>PDF fitur 1,<br>KK-9|
|US-02|Pengguna|langsung<br>memakai<br>aplikasi tanpa<br>login|tidak perlu<br>menyerahkan<br>identitas|Tidak ada formulir akun,<br>kata sandi, atau verifikasi<br>sebelum Beranda|KK-2, Q8:<br>19/20|
|US-03|Pengguna|menekan Quick<br>Exit dari<br>halaman mana<br>pun, termasuk<br>Onboarding dan<br>Masuk/Mulai|dapat<br>menyembunyi<br>kan layar<br>kapan pun<br>diperlukan|Tombol tampil di layar 2–<br>15 pada posisi yang<br>konsisten|KK-3, KK-11|
|US-04|Pengguna|berpindah|informasi|Perpindahan terjadi pada|KK-11|



|ID|Sebagai|Saya ingin|Agar|Kriteria penerimaan|Dasar|
|---|---|---|---|---|---|
|||seketika ke<br>halaman netral<br>saat Quick Exit<br>ditekan|sensitif<br>langsung tidak<br>terlihat|satu ketukan, tanpa<br>dialog konfirmasi.<br>Halaman netral tidak<br>menampilkan identitas<br>Ruang Aman maupun<br>informasi sensitif||
|US-05|Pengguna|tetap memiliki<br>progres setelah<br>memakai Quick<br>Exit|tidak perlu<br>mengulang<br>dari awal|Checklist dan Tersimpan<br>tidak terhapus oleh Quick<br>Exit|KK-11|
|US-06|Pengguna|mengaktifkan<br>PIN secara<br>opsional|dapat<br>menambah<br>keamanan<br>saat kembali<br>ke aplikasi|PIN dapat diaktifkan dan<br>dinonaktifkan di layar 15,<br>bila aktif, kembali dari<br>halaman netral meminta<br>PIN|KK-11|
|US-07|Pengguna|tampilan<br>aplikasi tidak<br>memperlihatka<br>n informasi<br>sensitif pada<br>daftar aplikasi<br>terbuka|informasi<br>tetap<br>tersembunyi<br>setelah Quick<br>Exit atau saat<br>berpindah<br>aplikasi|Cuplikan aplikasi pada<br>app switcher tidak<br>memuat konten sensitif|KK-11 (butir<br>9)|
|US-08|Pengguna<br>baru|memahami<br>tujuan aplikasi,<br>jaminan privasi,<br>dan fungsi<br>Quick Exit saat<br>Onboarding|merasa aman<br>sebelum<br>memakai|Onboarding menjelaskan<br>ketiga hal tersebut dan<br>dapat dilewati|Q8, Q3:<br>11/20,<br>spesifikasi<br>desain|
|US-09|Pengguna|memilih salah<br>satu dari empat<br>kategori<br>kebutuhan|diarahkan ke<br>jalur yang<br>sesuai|Layar 6 menampilkan K1–<br>K4, satu pilihan mengarah<br>ke Panduan sesuai<br>kategori|KK-9|
|US-10|Pengguna|membaca<br>panduan<br>langkah awal<br>sesuai kategori|mengetahui<br>apa yang<br>harus<br>dilakukan|Panduan memakai materi<br>dari sumber proyek,<br>berbentuk langkah<br>bernomor berbahasa<br>sederhana|KK-10, Q3:<br>9/20, Q9|
|US-11|Pengguna|menandai<br>langkahyang|melihat<br>progres dan|Butir checklist dapat<br>dicentang, progres tampil|PDF fitur 4|



|ID|Sebagai|Saya ingin|Agar|Kriteria penerimaan|Dasar|
|---|---|---|---|---|---|
|||sudah dilakukan|tidak bingung|dan tersimpan di<br>perangkat||
|US-12|Pengguna|mencari layanan<br>dan menyaring<br>berdasarkan<br>kategori|menemukan<br>layanan yang<br>sesuai|Kolom pencarian dan<br>filter K1–K4, filter terisi<br>bila berasal dari layar 6|Q3: 9/20,<br>Q7: 8/20,<br>KK-9|
|US-13|Pengguna|melihat daftar<br>layanan yang<br>ringkas|membandingk<br>an pilihan|Daftar memuat informasi<br>dari data layanan yang<br>tersedia|KK-6, PDF<br>use case|
|US-14|Pengguna|melihat layanan<br>pada peta|mengetahui<br>lokasi layanan|Mode Peta tersedia di<br>layar 10, titik layanan<br>hanya berasal dari data<br>layanan nyata|KK-1, PDF<br>fitur 2|
|US-15|Pengguna|membuka detail<br>layanan dan<br>menghubunginy<br>a|dapat<br>langsung<br>meminta<br>bantuan|Detail menampilkan<br>informasi layanan, tombol<br>Hubungi membuka<br>lembar pilihan kanal<br>sesuai data layanan|PDF use<br>case<br>langkah 6–7|
|US-16|Pengguna|menyimpan<br>panduan,<br>layanan, atau<br>informasi|dapat<br>membukanya<br>kembali tanpa<br>mencari ulang|Aksi simpan tersedia di<br>layar 7, 11, 12, 13, koleksi<br>di layar 15|KK-1, PDF<br>fitur 5|
|US-17|Pengguna|membaca<br>penjelasan<br>bantuan hukum|memahami<br>hak dan<br>prosedurnya|Layar 12 memuat<br>penjelasan dalam bahasa<br>sederhana dari materi<br>sumber|Q6: 9/20,<br>Q7: 8/20|
|US-18|Pengguna|mengenali hak<br>korban|mengetahui<br>apa yang<br>dapat diminta|Layar 13 memuat hak<br>dalam bahasa sederhana<br>dari materi sumber|Q7: 7/20,<br>brief|
|US-19|Pengguna|membaca<br>pertanyaan<br>yang sering<br>diajukan|memperoleh<br>jawaban atas<br>keraguan awal|Layar 14 menampilkan<br>pertanyaan dalam bentuk<br>akordeon|PDF fitur 3|
|US-20|Pengguna|mengatur<br>privasi tanpa<br>perlu akun|merasa<br>mengendalika<br>n data di<br>perangkat|Layar 15 memuat<br>pengaturan Quick Exit,<br>PIN opsional, dan data<br>tersimpan|KK-2, KK-11|



|ID|Sebagai|Saya ingin|Agar|Kriteria penerimaan|Dasar|
|---|---|---|---|---|---|
|US-21|Pengguna|melihat<br>informasi biaya<br>layanan|mengetahui<br>apakah<br>layanan sesuai<br>kemampuan|Biaya tampil pada layanan<br>apabila data tersedia|Q3: 8/20|



## **3. Functional Requirements** 

|ID|Kebutuhan fungsional|Layar|US|
|---|---|---|---|
|FR-01|Splash Screen menampilkan identitas Ruang Aman<br>secara singkat lalu otomatis menuju Onboarding.|1|US-08|
|FR-02|Onboarding menjelaskan tujuan aplikasi, jaminan<br>privasi, dan fungsi Quick Exit, dapat dilewati.|2|US-08|
|FR-03|Masuk/Mulai menyediakan tombol "Mulai" yang<br>langsung menuju Beranda tanpa login, registrasi,<br>atau verifikasi.|3|US-02|
|FR-04|Beranda menampilkan Quick Help, jalan masuk ke<br>Butuh Bantuan, pintasan Tersimpan, dan kartu<br>Pelajari menuju layar 12, 13, 14.|4|US-01, US-16|
|FR-05|Quick Help membuka jalur Bantuan Darurat (K4),<br>kontak ditampilkan dari data layanan yang tersedia.|4|US-01|
|FR-06|Tombol Quick Exit tampil pada layar 2–15 dengan<br>posisi konsisten, tidak ada tombol pada Splash<br>karena layar tersebut berpindah otomatis.|2–15|US-03|
|FR-07|Saat Quick Exit ditekan, aplikasi berpindah langsung<br>ke layar netral tanpa dialog konfirmasi. Layar netral<br>tampak seperti halaman biasa dan tidak memuat<br>logo, nama, warna merek, atau konten Ruang Aman.|State|US-04|
|FR-08|Kembali dari layar netral: bila PIN tidak aktif,<br>pengguna dapat kembali dari tampilan netral tanpa<br>PIN, bila PIN aktif, pengguna harus memasukkan<br>PIN.|State|US-04, US-06|
|FR-09|Quick Exit tidak menghapus checklist, data<br>Tersimpan, maupun pengaturan, pengguna kembali<br>ke layar terakhir.|State|US-05|
|FR-10|Pengguna dapat mengaktifkan, mengubah, dan<br>menonaktifkan PIN di layar 15.|15|US-06|



|ID|Kebutuhan fungsional|Layar|US|
|---|---|---|---|
|FR-11|Saat aplikasi berada di latar belakang atau setelah<br>Quick Exit, tampilan pada app switcher tidak<br>memperlihatkan konten sensitif.|Seluruh|US-07|
|FR-12|Navigasi bawah memuat empat tab: Beranda,<br>Bantuan, Layanan, Profil, tampil pada layar 4–15<br>kecuali saat lembar terbuka.|4–15|US-09, US-12|
|FR-13|Butuh Bantuan menjadi pintu masuk jalur bantuan<br>dan mengarahkan ke Pilih Jenis Kebutuhan.|5|US-09|
|FR-14|Pilih Jenis Kebutuhan menampilkan empat kategori<br>K1–K4, pilihan membawa pengguna ke Panduan<br>sesuai kategori.|6|US-09|
|FR-15|Panduan menampilkan langkah bernomor dari<br>materi sumber untuk kategori terpilih, dengan aksi<br>simpan dan lanjut ke Checklist.|7|US-10, US-16|
|FR-16|Checklist menampilkan butir yang dapat dicentang,<br>penanda progres, dan tombol lanjut ke Cari<br>Layanan.|8|US-11|
|FR-17|Cari Layanan menyediakan kolom pencarian dan<br>filter K1–K4 yang terisi otomatis dari kategori yang<br>dipilih.|9|US-12|
|FR-18|Daftar Layanan menampilkan hasil dalam mode<br>Daftar dengan informasi dari data layanan yang<br>tersedia.|10|US-13, US-21|
|FR-19|Daftar Layanan menyediakan mode Peta yang<br>menampilkan lokasi layanan dari data layanan,<br>akses lokasi perangkat bersifat opsional dan hanya<br>diminta saat pengguna membuka mode Peta.|10|US-14|
|FR-20|Detail Layanan menampilkan informasi layanan dari<br>data yang tersedia, aksi simpan, dan aksi "Lihat di<br>Peta".|11|US-15, US-16,<br>US-21|
|FR-21|Tombol Hubungi Layanan membuka lembar pilihan<br>kanal (misalnya telepon atau pesan) sesuai kanal<br>yang ada pada data layanan.|11|US-15|
|FR-22|Aksi simpan menambahkan item ke Tersimpan pada<br>perangkat dan dapat dibatalkan.|7, 11, 12, 13|US-16|
|FR-23|Tersimpan menampilkan itemyangdisimpan,|15(pintasan di 4)|US-16|



|ID|Kebutuhan fungsional|Layar|US|
|---|---|---|---|
||dikelompokkan menurut jenis, dan dapat dihapus<br>per item.|||
|FR-24|Informasi Bantuan Hukum menampilkan penjelasan<br>bantuan hukum dari materi sumber.|12|US-17|
|FR-25|Kenali Hakmu menampilkan hak korban dari materi<br>sumber dalam kartu yang dapat dibuka.|13|US-18|
|FR-26|FAQ menampilkan pertanyaan umum dalam bentuk<br>akordeon.|14|US-19|
|FR-27|Profil & Pengaturan Privasi tidak memuat data akun,<br>layar memuat Tersimpan, pengaturan Quick Exit,<br>PIN opsional, dan pengelolaan data di perangkat.|15|US-20|
|FR-28|Apabila data layanan belum tersedia, layar terkait<br>menampilkan keterangan bahwa data belum<br>tersedia, aplikasi tidak menampilkan nama lembaga,<br>kontak, atau lokasi buatan.|4, 9, 10, 11|US-13, US-14,<br>US-15|



## **4. Non-Functional Requirements** 

|ID|Kategori|Kebutuhan|Dasar|
|---|---|---|---|
|NFR-01|Privasi|Aplikasi dapat dipakai tanpa akun, data checklist<br>dan Tersimpan berada di perangkat pengguna.<br>Kebijakan penyimpanan data pada produk nyata<br>ditetapkan pada tahap pengembangan.|KK-2, Q8:<br>19/20|
|NFR-02|Kecepatan Quick<br>Exit|Quick Exit selesai dalam satu interaksi tanpa dialog<br>atau jeda yang terlihat oleh pengguna.|KK-11|
|NFR-03|Keamanan<br>tampilan|Konten sensitif tidak tampak pada app switcher<br>setelah Quick Exit atau saat aplikasi di latar<br>belakang.|KK-11|
|NFR-04|Keandalan state|Progres dan data tersimpan tetap utuh setelah<br>Quick Exit.|KK-11|
|NFR-05|Aksesibilitas|Kontras teks minimal 4,5:1, teks isi minimal 16 px,<br>target sentuh minimal 48 × 48 px, informasi tidak<br>disampaikan hanya melalui warna.|spesifikasi<br>desain<br>(pedoman<br>aksesibilitas<br>umum)|
|NFR-06|Bahasa|Bahasa Indonesia sederhana,kalimatpendek,nada|Q6: 9/20, Q9|



|ID|Kategori|Kebutuhan|Dasar|
|---|---|---|---|
|||tenang dan tidak menghakimi, istilah hukum diberi<br>penjelasan.||
|NFR-07|Kebenaran<br>konten|Panduan dan informasi hukum hanya berasal dari<br>materi sumber proyek, data layanan hanya berasal<br>dari proyek.|KK-6, KK-10|
|NFR-08|Kegunaan|Alur utama dapat diselesaikan pengguna tanpa<br>bantuan, diuji pada usability testing.|Soal nomor 9|
|NFR-09|Konsistensi|Warna, tipografi, ikon, jarak, dan komponen<br>mengikuti UI PRD (Dokumen 05).|spesifikasi<br>desain|
|NFR-10|Nada konten|Tidak memakai gambar atau ilustrasi kekerasan<br>eksplisit.|Q3: 16/20,<br>spesifikasi<br>desain|
|NFR-11|Kompatibilitas|Tata letak adaptif untuk ponsel Android dan iOS.|spesifikasi<br>desain|
|NFR-12|Izin lokasi|Akses lokasi bersifat opsional dan tidak diminta<br>sebelum mode Peta dibuka. Penyimpanan riwayat<br>lokasi tidak termasuk fungsi prototype.|KK-1,<br>spesifikasi<br>desain|



## **5. Prioritas Kebutuhan** 

Prioritas memakai MoSCoW. Must berlaku bagi kebutuhan yang diputuskan proyek atau didukung kuat data kuesioner dan membentuk alur utama. Should berlaku bagi kebutuhan yang penting tetapi tidak menghentikan alur utama, Could berlaku untuk kebutuhan yang bersifat opsional dalam keputusan proyek. 

|Prioritas|User Story|Alasan|
|---|---|---|
|Must|US-01, US-02, US-03, US-04,<br>US-05, US-09, US-10, US-12,<br>US-13, US-15|Keputusan proyek (KK-2, KK-3, KK-9, KK-11) atau<br>pembentuk alur utama, US-01 didukung 18 dari 20<br>responden|
|Must|US-14, US-16|Keputusan proyek (KK-1), bergantung pada data<br>layanan|
|Should|US-07, US-08, US-11, US-17,<br>US-18, US-19, US-20, US-21|Mendukung privasi, pemahaman, dan kepercayaan,<br>memiliki dasar kuesioner atau PDF|
|Could|US-06|PIN dinyatakan proyek sebagai fitur opsional|



## **6. Traceability antara User Stories, Requirements, dan Layar** 

|Layar|User Story|Functional Requirement|NFR terkait|
|---|---|---|---|
|1 Splash Screen|US-08|FR-01|NFR-09|
|2 Onboarding|US-03, US-08|FR-02, FR-06|NFR-01, NFR-06|
|3 Masuk/Mulai|US-02, US-03|FR-03, FR-06|NFR-01|
|4 Beranda|US-01, US-03, US-16|FR-04, FR-05, FR-06, FR-12,<br>FR-28|NFR-02, NFR-05|
|5 Butuh Bantuan|US-03, US-09|FR-06, FR-12, FR-13|NFR-08|
|6 Pilih Jenis Kebutuhan|US-09|FR-06, FR-14|NFR-08|
|7 Panduan Langkah Awal|US-10, US-16|FR-06, FR-15, FR-22|NFR-06, NFR-07|
|8 Checklist Panduan|US-11|FR-06, FR-16|NFR-04|
|9 Cari Layanan|US-12|FR-06, FR-12, FR-17, FR-28|NFR-07|
|10 Daftar Layanan|US-13, US-14, US-21|FR-06, FR-18, FR-19, FR-28|NFR-12|
|11 Detail Layanan|US-15, US-16, US-21|FR-06, FR-20, FR-21, FR-22,<br>FR-28|NFR-07|
|12 Informasi Bantuan<br>Hukum|US-17, US-16|FR-06, FR-22, FR-24|NFR-06, NFR-07|
|13 Kenali Hakmu|US-18, US-16|FR-06, FR-22, FR-25|NFR-06, NFR-07|
|14 FAQ|US-19|FR-06, FR-26|NFR-06|
|15 Profil & Pengaturan<br>Privasi|US-06, US-16, US-20|FR-06, FR-10, FR-12, FR-23,<br>FR-27|NFR-01, NFR-03|
|State: Layar netral dan|US-04, US-05,|FR-07, FR-08, FR-09, FR-11|NFR-02, NFR-03,|
|PIN|US-06, US-07||NFR-04|



Pemeriksaan kelengkapan: setiap layar memiliki minimal satu user story dan satu functional requirement. Setiap user story diturunkan ke minimal satu functional requirement, keempat kategori K1 –K4 terwakili pada US-09, FR-14, dan filter pada FR-17. 

