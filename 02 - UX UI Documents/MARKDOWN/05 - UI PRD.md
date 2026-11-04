# **05 — UI PRD** 

Ruang Aman: Aplikasi Mobile untuk Akses Informasi dan Bantuan Hukum bagi Korban Kekerasan Dokumen 05 dari 06 · Versi Final · 4 November 2026 

**Klasifikasi. Keputusan Proyek (KK-n) adalah jawaban klarifikasi proyek pada klarifikasi nomor n. Spesifikasi desain merupakan acuan visual dan interaksi untuk implementasi antarmuka. Qn adalah pertanyaan kuesioner (20 responden). Nilai warna, ukuran, dan jarak yang tercantum merupakan token desain yang digunakan secara konsisten dalam prototype.** 

## **1. Design Overview** 

UI Ruang Aman dirancang untuk pengguna yang mungkin cemas, tergesa, atau berada di tempat yang tidak sepenuhnya privat. Karena itu antarmuka dibuat tenang, lapang, dan jelas: tema terang dengan latar putih gading, satu warna aksen utama, bentuk membulat, dan satu tindakan utama pada setiap layar. Warna dan bentuk tidak boleh menimbulkan kesan tegang, sedangkan fungsi penting seperti bantuan cepat dan Quick Exit harus langsung dikenali. 

Karakter visual yang dituju: **tenang, hangat, jelas, dan tidak seperti template aplikasi pada umumnya** . Hal yang sengaja dihindari adalah gradien ungu atau neon, efek kaca yang generik, ilustrasi kekerasan eksplisit, dan penggunaan warna merah alarm secara masif. 

Dokumen ini memuat fondasi visual, spesifikasi komponen, dan spesifikasi terperinci 15 layar beserta state khusus Quick Exit. 

## **2. Design Principles** 

|Prinsip|Makna dalam UI|Dasar|
|---|---|---|
|Privasi lebih dahulu|Quick Exit selalu terlihat, tidak ada<br>informasi pribadi pada layar, layar<br>netral tanpa identitas|Q8: 19/20, KK-3, KK-11|
|Satu layar, satu tujuan|Satu tindakan utama per layar,<br>maksimal empat pilihan pada satu<br>keputusan|Q3: 16/20|
|Bantuan dalam jangkauan|Quick Help pada paruh atas Beranda|Q7: 18/20|
|Tenang, bukan menakutkan|Palet lembut, sudut membulat,<br>bahasa tidak menghakimi|Q3: 16/20|
|Bertahap dan mudah dibaca|Langkah bernomor, teks singkat,<br>bahasa sederhana|Q9: 15/20, Q6|
|Makna warna konsisten|Setiap warna mewakili satu fungsi|spesifikasi desain|



|Prinsip|Makna dalam UI|Dasar|
|---|---|---|
|Konten jujur|Tidak menampilkan data layanan<br>i|KK-6, KK-10|
||atau prosedur yang tidak bersumber||



## **3. Design Foundation** 

|Aspek|Ketentuan|
|---|---|
|Platform|Mobile, Android dan iOS (adaptasi pada bab 16)|
|Frame acuan|390 × 844 px (iOS) dan 360 × 800 px (Android), tata letak adaptif pada<br>rentang lebar sekitar 360–430 px|
|Tema|Terang saja, mode gelap tidak termasuk lingkup|
|Satuan|px pada desain, dp pada Android dan pt pada iOS ketika<br>diimplementasikan|
|Sistem desain|Seluruh warna, tipografi, jarak, dan radius didefinisikan sebagai token agar<br>konsisten|
|Pustaka ikon|Phosphor, gaya Regular|
|Nama aplikasi|Ruang Aman (KK-4)|



## **4. Color Palette** 

Rasio kontras dihitung dengan rumus WCAG, target teks minimal 4,5:1. 

|Token|Hex|Makna bagi pengguna|Penggunaan|Kontras|
|---|---|---|---|---|
|Latar|#FAF8F5|Lembut, tenang|Latar seluruh layar (sekitar<br>60% area bersama<br>permukaan)|n/a|
|Permukaan|#FFFFFF|Bersih, terpisah dari<br>latar|Kartu, lembar, input|n/a|
|Teks utama|#1F2A2E|Jelas dan tegas|Judul dan isi|13,86:1 pada<br>latar|
|Teks<br>sekunder|#5B6B70|Pendukung|Keterangan, label|5,24:1 pada<br>latar|
|Primer (teal)|#2A6B6F|Aman, tepercaya,<br>"lanjutkan"|Tombol utama, tab aktif,<br>tautan|6,12:1 dengan<br>teks putih|
|Primer<br>lembut|#E3EFEC|Wilayah informasi<br>yang tenang|Latar kartu info, chip<br>terpilih|5,19:1 dengan<br>teks primer|



|Token|Hex|Makna bagi pengguna|Penggunaan|Kontras|
|---|---|---|---|---|
|Bantuan<br>(terakota)|#B3452E|Mendesak tetapi<br>hangat, "butuh<br>sekarang"|Quick Help dan tombol<br>Hubungi Layanan|5,52:1 dengan<br>teks putih|
|Bantuan<br>lembut|#FBE9E4|Pendukung area<br>bantuan|Latar lembar Bantuan<br>Darurat|4,70:1 dengan<br>teks bantuan|
|Selesai<br>(hijau)|#2F7A57|Berhasil, selesai|Centang checklist, status<br>tersimpan|5,20:1 pada<br>putih|
|Perhatian<br>(amber)|#8A5A00<br>pada<br>#FFF3D6|Perlu dibaca|Biaya, catatan penting|5,37:1|
|Keluar (netral<br>gelap)|#1F2A2E<br>(garis dan<br>teks)|Menyembunyikan,<br>keluar|Tombol Quick Exit|13,86:1 pada<br>latar|
|Garis|#E4DFD8|Pemisah halus|Border kartu|n/a|



**Aturan makna warna. Teal berarti melanjutkan, terakota berarti bantuan segera, hijau berarti selesai, amber berarti perhatikan, netral gelap berarti keluar atau sembunyikan. Quick Exit sengaja tidak berwarna aksen agar tidak bersaing dengan tombol utama, tetapi selalu berada pada posisi yang sama. Informasi tidak pernah disampaikan hanya lewat warna.** 

**Layar netral** memakai palet abu-abu terang tersendiri (di luar token merek) agar tidak menyerupai Ruang Aman (lihat layar netral pada bab 13.16). 

## **5. Typography** 

Satu keluarga huruf: **Plus Jakarta Sans** (gratis, ramah, modern, mendukung teks Indonesia), cadangan sans-serif sistem. Teks isi tidak kurang dari 16 px karena pengguna mungkin membaca dalam keadaan tegang. 

|Peran|Ukuran / tinggi baris|Berat|Contoh|
|---|---|---|---|
|Judul layar|28 / 36|Bold|"Bantuan apa yang kamu butuhkan?"|
|Judul bagian|20 / 28|SemiBold|"Langkah pertama"|
|Isi|16 / 24|Regular|Penjelasan panduan|
|Label tombol|16 / 20|SemiBold|"Lanjut"|
|Keterangan|13 / 18|Regular|Jam layanan, catatan|



Baris dijaga pendek dan rata kiri, satu ide per paragraf, teks tidak ditulis dengan huruf kapital semua. 

## **6. Spacing System** 

Skala kelipatan 4 px dengan satuan dasar 8 px. 

|Token|Nilai|Penggunaan|
|---|---|---|
|space-1|4 px|Jarak ikon dan label|
|space-2|8 px|Jarak dalam kelompok|
|space-3|12 px|Jarak antar elemen dalam kartu|
|space-4|16 px|Padding kartu|
|space-5|20 px|Margin sisi layar|
|space-6|24 px|Jarak antar kelompok|
|space-8|32 px|Jarak antar bagian besar|



## **7. Grid dan Layout** 

Tata letak satu kolom dengan margin sisi 20 px. Area aman (safe area) atas dan bawah dihormati pada kedua platform. Struktur tiap layar: header (judul atau tombol kembali, Quick Exit di kanan atas), konten yang dapat digulir, tindakan utama di bagian bawah, dan tab bar bila berlaku. Tindakan utama diletakkan pada area jangkauan ibu jari. Kartu memakai lebar penuh (350 px pada frame 390 px). 

Quick Exit diletakkan di pojok kanan atas pada seluruh layar 2–15 dengan posisi yang konsisten. 

## **8. Buttons dan Components** 

|Komponen|Spesifikasi|Perilaku|
|---|---|---|
|Tombol utama|Lebar penuh, tinggi 52 px, radius 14<br>px, teal, teks putih, satu per layar|Tekan: warna lebih gelap, nonaktif:<br>abu-abu dengan teks keterangan|
|Tombol sekunder|Garis teal 1,5 px, latar transparan,<br>tinggi 48 px|Untuk jalan alternatif|
|Tombol tautan|Teks teal 16 px, target 48 px|Untuk "Lewati" dan tautan<br>kontekstual|
|Quick Help|Kartu terakota besar, tinggi sekitar 112<br>px, ikon dan teks "Saya Butuh Bantuan<br>Sekarang"|Satu ketukan membuka lembar<br>Bantuan Darurat|
|Quick Exit|Pil, ikon SignOut dan label "Keluar<br>Cepat", garis netral gelap, tinggi<br>tampak 36 px dengan target sentuh 48<br>px|Satu ketukan, tanpa konfirmasi dan<br>tanpa animasi, berpindah ke layar<br>netral (KK-11)|



|Komponen|Spesifikasi|Perilaku|
|---|---|---|
|Kartu kategori|Kartu putih, radius 16 px, ikon, nama,<br>satu baris deskripsi, terpilih: garis teal<br>dan latar primer lembut|Dipilih dengan satu ketukan,<br>dilanjutkan dengan tombol utama|
|Kartu layanan|Nama, badge kategori, biaya (amber),<br>jam, aksi simpan|Ketuk membuka Detail Layanan|
|Segmented control|"Daftar" dan "Peta", tinggi 44 px|Mengganti mode tanpa<br>meninggalkan layar 10|
|Kolom pencarian|Tinggi 52 px, ikon MagnifyingGlass,<br>placeholder "Cari layanan"|Riwayat pencarian tidak disimpan|
|Chip filter|Tinggi 36 px, target 48 px|Terpilih: primer lembut dengan<br>garis teal|
|Butir checklist|Kotak centang 28 px, teks 16 px|Dicentang menjadi hijau dengan<br>ikon centang, progres diperbarui|
|Akordeon|Judul 16 px SemiBold dan ikon panah|Satu bagian terbuka pada satu<br>waktu|
|Bottom sheet|Radius atas 24 px, pegangan, overlay<br>gelap tipis|Dapat ditutup dengan tarik ke<br>bawah atau ketuk di luar|
|Tab bar|Empat tab: Beranda, Bantuan,<br>Layanan, Profil|Tab aktif: teal dengan label tebal|
|Aksi simpan|Ikon BookmarkSimple, target 48 px|Aktif: terisi hijau, ketuk lagi<br>membatalkan|
|Toggle PIN|Saklar 52 × 32 px|Aktif memulai pengaturan PIN|
|Papan PIN|Tombol angka 72 px|Tidak menampilkan angka yang<br>dimasukkan|
|Banner informasi|Latar primer lembut atau amber|Menjelaskan keadaan, mis. data<br>layanan belum tersedia|



## **9. Iconography** 

Set **Phosphor Regular** : garis halus dengan ujung membulat, familiar tetapi tidak kaku. Fungsi penting selalu disertai label teks. 

|Fungsi|Ikon|
|---|---|
|Beranda, Bantuan, Layanan, Profil|House, LifeBuoy, MagnifyingGlass, User|
|Bantuan Hukum,Pendampingan,Informasi|Scales,HandHeart,ClipboardText,Siren|



|Fungsi|Ikon|
|---|---|
|Pelaporan, Bantuan Darurat||
|Checklist|CheckCircle|
|Hak, FAQ|ShieldCheck, Question|
|Telepon, pesan|Phone, ChatCircle|
|Peta, lokasi|MapTrifold, MapPin|
|Simpan|BookmarkSimple|
|Privasi, PIN|LockKey|
|Quick Exit|SignOut|



## **10. Visual Hierarchy** 

|Tingkat|Elemen|Perlakuan|
|---|---|---|
|1|Judul layar dan pertanyaan|Ukuran 28 px, Bold, teks utama|
|2|Tindakan utama|Tombol teal lebar penuh, pada Beranda, kartu Quick<br>Help terakota|
|3|Isi dan pilihan|Kartu putih dengan teks 16 px|
|4|Informasi pendukung|Teks sekunder 13–16 px|
|5|Quick Exit|Tampak jelas tetapi ringan, posisinya yang konstan<br>membuatnya mudah ditemukan tanpa bersaing<br>dengan tindakan utama|



Setiap layar memiliki satu titik fokus (focal point). Informasi yang paling memengaruhi keputusan, seperti biaya dan jam layanan, diletakkan di bagian atas kartu. 

## **11. Gestalt Principles** 

|Prinsip|Penerapan|Layar|
|---|---|---|
|Proximity|Jarak dalam kelompok 8 px, antar kelompok 24 px|10, 11|
|Similarity|Kartu layanan dan kategori seragam, ikon satu gaya,<br>warna sama berarti fungsi sama|6, 9, 10, 14|
|Figure–ground|Kartu putih di atas latar gading, lembar bawah dengan<br>overlay|4, 11|
|Common region|Pilihan dikelompokkan dalam kartu berradius sama|6, 15|



|Prinsip|Penerapan|Layar|
|---|---|---|
|Continuity|Garis penghubung langkah dan indikator progres|2, 7, 8|
|Closure|Ikon garis sederhana dan cincin progres|8|
|Prägnanz|Satu tujuan per layar|5, 6|
|Focal point|Satu elemen beraksen per layar|4|
|Hukum Hick|Maksimal empat pilihan pada Pilih Jenis Kebutuhan|6|
|Hukum Fitts|Tombol besar pada jangkauan ibu jari|Seluruh layar|
|Hukum Jakob|Tab bawah, kolom cari, akordeon|4, 9, 14|



## **12. Design Language** 

**Nada bahasa.** Memakai "kamu", kalimat pendek, tidak menghakimi, tidak memaksa. Contoh: "Kamu tidak harus melapor sekarang." "Mulai dari langkah kecil." "Pilih yang paling sesuai, bisa diubah kapan saja." Janji teknis seperti "datamu pasti tidak tersimpan" tidak ditulis sebelum ditetapkan oleh pengembang. 

**Ilustrasi. Bentuk abstrak dan netral (lengkung lembut, bidang warna primer lembut), tanpa figur korban, tanpa adegan kekerasan.** 

**Gerak. Transisi 200–250 ms dengan perlambatan halus, mengikuti pengaturan "kurangi gerak" perangkat. Quick Exit tidak memakai animasi karena harus seketika.** 

## **13. Spesifikasi 15 Layar** 

Isi panduan, informasi hukum, hak korban, dan jawaban FAQ mengikuti materi sumber proyek (KK-10). Spesifikasi di bawah menetapkan struktur dan perilaku antarmuka. Informasi layanan berasal dari data layanan yang tersedia (KK-6). Quick Exit tampil pada layar 2–15 (FR-06 pada Dokumen 03). 

### **13.1 Splash Screen** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Memberi kesan pertama yang tenang.|
|Fungsi|Menampilkan identitas Ruang Aman selagi aplikasi dimuat.|
|Hierarki|Logo, lalu nama, lalu tagline.|
|Komponen|Logo, wordmark "Ruang Aman", tagline singkat, latar gading.|
|Konten utama|Nama aplikasi, tagline spesifikasi desain: "Tempat tenang untuk mencari<br>langkah dan bantuan".|
|Interaksi|Tidak ada,berpindah otomatis.|



|Aspek|Spesifikasi|
|---|---|
|Navigasi|Masuk: peluncuran aplikasi. Keluar: Onboarding (pertama kali) atau<br>Beranda (peluncuran berikutnya, spesifikasi desain).|
|Perilaku tombol|Tidak ada tombol. Quick Exit tidak ditampilkan karena layar berpindah<br>otomatis.|
|Kondisi khusus|Pemuatan lebih lama: indikator halus di bawah logo.|



### **13.2 Onboarding** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjelaskan nilai aplikasi dan jaminan privasi sebelum dipakai.|
|Fungsi|Tiga slide: (1) satu tempat untuk langkah dan bantuan, (2) tanpa login<br>dan ada Keluar Cepat, (3) dituntun selangkah demi selangkah.|
|Hierarki|Ilustrasi, judul, teks dua baris, indikator slide, tombol.|
|Komponen|Ilustrasi abstrak, indikator titik, tombol utama, tautan "Lewati", Quick<br>Exit.|
|Konten utama|Judul dan teks singkat tiap slide, slide 2 memperagakan posisi tombol<br>Quick Exit.|
|Interaksi|Geser antar slide atau ketuk "Lanjut".|
|Navigasi|Masuk: Splash. Keluar: Masuk/Mulai (juga lewat "Lewati").|
|Perilaku tombol|"Lanjut" menuju slide berikutnya, pada slide 3 berubah menjadi "Mulai".<br>Quick Exit berfungsi sejak layar ini (KK-3).|
|Kondisi khusus|Slide terakhir tidak dapat digeser lebih jauh.|



### **13.3 Masuk/Mulai** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Membuka aplikasi dengan hambatan serendah mungkin.|
|Fungsi|Mengantar pengguna langsung ke Beranda tanpa login (KK-2).|
|Hierarki|Judul, penjelasan satu kalimat, tombol utama, catatan privasi.|
|Komponen|Ilustrasi, tombol "Mulai", teks catatan privasi singkat, Quick Exit.|
|Konten utama|Judul spesifikasi desain: "Mulai kapan pun kamu siap", catatan bahwa|



|Aspek|Spesifikasi|
|---|---|
||aplikasi dipakai tanpa akun.|
|Interaksi|Satu ketukan pada "Mulai".|
|Navigasi|Masuk: Onboarding. Keluar: Beranda.|
|Perilaku tombol|Tidak ada formulir, kata sandi, atau verifikasi. Quick Exit berfungsi (KK-3).|
|Kondisi khusus|Tidak ada pilihan Masuk atau Daftar karena aplikasi tanpa akun.|



### **13.4 Beranda** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjadi pusat navigasi dan akses bantuan cepat.|
|Fungsi|Menyediakan Quick Help, jalan masuk ke jalur bantuan, pintasan<br>Tersimpan, dan akses ke informasi.|
|Hierarki|(1) Quick Help, (2) kartu "Butuh Bantuan", (3) ringkasan checklist bila ada<br>progres, (4) pintasan Tersimpan, (5) bagian "Pelajari".|
|Komponen|Header dengan sapaan netral dan Quick Exit, kartu Quick Help terakota,<br>kartu teal, kartu progres, tiga kartu Pelajari, tab bar.|
|Konten utama|"Saya Butuh Bantuan Sekarang", "Butuh Bantuan", "Tersimpan", Pelajari:<br>Informasi Bantuan Hukum, Kenali Hakmu, FAQ.|
|Interaksi|Ketuk kartu, geser vertikal.|
|Navigasi|Masuk: Mulai, tab Beranda. Keluar: lembar Bantuan Darurat, layar 5, 12,<br>13, 14, 15, dan tab lain.|
|Perilaku tombol|Quick Help membuka lembar Bantuan Darurat (K4) berisi kontak dari<br>data layanan, tautan ke layanan K4 (layar 10), dan tautan ke panduan<br>darurat (layar 7). Kartu Butuh Bantuan membuka layar 5.|
|Kondisi khusus|Data layanan belum tersedia: lembar menampilkan keterangan, bukan<br>kontak buatan. Belum ada progres: kartu progres tidak ditampilkan.|



### **13.5 Butuh Bantuan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjadi pintu masuk jalur bantuan dengan suasana menenangkan.|
|Fungsi|Mengajak pengguna menyatakan kebutuhan atau langsung mencari<br>layanan.|
|Hierarki|Judul,kalimatpenenang,tindakan utama,tindakan alternatif.|



|Aspek|Spesifikasi|
|---|---|
|Komponen|Judul, teks, tombol utama, tombol sekunder, kartu pintasan Bantuan<br>Darurat, tab bar, Quick Exit.|
|Konten utama|Judul spesifikasi desain: "Kamu tidak sendiri. Mulai dari mana saja.",<br>"Ceritakan kebutuhanmu", "Langsung cari layanan".|
|Interaksi|Ketuk tombol atau kartu.|
|Navigasi|Masuk: Beranda, tab Bantuan. Keluar: layar 6, layar 9, lembar Bantuan<br>Darurat.|
|Perilaku tombol|"Ceritakan kebutuhanmu" menuju layar 6, "Langsung cari layanan"<br>menuju layar 9.|
|Kondisi khusus|Tidak ada.|



### **13.6 Pilih Jenis Kebutuhan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Mengarahkan pengguna ke jalur sesuai kategori resmi (KK-9).|
|Fungsi|Pengguna memilih satu dari empat kategori.|
|Hierarki|Judul pertanyaan, empat kartu kategori, tombol lanjut.|
|Komponen|Empat kartu kategori dengan ikon, tombol utama "Lanjut", tab bar,<br>Quick Exit.|
|Konten utama|"Bantuan apa yang kamu butuhkan?", Bantuan Hukum, Pendampingan,<br>Informasi Pelaporan, Bantuan Darurat, masing-masing dengan satu baris<br>deskripsi singkat.|
|Interaksi|Ketuk kartu untuk memilih, lalu "Lanjut".|
|Navigasi|Masuk: layar 5. Keluar: layar 7 dengan kategori terpilih.|
|Perilaku tombol|"Lanjut" nonaktif sampai ada pilihan. Pilihan dapat diganti sebelum<br>lanjut.|
|Kondisi khusus|Tidak ada kategori kelima atau jalur tambahan di luar empat kategori<br>resmi.|



### **13.7 Panduan Langkah Awal** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjawab "apayangharus dilakukan lebih dahulu".|



|Aspek|Spesifikasi|
|---|---|
|Fungsi|Menyajikan langkah bernomor dari materi sumber sesuai kategori.|
|Hierarki|Judul dan chip kategori, daftar langkah, tautan kontekstual, tindakan<br>utama.|
|Komponen|Header dengan aksi simpan dan Quick Exit, daftar langkah dengan garis<br>penghubung, tautan ke layar 12 dan 13, tombol utama dan tombol<br>tautan.|
|Konten utama|Langkah dari materi sumber untuk K1–K4, setiap langkah memuat judul<br>pendek dan satu hingga dua kalimat.|
|Interaksi|Gulir, ketuk simpan, ketuk tautan.|
|Navigasi|Masuk: layar 6, lembar Bantuan Darurat. Keluar: layar 8, layar 9, layar 10<br>(K4), layar 12, layar 13.|
|Perilaku tombol|K1–K3: "Lanjut ke Checklist" (layar 8) dan tautan "Lewati ke Cari<br>Layanan". K4 (spesifikasi desain, agar bantuan segera lebih cepat): "Lihat<br>layanan Bantuan Darurat" (layar 10) dan tautan "Lihat Checklist". Simpan<br>menambah panduan ke Tersimpan.|
|Kondisi khusus|Materi untuk suatu kategori belum diterima: tampil keterangan, bukan<br>teks buatan.|



### **13.8 Checklist Panduan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Membuat langkah terstruktur dan dapat dilacak.|
|Fungsi|Pengguna menandai langkah yang sudah dilakukan, progres tersimpan di<br>perangkat.|
|Hierarki|Judul, penanda progres, daftar butir, tombol lanjut.|
|Komponen|Cincin atau bilah progres, butir dengan kotak centang, tombol utama,<br>Quick Exit.|
|Konten utama|Butir dasar dari PDF: memastikan diri berada di tempat yang aman,<br>mencari informasi layanan bantuan, menghubungi layanan yang sesuai.<br>Butir tambahan sesuai materi per kategori.|
|Interaksi|Ketuk butir untuk mencentang atau membatalkan.|
|Navigasi|Masuk: layar 7. Keluar: layar 9.|



|Aspek|Spesifikasi|
|---|---|
|Perilaku tombol|"Cari Layanan" menuju layar 9 dengan filter kategori terisi.|
|Kondisi khusus|Seluruh butir tercentang: pesan penutup yang menenangkan. Progres<br>tidak terhapus oleh Quick Exit (KK-11).|



### **13.9 Cari Layanan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menemukan layanan sesuai kebutuhan.|
|Fungsi|Pencarian kata kunci dan filter kategori.|
|Hierarki|Judul, kolom pencarian, filter kategori, tombol cari.|
|Komponen|Kolom pencarian, chip "Semua", Bantuan Hukum, Pendampingan,<br>Informasi Pelaporan, Bantuan Darurat, tombol utama, tab bar, Quick<br>Exit.|
|Konten utama|Placeholder "Cari layanan", tidak ada riwayat pencarian (spesifikasi<br>desain, demi privasi).|
|Interaksi|Ketik, pilih chip, ketuk "Cari".|
|Navigasi|Masuk: layar 8, layar 5, tab Layanan. Keluar: layar 10.|
|Perilaku tombol|"Cari" menampilkan layar 10 dengan kata kunci dan filter.|
|Kondisi khusus|Filter terisi otomatis dari kategori pilihan. Data layanan belum tersedia:<br>banner keterangan.|



### **13.10 Daftar Layanan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Membandingkan layanan yang sesuai.|
|Fungsi|Menampilkan hasil dalam mode Daftar atau mode Peta (KK-1).|
|Hierarki|Judul dan jumlah hasil, segmented control Daftar/Peta, chip filter, kartu<br>atau peta.|
|Komponen|Segmented control, kartu layanan (nama, badge kategori, biaya, jam,<br>wilayah, simpan), peta dengan titik layanan dan kartu singkat di bawah,<br>tab bar, Quick Exit.|
|Konten utama|Seluruh isi kartu berasal dari data layanan proyek.|
|Interaksi|Ketuk kartu, ganti mode, ketuk titik pada peta.|



|Aspek|Spesifikasi|
|---|---|
|Navigasi|Masuk: layar 9, layar 7 (K4), lembar Bantuan Darurat, tombol Lihat di<br>Peta dari layar 11. Keluar: layar 11.|
|Perilaku tombol|Mode Peta meminta izin lokasi hanya saat dibuka, izin dapat ditolak<br>tanpa menghalangi penggunaan.|
|Kondisi khusus|Data belum tersedia: keterangan, tanpa kartu atau titik buatan. Hasil<br>kosong: saran mengubah kata kunci atau filter.|



### **13.11 Detail Layanan** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Memberi informasi lengkap dan mempermudah menghubungi layanan.|
|Fungsi|Menampilkan detail layanan dan lembar pilihan kanal.|
|Hierarki|Nama dan kategori, informasi penting (biaya, jam), deskripsi, kontak dan<br>alamat, tombol Hubungi.|
|Komponen|Header dengan simpan dan Quick Exit, blok informasi penting, teks,<br>tautan "Lihat di Peta", tombol Hubungi Layanan terakota yang<br>menempel di bawah, lembar pilihan kanal.|
|Konten utama|Seluruh isi berasal dari data layanan proyek.|
|Interaksi|Gulir, simpan, Lihat di Peta, Hubungi.|
|Navigasi|Masuk: layar 10. Keluar: layar 10 (mode Peta), lembar Hubungi, aplikasi<br>telepon atau pesan perangkat.|
|Perilaku tombol|"Hubungi Layanan" membuka lembar dengan kanal yang tersedia pada<br>data, memilih kanal membuka aplikasi perangkat.|
|Kondisi khusus|Kanal tidak tersedia: tombol nonaktif disertai keterangan.|



### **13.12 Informasi Bantuan Hukum** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjelaskan bantuan hukum dalam bahasa sederhana.|
|Fungsi|Menyajikan penjelasan dari materi sumber dalam bagian yang dapat<br>dibuka.|
|Hierarki|Judul, ringkasan satu kalimat, bagian akordeon, tindakan.|
|Komponen|Header dengan simpan dan Quick Exit, akordeon, kotak ringkas, tombol<br>sekunder.|



|Aspek|Spesifikasi|
|---|---|
|Konten utama|Bagian mengikuti materi sumber proyek, contoh struktur spesifikasi<br>desain: pengertian, siapa yang dapat memperoleh, biaya, prosedur<br>ringkas.|
|Interaksi|Buka dan tutup bagian, simpan.|
|Navigasi|Masuk: Beranda (Pelajari), layar 7. Keluar: layar 9 dan layar 10 dengan<br>filter Bantuan Hukum.|
|Perilaku tombol|"Cari Layanan Bantuan Hukum" menuju layar 10 dengan filter K1.|
|Kondisi khusus|Materi belum diterima: keterangan, bukan teks buatan.|



### **13.13 Kenali Hakmu** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menyampaikan hak korban agar pengguna mengetahui yang dapat<br>diminta.|
|Fungsi|Menyajikan hak dalam kartu yang dapat dibuka.|
|Hierarki|Judul, kalimat pengantar, kartu hak, tindakan.|
|Komponen|Header dengan simpan dan Quick Exit, kartu hak dengan ikon<br>ShieldCheck, tombol sekunder.|
|Konten utama|Hak korban dari materi sumber proyek, ditulis dalam kalimat pendek.|
|Interaksi|Buka dan tutup kartu, simpan.|
|Navigasi|Masuk: Beranda (Pelajari), layar 7. Keluar: layar 9.|
|Perilaku tombol|"Cari Layanan" menuju layar 9.|
|Kondisi khusus|Materi belum diterima: keterangan.|



### **13.14 FAQ** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Menjawab keraguan awal pengguna yang belum siap mencari bantuan<br>(PDF).|
|Fungsi|Pertanyaan umum dalam bentuk akordeon.|
|Hierarki|Judul, daftar pertanyaan, tautan lanjutan.|
|Komponen|Akordeon, Quick Exit, tautan.|
|Konten utama|Pertanyaan awal dari PDF: harus mulai dari mana,apakah bisa|



|Aspek|Spesifikasi|
|---|---|
||mendapatkan bantuan hukum, ke mana mencari bantuan. Jawaban dari<br>materi sumber proyek.|
|Interaksi|Buka dan tutup pertanyaan.|
|Navigasi|Masuk: Beranda (Pelajari). Keluar: layar 5.|
|Perilaku tombol|Tautan "Butuh Bantuan" menuju layar 5.|
|Kondisi khusus|Jawaban belum diterima: keterangan.|



### **13.15 Profil & Pengaturan Privasi** 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Memberi kendali atas privasi dan data di perangkat tanpa akun (KK-2).|
|Fungsi|Menampilkan Tersimpan, pengaturan Quick Exit dan PIN, serta<br>pengelolaan data perangkat.|
|Hierarki|Judul dan keterangan "tanpa akun", Tersimpan, Privasi, Data.|
|Komponen|Kartu keterangan, tab Tersimpan (Layanan, Panduan, Informasi),<br>keterangan Quick Exit, toggle PIN, tombol "Ubah PIN", tombol "Hapus<br>data di perangkat", tab bar.|
|Konten utama|Tidak ada nama atau foto pengguna. Penjelasan singkat fungsi Quick Exit<br>dan PIN opsional.|
|Interaksi|Buka item tersimpan, hapus item, aktifkan atau nonaktifkan PIN.|
|Navigasi|Masuk: tab Profil, pintasan Tersimpan dari Beranda. Keluar: item<br>tersimpan ke layar 7, 11, 12, atau 13.|
|Perilaku tombol|Toggle PIN memulai pengaturan PIN dua kali masukan. "Hapus data di<br>perangkat" meminta konfirmasi karena menghapus checklist dan<br>Tersimpan (konfirmasi hanya untuk penghapusan, Quick Exit tidak<br>meminta konfirmasi).|
|Kondisi khusus|Tersimpan kosong: keterangan singkat. PIN terlupa: perilaku pemulihan<br>PIN tidak ditambahkan sebagai fitur prototype karena tidak ditetapkan<br>dalam keputusan proyek.|



### **13.16 State khusus: layar netral dan layar PIN** 

State ini bukan bagian dari 15 layar dan tidak memiliki tab bar maupun Quick Exit. 

|Aspek|Spesifikasi|
|---|---|
|Tujuan|Segera menyembunyikan konten Ruang Aman (KK-11).|
|Layar netral|Halaman sederhana dengan tampilan umum yang tidak<br>mencurigakan. Halaman tidak menampilkan logo, nama, warna<br>merek, atau teks Ruang Aman, serta tidak menampilkan konten<br>sensitif.|
|Cara kembali tanpa PIN|Jika PIN tidak diaktifkan, pengguna dapat kembali ke aplikasi<br>dari tampilan netral tanpa memasukkan PIN.|
|Cara kembali dengan PIN|Jika PIN diaktifkan, pengguna harus memasukkan PIN sebelum<br>konten aplikasi ditampilkan kembali.|
|Keamanan app switcher|Saat aplikasi di latar belakang atau setelah Quick Exit, cuplikan<br>pada daftar aplikasi terbuka ditutup dengan tampilan netral<br>(KK-11 butir 9).|
|Data|Checklist, Tersimpan, dan pengaturan tidak terhapus.|



## **14. Interaction dan Component Behavior** 

|Interaksi|Perilaku|
|---|---|
|Quick Exit|Satu ketukan, pindah ke layar netral pada saat itu juga, tanpa<br>animasi dan tanpa dialog, layar sebelumnya dapat dipulihkan<br>pada posisi terakhir.|
|Kembali dari layar netral|Sesuai bab 13.16, PIN hanya diminta bila diaktifkan.|
|Pilih kategori|Ketuk kartu menandai pilihan, "Lanjut" aktif, mengganti pilihan<br>memperbarui tanda tanpa perpindahan.|
|Checklist|Ketuk butir mencentang dengan perubahan warna dan ikon,<br>ketuk lagi membatalkan, progres diperbarui seketika.|
|Simpan|Ketuk ikon mengisi ikon dan menampilkan pesan singkat<br>"Tersimpan" dengan opsi urungkan.|
|Filter dan pencarian|Chip aktif menyaring, riwayat pencarian tidak disimpan.|
|Daftar/Peta|Mengganti mode tanpa kehilangan filter.|
|Hubungi Layanan|Membuka lembar pilihan kanal, memilih kanal membuka<br>aplikasi perangkat.|
|Bottom sheet|Dapat ditutup dengan tarik ke bawah atau ketuk di luar.|
|Tombol kembali sistem|Mundur satu layar, pada layar netral tidak membuka konten|



|Interaksi|Perilaku|
|---|---|
||Ruang Aman.|
|Gerak|Transisi 200–250 ms, mengikuti pengaturan kurangi gerak.|



## **15. UI States** 

|Keadaan|Penerapan|
|---|---|
|Default, ditekan, nonaktif|Tombol dan chip memiliki tiga keadaan, nonaktif disertai<br>keterangan penyebab bila relevan|
|Terpilih|Kartu kategori dan chip memakai garis teal dan latar primer<br>lembut|
|Selesai|Butir checklist hijau dengan ikon centang|
|Data layanan belum tersedia|Banner keterangan pada layar 4 (lembar), 9, 10, 11, tidak<br>ada nama, kontak, atau lokasi buatan (KK-6)|
|Hasil kosong|Keterangan dan saran mengubah kata kunci atau filter|
|Tersimpan kosong|Keterangan singkat pada layar 15|
|Materi belum diterima|Keterangan pada layar 7, 12, 13, 14|
|Izin lokasi ditolak|Peta tampil tanpa lokasi pengguna, pencarian tetap<br>berfungsi|
|Tidak ada koneksi|Peta tidak dapat dimuat dan ditampilkan keterangan,<br>perilaku konten lain ditentukan pengembang|
|PIN salah|Pesan netral, tetap di layar netral|
|Quick Exit aktif|Layar netral, layar sebelumnya tersembunyi, bukan dihapus|



## **16. Adaptasi Android dan iOS** 

Desain memakai satu bahasa visual pada kedua platform. Penyesuaian hanya dilakukan pada komponen sistem dan perilaku navigasi. Angka acuan platform perlu diverifikasi oleh pengembang pada versi sistem yang digunakan. 

|Aspek|Android|iOS|Ketentuan Ruang Aman|
|---|---|---|---|
|Frame desain|360 × 800 px|390 × 844 px|Tata letak adaptif 360–430 px|
|Navigasi<br>bawah|Navigation bar (acuan<br>tinggi 80 dp pada Material<br>3)|Tab bar (acuan 49 pt<br>ditambah safe area)|Empat tab yang sama, ikon<br>dan label sama|



|Aspek|Android|iOS|Ketentuan Ruang Aman|
|---|---|---|---|
|Target sentuh|Minimal 48 dp|Minimal 44 pt|48 × 48 px pada kedua<br>platform|
|Tombol<br>kembali|Tombol atau gestur<br>kembali sistem|Gestur geser dari tepi<br>dan tombol kembali di<br>header|Kembali satu layar, tidak<br>keluar dari aplikasi pada<br>tengah alur|
|Bottom sheet|Modal bottom sheet|Sheet dengan<br>pegangan|Perilaku sama: tarik ke bawah<br>untuk menutup|
|Izin lokasi|Dialog izin sistem|Dialog izin sistem|Diminta hanya saat mode<br>Peta dibuka|
|Tipografi|Plus Jakarta Sans,<br>cadangan Roboto|Plus Jakarta Sans,<br>cadangan SF Pro|Ukuran sama|
|Pengamanan<br>app switcher|Dapat memakai<br>pengaman jendela (secure<br>window flag) pada<br>aktivitas aplikasi, efek<br>samping: tangkapan layar<br>juga diblokir|Dapat menampilkan<br>tampilan penutup<br>netral saat aplikasi<br>menjadi tidak aktif|Keputusan implementasi oleh<br>pengembang, kebutuhan<br>fungsional tetap FR-11|
|Panggilan dan<br>pesan|Membuka aplikasi<br>telepon atau pesan|Membuka aplikasi<br>telepon atau pesan|Mengikuti kanal pada data<br>layanan|
|Mode gelap|Di luar lingkup|Di luar lingkup|Prototype hanya tema terang|



