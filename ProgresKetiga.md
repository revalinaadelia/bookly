# PRAKTIKUM 13: PROGRES TUBES 3 - APLIKASI CAFELORA

# 📃 Identitas Diri

- **Kelompok**         : Kelompok 1
- **Anggota Kelompok** : 
  1. Arya Wicaksana Putra (4520210092)
  2. Aditya Nur Lintang (4523210003)
  3. Alip Khoeril Akbar (4523210009)
  4. Muhammad Fauzan (4523210073)
  5. Revalina Adelia (4523210091)
  6. Chaerul Cahyadi (4523210120)
- **Mata Kuliah**      : Pemrograman Berbasis Web (A)
- **Dosen Pengampu**   : Adi Wahyu Pribadi, S.Si., M.Kom.
- **Topik Proyek**     : Cafe

---
# Latar Belakang

Perkembangan teknologi informasi telah membawa perubahan dalam berbagai sektor usaha, termasuk pada bidang kuliner dan kafe. Kafe sebagai usaha jasa dituntut untuk mampu memberikan pelayanan yang cepat, akurat, dan efisien guna meningkatkan kepuasan pelanggan serta mendukung kelancaran operasional. Dalam aktivitas sehari-hari, kafe melibatkan proses penyajian informasi menu, pencatatan pesanan, transaksi pembayaran, hingga pengelolaan data penjualan. Apabila proses tersebut masih dilakukan secara manual atau tidak terintegrasi, maka berpotensi menimbulkan permasalahan seperti kesalahan pencatatan, keterlambatan pelayanan, serta kesulitan dalam penyusunan laporan penjualan.

Selain itu, perubahan perilaku pelanggan yang semakin terbiasa dengan pembayaran digital menuntut kafe untuk menyediakan metode pembayaran yang lebih fleksibel. Keterbatasan sistem pembayaran yang hanya mengandalkan transaksi tunai dapat mengurangi kenyamanan pelanggan dan memperlambat proses transaksi. Di sisi lain, pengelola kafe juga menghadapi kendala dalam memantau stok, mengevaluasi performa penjualan harian maupun bulanan, serta mengambil keputusan berdasarkan data yang akurat apabila belum didukung oleh sistem yang terstruktur.

Berdasarkan permasalahan tersebut, diperlukan sebuah sistem aplikasi yang mampu mengintegrasikan seluruh proses operasional kafe dalam satu platform yang terpusat dan mudah digunakan. Oleh karena itu, dibuatlah Cafelora, yaitu sistem yang dirancang untuk mendukung operasional kafe modern melalui sistem pemesanan, transaksi, dan pengelolaan data yang terintegrasi. Cafelora menyediakan tampilan menu yang informatif bagi pelanggan, sistem Point of Sale (POS) yang terstruktur untuk kasir, serta dukungan pembayaran non-tunai melalui integrasi payment gateway. Dengan adanya aplikasi ini, diharapkan proses pelayanan kafe dapat berjalan lebih efisien, akurat, dan responsif, sekaligus membantu pengelola kafe dalam meningkatkan kualitas layanan dan efektivitas operasional secara keseluruhan.

---
# Tujuan Proyek

Tujuan dari pembuatan aplikasi *Cafelora* adalah sebagai berikut:
1. Membuat sistem aplikasi yang mampu mendukung operasional kafe secara terintegrasi dan terstruktur.
2. Menyediakan sistem pemesanan dan transaksi yang cepat, akurat, serta mudah digunakan oleh kasir dan staf.
3. Menyajikan informasi menu secara jelas dan informatif untuk membantu pelanggan dalam memilih produk.
4. Mendukung proses pembayaran baik secara tunai maupun non-tunai melalui integrasi *payment gateway*.
5. Membantu pengelola kafe dalam mengelola data menu, stok, serta laporan penjualan secara efisien sebagai bahan evaluasi usaha.

---
# Kondisi Objek Permasalahan

Berdasarkan hasil pengamatan terhadap proses operasional kafe, diperoleh beberapa kondisi permasalahan sebagai berikut:
1. Proses pemesanan dan pencatatan transaksi masih berpotensi dilakukan secara manual atau tidak terintegrasi dalam satu sistem.
2. Informasi menu belum disajikan secara terstruktur sehingga kurang optimal dalam membantu pelanggan.
3. Kesalahan dalam perhitungan harga dan pencatatan transaksi masih mungkin terjadi.
4. Metode pembayaran yang tersedia masih terbatas dan belum sepenuhnya mendukung transaksi non-tunai.
5. Proses pengelolaan laporan penjualan dan pemantauan performa usaha belum berjalan secara efisien dan sistematis.

---
# Solusi yang Ditawarkan

Sebagai upaya untuk mengatasi permasalahan tersebut, aplikasi *Cafelora* menawarkan solusi berupa:
1. Penerapan sistem pemesanan dan transaksi terintegrasi berbasis aplikasi.
2. Penyediaan tampilan menu yang informatif dan mudah dipahami oleh pelanggan.
3. Penggunaan sistem *Point of Sale* (POS) dengan perhitungan harga otomatis untuk meminimalkan kesalahan transaksi.
4. Integrasi *payment gateway* guna mendukung proses pembayaran non-tunai yang lebih fleksibel.
5. Penyediaan fitur laporan penjualan dan visualisasi data sebagai pendukung evaluasi dan pengambilan keputusan pengelola kafe.

---
# Deskripsi Cafelora

Cafelora merupakan sistem yang dirancang untuk mendukung operasional kafe modern melalui sistem pemesanan, transaksi, dan pengelolaan data yang terintegrasi. Sistem ini dibuat untuk membantu kafe dalam menyajikan informasi menu secara jelas, memproses pesanan dengan lebih terstruktur, serta mempercepat alur transaksi secara efisien. 

Dalam penerapannya, Cafelora menyediakan antarmuka pelanggan yang informatif untuk memudahkan pemilihan menu, serta antarmuka kasir yang sederhana namun sistematis guna meminimalkan kesalahan dalam proses pemesanan dan pembayaran. Pendekatan digital yang diterapkan memungkinkan alur pelayanan kafe menjadi lebih tertata, meningkatkan efisiensi kerja staf, serta membantu pengelola dalam memantau dan mengelola aktivitas oeprasional secara lebih efektif.

Sebagai solusi berbasis aplikasi, Cafelora berperan dalam mendukung peningkatan kualitas layanan dan kelancaran operasional kafe secara keseluruhan melalui sistem yang praktis, terstruktur, dan mudah digunakan.

---
# Aktor yang Terlibat dalam Sistem

Dalam implementasi aplikasi Cafelora, sistem melibatkan beberapa aktor yang memiliki peran dan hak akses berbeda sesuai dengan kebutuhan operasional kafe. Pembagian aktor ini bertujuan untuk memastikan setiap proses berjalan secara terstruktur serta menghindari penyalahgunaan akses terhadap fitur tertentu.

## 1. Admin

Admin berperan sebagai pengelola utama sistem. Admin memiliki hak akses penuh terhadap fitur manajemen data, termasuk pengelolaan menu, kategori, varian, topping, data pengguna, serta pemantauan laporan penjualan. Selain itu, admin juga bertanggung jawab dalam mengatur alur status transaksi dan memastikan sistem berjalan sesuai kebutuhan operasional kafe.

## 2. Kasir/Staf

Kasir atau staf bertugas menangani proses transaksi penjualan secara langsung. Aktor ini memiliki akses ke sistem Point of Sale (POS) untuk mencatat pesanan pelanggan, melakukan perhitungan total harga secara otomatis, menerima pembayaran, serta mencetak struk transaksi. Akses kasir dibatasi hanya pada fitur yang berkaitan dengan transaksi agar proses operasional tetap terkontrol.

## 3. Pelanggan

Pelanggan merupakan pengguna sistem pada sisi frontend. Pelanggan dapat mengakses sistem untuk melihat daftar menu, melakukan pencarian dan penyaringan menu berdasarkan kategori atau varian, serta melihat detail informasi setiap menu. Peran pelanggan difokuskan pada kemudahan dalam memperoleh informasi menu tanpa memiliki akses ke proses pengelolaan data atau transaksi internal.

---
# Functional Requirement Aplikasi Cafelora

*Functional requirement* berikut menjelaskan kemampuan utama yang harus dimiliki oleh sistem Cafelora agar dapat mendukung operasional kafe secara optimal sesuai dengan peran masing-masing pengguna.
1. Sistem dapat mengelola data menu kafe yang meliputi penambahan, perubahan, dan penghapusan menu, kategori, varian, serta topping oleh admin.
2. Sistem dapat menyimpan dan menampilkan gambar menu untuk setiap item agar informasi menu dapat disajikan secara visual dan informatif kepada pelanggan.
3. Sistem dapat mencatat dan memperbarui stok menu secara otomatis berdasarkan transaksi yang terjadi.
4. Sistem dapat mengelola data pengguna dengan peran berbeda, seperti admin dan kasir, serta membatasi akses fitur sesuai dengan peran masing-masing.
5. Sistem dapat menerima dan memproses pesanan yang terdiri dari beberapa item menu, termasuk penambahan topping atau varian sesuai pilihan pengguna.
6. Sistem dapat menghitung total harga pesanan secara otomatis berdasarkan menu, varian, dan topping yang dipilih.
7. Sistem dapat memproses pembayaran tunai dengan fitur input uang bayar dan perhitungan kembalian secara otomatis.
8. Sistem dapat mendukung pembayaran non-tunai melalui integrasi *payment gateway* sebagai alternatif metode pembayaran.
9. Sistem dapat mengelola status transaksi mulai dari pemesanan hingga transaksi selesai sesuai dengan alur yang telah ditentukan.
10. Sistem dapat menghasilkan struk transaksi dalam bentuk digital yang dapat dicetak atau disimpan dalam format HTML atau PDF.
11. Sistem dapat menampilkan daftar menu makanan dan minuman kepada pelanggan secara jelas dan terstruktur melalui antarmuka frontend.
12. Sistem dapat menyediakan fitur pencarian atau filter menu berdasarkan nama, harga, dan kategori untuk memudahkan pelanggan dalam memilih menu.
13. Sistem dapat menghasilkan laporan transaksi penjualan berdasarkan periode tertentu untuk membantu evaluasi usaha.
14. Sistem dapat menampilkan grafik atau chart penjualan sebagai ringkasan performa transaksi harian dan bulanan.
15. Sistem dapat mengekspor laporan transaksi ke dalam format PDF atau Excel untuk kebutuhan dokumentasi dan analisis lanjutan.

---
# Fitur Aplikasi Cafelora

## Fitur Admin

### 1. CRUD Menu, Kategori, Varian, dan Topping

Fitur ini memungkinkan admin untuk menambah, mengubah, menghapus, dan melihat data menu berdasarkan kategori, varian, dan topping yang tersedia. Dengan adanya fitur ini, admin dapat memastikan data menu selalu terbarui dan sesuai dengan kebutuhan operasional kafe.

### 2. Upload dan Manajemen Gambar Menu

Admin dapat mengunggah dan mengelola gambar menu yang ditampilkan pada sistem. Gambar menu berfungsi sebagai informasi visual bagi pelanggan agar lebih mudah mengenali produk yang ditawarkan.

### 3. Sistem Manajemen Stok Otomatis

Sistem secara otomatis mengelola stok berdasarkan transaksi yang terjadi. Fitur ini membantu admin dalam memantau ketersediaan produk dan mengurangi risiko kesalahan pencatatan stok.

### 4. Workflow Status Transaksi dari Awal hingga Selesai

Fitur ini mengatur alur status transaksi mulai dari pesanan dibuat hingga transaksi selesai. Dengan workflow ini, admin dapat memantau proses transaksi secara lebih terstruktur.

### 5. Pengelolaan User

Admin memiliki akses untuk mengelola data pengguna sistem, termasuk menambah, mengubah, atau menghapus akun kasir dan staf sesuai dengan kebutuhan operasional.

### 6. Dashboard Pendapatan serta Grafik Penjualan Harian dan Bulanan

Dashboard menyajikan ringkasan pendapatan dan grafik penjualan dalam periode tertentu. Fitur ini membantu admin dalam memantau performa usaha secara cepat dan informatif.

### 7. Export Laporan Transaksi ke Format PDF/Excel

Admin dapat mengekspor laporan transaksi ke dalam format PDF atau Excel untuk keperluan dokumentasi, evaluasi, maupun pelaporan.

---
## Fitur Kasir/Staf (POS)

### 1. Input Pesanan menggunakan Komponen Repeater

Kasir dapat memasukkan beberapa item pesanan dalam satu transaksi secara fleksibel. Komponen repeater memudahkan pengelolaan item tanpa perlu mengulang proses input.

### 2. Penambahan Topping dan Modifier secara Dinamis

Fitur ini memungkinkan kasir menambahkan topping atau modifier pada menu sesuai dengan permintaan pelanggan, sehingga pesanan menjadi lebih variatif.

### 3. Perhitungan Total Harga secara Otomatis

Sistem secara otomatis menghitung total harga pesanan berdasarkan item, topping, dan jumlah yang dipilih, sehingga meminimalkan kesalahan perhitungan.

### 4. Fitur Input Uang Bayar dan Kalkulasi Kembalian

Kasir dapat memasukkan nominal pembayaran pelanggan, dan sistem akan menghitung jumlah kembalian secara otomatis.

### 5. Cetak Struk Transaksi dalam Bentuk PDF/HTML

Setelah transaksi selesai, sistem menyediakan struk dalam format PDF atau HTML yang dapat dicetak atau disimpan sebagai bukti transaksi.

### 6. Akses Halaman yang Dibatasi sesuai Role

Kasir hanya dapat mengakses fitur yang berkaitan dengan transaksi, sehingga keamanan dan fokus kerja tetap terjaga.

---
## Fitur Pelanggan (Frontend)

### 1. Melihat Daftar Menu Makanan dan Minuman

Pelanggan dapat melihat seluruh menu yang tersedia beserta informasi dasar seperti nama dan harga produk.

### 2. Filter Menu Berdasarkan Nama, Harga, dan Kategori

Fitur filter membantu pelanggan dalam menyaring menu sesuai dengan nama, harga, dan kategori yang diinginkan.

### 3. Tampilan Menu Berbentuk Kartu 

Menu ditampilkan dalam bentuk kartu untuk memudahkan pelanggan dalam melihat dan memilih produk secara visual.

### 4. Halaman Detail Menu 

Halaman ini menyajikan informasi lebih lengkap mengenai menu, seperti deskripsi dan detail tambahan yang relevan.

---
## Fitur Tambahan (Opsional)

### 1. Integrasi Payment Gateway (Midtrans atau Xendit)

Sistem mendukung pembayaran non-tunai melalui integrasi *payment gateway* untuk memberikan fleksibilitas metode pembayaran kepada pelanggan.

### 2. Filter Laporan Berdasarkan Tanggal dan Status Transaksi

Admin dapat menyaring laporan transaksi berdasarkan rentang waktu dan status tertentu agar analisis data lebih terfokus.

### 3. Fitur Chart Penjualan untuk Monitoring Transaksi 7 Hari Terakhir

Grafik penjualan disediakan untuk membantu pemantauan tren transaksi dalam jangka waktu pendek secara visual.

---
# Pembagian Jobdesk

## 1. Chaerul Cahyadi (Ketua) (4523210120)

1. Menyusun struktur proyek secara keseluruhan.
2. Mengintegrasikan fitur transaksi dan perhitungan harga.
3. Menangani dashboard serta visualisasi data laporan.
4. Melakukan final review terhadap seluruh fitur.

## 2. Arya Wicaksana Putra (4520210092)

1. Mendesain ERD serta relasi antar tabel database.
2. Membuat CRUD data master seperti kategori dan topping.
3. Mengimplementasikan validasi form dan upload gambar menu.

## 3. Aditya Nur Lintang (4523210003)

1. Melakukan setup awal Laravel dan Filament.
2. Mengimplementasikan role, Policy, dan access control.
3. Mengelola user Admin dan Staff.

## 4. Alip Khoeril Akbar (4523210009)

1. Mendesain UI untuk tampilan menu pelanggan (frontend).
2. Mengatur layout grid pada halaman menu.
3. Membuat komponen kartu menu dan fitur filter.

## 5. Muhammad Fauzan (4523210073)

1. Membuat fitur POS kasir.
2. Mengimplementasikan Repeater item transaksi dan kalkulasi otomatis.
3. Membuat fitur cetak struk dalam format HTML-PDF.

## 6. Revalina Adelia (4523210091)

1. Membuat fitur laporan dan export PDF/Excel.
2. Mengatur workflow status transaksi.
3. Menyusun dokumentasi teknis proyek dan README.

---
# Teknologi yang Digunakan

Aplikasi Cafelora dibangun menggunakan kombinasi teknologi backend, forntend, dan database yang saling terintegrasi untuk mendukung proses operasional kafe secara optimal. Pemilihan teknologi ini didasarkan pada kebutuhan pengembangan aplikasi yang terstruktur, mudah dikembangkan, serta sesuai dengan praktik pembuatan aplikasi web modern.

| Teknologi         | Versi  | Keterangan                                                                                                                                     | 
|-------------------|--------|------------------------------------------------------------------------------------------------------------------------------------------------|
| PHP               | ^8.2   | Bahasa pemrograman server-side yang digunakan untuk menangani logika bisnis, proses transaksi, dan pengelolaan data aplikasi.                  |
| Laravel Framework | ^12.0  | Framework PHP berbasis MVC yang digunakan untuk mengatur alur aplikasi, mulai dari routing, controller, model, hingga view secara terstruktur. | 
| Composer          | Latest | Dependency manager PHP yang digunakan untuk mengelola library dan package yang dibutuhkan oleh Laravel.                                        | 
| NPM               | Latest | Package manager JavaScript yang digunakan untuk mengelola dependency frontend.                                                                 |
| Vite              | Latest | Build tool frontend yang digunakan untuk mengelola dan mengompilasi aset frontend agar lebih cepat dan optimal.                                | 
| MySQL/PostgreSQL  | Latest | Database relasional yang digunakan untuk menyimpan data aplikasi seperti menu, transaksi, pengguna, dan laporan penjualan.                     | 
| Filament          | ^3.3   | Admin panel Laravel yang digunakan untuk mempercepat pembuatan fitur CRUD, form, tabel, serta manajemen data pada sisi admin dan kasir.        |

---
# Persyaratan Sistem

Sebelum menjalankan aplikasi Cafelora, perangkat yang digunakan harus memenuhi beberapa persyaratan sistem agar aplikasi dapat berjalan dengan baik dan stabil.

## 1. PHP >= 8.2

Digunakan sebagai runtime utama aplikasi Laravel. Versi ini dipilih karena kompatibel dengan Laravel 12 dan mendukung fitur bahasa terbaru.

## 2. Composer

Digunakan untuk mengelola dependency PHP yang dibutuhkan oleh framework Laravel dan library pendukung lainnya.

## 3. Node.js & NPM     

Digunakan untuk menjalankan proses instalasi dependency frontend serta membangun aset frontend menggunakan Vite.

## 4. MySQL atau PostgreSQL

Digunakan sebagai sistem manajemen basis data untuk menyimpan seluruh data aplikasi.

## 5. Web Server           

Aplikasi dapat dijalankan menggunakan web server seperti Apache atau Nginx, maupun menggunakan Laravel built-in server untuk kebutuhan development.

Untuk pengguna sistem operasi Windows, disarankan menggunakan salah satu tools berikut:
1. *Laragon*, karena menyediakan PHP, MySQL, dan Apache dalam satu paket sehingga memudahkan proses setup.
2. *XAMPP*, sebagai alternatif server lokal yang umum digunakan.
3. *Herd*, sebagai alternatif yang lebih ringan untuk pengembangan Laravel secara lokal.

---
# Langkah Instalasi

## 1. Clone atau Download Repository

```bash
# Clone repository (jika menggunakan git)
https://github.com/xnoname2003/cafelora.git
cd cafelora
```

Langkah ini bertujuan untuk memperoleh kode sumber aplikasi Cafelora. Repository dapat di-clone menggunakan Git atau diunduh secara manual. Setelah proses selesai, pengguna masuk ke direktori proyek untuk melanjutkan ke tahap instalasi berikutnya.

## 2. Install Dependencies PHP

```bash
composer install
```

Perintah ini digunakan untuk menginstal seluruh dependency PHP yang dibutuhkan oleh aplikasi Laravel. Dependency tersebut didefinisikan dalam file `composer.json` dan diperlukan agar aplikasi dapat berjalan sesuai dengan konfigurasi yang telah ditentukan.

## 3. Install Dependencies JavaScript

```bash
npm install
```

Perintah ini digunakan untuk menginstal seluruh dependency JavaScript yang dibutuhkan untuk pengelolaan frontend aplikasi. Dependency ini mencakup library pendukung antarmuka dan proses build aset frontend menggunakan Vite.

## 4. Konfigurasi Environment

```bash
# Copy file .env.example menjadi .env
copy .env.example .env

# Generate application key
php artisan key:generate
```

Langkah ini dilakukan untuk menyiapkan file konfigurasi environment aplikasi:
1. File `.env` digunakan untuk menyimpan konfigurasi penting seperti koneksi database dan pengaturan aplikasi.
2. Perintah `php artisan key:generate` digunakan untuk membuat *application key* yang berfungsi menjaga keamanan data, seperti enkripsi session dan informasi sensitif lainnya.

## 5. Konfigurasi Database

Pengguna perlu menyesuaikan konfigurasi database pada file `.env` agar aplikasi dapat terhubung dengan database lokal.

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=cafelora
DB_USERNAME=root
DB_PASSWORD=
```

Pengaturan ini meliputi jenis database, alamat server, port, nama database, serta kredensial yang digunakan. Pastikan database dengan nama yang sesuai sudah dibuat sebelumnya.

## 6. Jalankan Migration & Seeder

```bash
# Membuat tabel-tabel di database
php artisan migrate

# (Optional) Generate data dummy untuk testing
php artisan db:seed
```

1. `php artisan migrate` digunakan untuk membuat seluruh tabel database berdasarkan file migration.
2. `php artisan db:seed` bersifat opsional dan digunakan untuk mengisi database dengan data awal (dummy) agar aplikasi dapat langsung diuji tanpa memasukkan data secara manual.

## 7. Build Assets Frontend

```bash
# Untuk development (dengan hot reload)
npm run dev

# Untuk production
npm run build
```

1. `npm run dev` digunakan pada tahap pengembangan karena mendukung *hot reload* sehingga perubahan kode frontend dapat langsung terlihat.
2. `npm run build` digunakan untuk membangun aset frontend versi production yang lebih optimal.

## 8. Jalankan Aplikasi

```bash
# Menggunakan Laravel built-in server
php artisan serve
```

Perintah ini digunakan untuk menjalankan *Laravel built-in server*. Setelah server berjalan, aplikasi dapat diakses melalui browser pada alamat:

`http://127.0.0.1:8000`

---
# Agenda Pekerjaan di GitHub

---

| No. | Nama               | Fitur                                        | Deskripsi Progres                                                                                       | Tanggal Push GitHub |
|-----|--------------------|----------------------------------------------|---------------------------------------------------------------------------------------------------------|---------------|
| 1.  | Chaerul Cahyadi    | Tidak Ada                                                       | Inisialisasi Cafelora                                                                                     | 26/11/2025        |
| 2.  | Aditya Nur Lintang | Manajemen User dan Role                                         | Setup Laravel + Filament, Implementasi Role + Policy (Admin, Staff, Customer)                                                                                    | 26/11/2025        |
| 3.  | Chaerul Cahyadi    | Tidak Ada                                                       | Fix Error Implementasi Role Policy                                                                                       | 27/11/2025        |
| 4.  | Chaerul Cahyadi    | Menu Management                                                 | ERD dan Struktur Tabel Sistem Cafelora                                                                                     | 29/11/2025        |
| 5.  | Chaerul Cahyadi    | Tidak Ada                                                       | Update .env.example                                                                                      | 29/11/2025        |
| 6.  | Chaerul Cahyadi    | Tidak Ada                                                       | Update Policy dan Crud Menu Management                                                                                   | 30/11/2025        |
| 7.  | Chaerul Cahyadi    | Tidak Ada                                                       | Fix Policy                                                                                       | 30/11/2025        |
| 8.  | Alip Khoeril Akbar | Frontend (Pelanggan)                                            | Membuat Frontend Untuk Pelanggan Melihat Daftar Menu dan Sedikit Penyesuaian Code Pada MenuResource.php                                                       | 30/11/2025        |
| 9.  | Chaerul Cahyadi    | Tidak Ada                                                       | Update ERD Documentation and Replace Image                                                                                        | 6/12/2025         |
| 10. | Chaerul Cahyadi    | Tidak Ada                                                       | Fix Landing Page and ERD                                                                                          | 6/12/2025         |
| 11. | Alip Khoeril Akbar | Frontend (Pelanggan)                                            | Modifikasi Tampilan Frontend Pelanggan                                                                                    | 6/12/2025         |
| 12. | Alip Khoeril Akbar | Frontend (Pelanggan)                                            | Membuat Fitur Search Pada Halaman Frontend (Pelanggan) Berdasarkan Nama menu, Harga, Kategori                                                                        | 7/12/2025         |
| 13. | Alip Khoeril Akbar | Frontend (Pelanggan)                                            | Membuat Fitur Search Pada Halaman Frontend (Pelanggan) Berdasarkan Nama menu, Harga, Kategori                                                                        | 8/12/2025         |
| 14. | Alip Khoeril Akbar | Frontend (Pelanggan)                                            | Fix URL Filter Frontend (Pelanggan)                                                                                  | 10/12/2025        |
| 15. | Muhammad Fauzan    | Menu Transaction Management                                     | Transactions dan POS Kasir                                                                                        | 10/11/2025        |
| 16. | Revalina Adelia    | Dokumentasi                                                     | Menambahkan Dokumentasi Fitur, Tampilan, Instalasi, dan Agenda                                                                                       | 12/12/2025        |
| 17. | Alip Khoeril Akbar | Membuat Halaman Detail Menu dari Setiap Menu                    | Membuat Halaman Detail Menu dari Setiap Menu                                                                                         | 13/12/2025        |
| 18. | Alip Khoeril Akbar | Membuat Section Rekomendasi Menu (BestSeller) dan Fix Responsif | Membuat Section Rekomendasi Menu (BestSeller) dan Fix Responsif                                                                                    | 13/12/2025        |
| 19. | Muhammad Fauzan    | Responsive POS Kasir, BestSeller Menu, dan fitur struk          | Menambahkan Fitur Responsive pada Halaman POS, BestSeller serta Struk untuk Otomatisasi Print                                                                      | 13/12/2025        |
| 20. | Chaerul Cahyadi    | Metode Pembayaran                                               | Implementasi Payment Gateway Midtrans                                                                                     | 17/12/2025        |
| 21. | Revalina Adelia    | Dokumentasi                                                     | Menambahkan Pendahuluan dan Tampilan, Update Fitur + Instalasi + Agenda | 17/12/2025 |

---
# Agenda Presentasi Progres Tugas Besar

| No. | Hari/Tanggal           | Presentasi ke-             | Hasil Progres                                                                                                       |
|-----|------------------------|----------------------------|---------------------------------------------------------------------------------------------------------------------|
| 1.  | Rabu, 10 Desember 2025 | Presentasi Progres Pertama | Master Menu, Dashboard Filament, GitHub dan Branch sudah Berjalan                                                   |
| 2.  | Rabu, 17 Desember 2025 | Presentasi Progres Kedua   | Role dan Policy, CRUD (User, Menu, Category, Variant), Tampilan Frontend, POS Kasir, Integrasi Payment Gateway, dan Dokumentasi |

---
# Bukti Dokumentasi Presentasi

## 1. Rabu, 10 Desember 2025 (Progres Pertama)

<img width="1919" height="1079" alt="PresentasiProgresPertama" src="https://github.com/user-attachments/assets/61457389-3ae4-40cd-88c9-5de514c35383" />

## 2. Rabu, 17 Desember 2025 (Progres Kedua)
<img width="1365" height="767" alt="PresentasiProgresKedua" src="https://github.com/user-attachments/assets/e3343e38-3d15-4c76-be62-4524444257eb" />

---
# Rekap Uji Fungsionalitas & Status Progres Pengembangan Fitur

Bagian ini menyajikan hasil *uji fungsionalitas* serta *perkembangan progres fitur* aplikasi *Cafelora* yang dikerjakan secara kolaboratif oleh tim. Dokumentasi disusun berdasarkan *tahapan waktu pengembangan* untuk menunjukkan alur pengerjaan mulai dari *inisialisasi sistem, pengembangan fitur inti,* hingga *finalisasi dan validasi*.

Pengembangan dimulai pada *26 November 2025* dan berlangsung secara bertahap hingga tahap penyelesaian.

---
## Tahap 1 - Inisialisasi Sistem & Fondasi Fitur (Rabu, 26 November 2025 - Selasa, 2 Desember 2025)

### 1. Chaerul Cahyadi (Ketua)

| No. | Fitur                     | Deskripsi Uji                                               | Status      | Tanggal Mulai     |
|-----|---------------------------|-------------------------------------------------------------|-------------|-------------------|
| 1   | Struktur Proyek & Routing | Validasi struktur folder Laravel dan routing utama aplikasi | ✅ Selesai  | 26 November 2025  |
| 2   | Review Awal Fitur Tim     | Pengecekan awal hasil pekerjaan anggota                     | 🔄 Berjalan | 26 November 2025  |
| 3   | Dashboard Admin           | Tampilan dashboard admin berhasil ditampilkan               | ✅ Selesai  | 29 November 2025  |

### 2. Arya Wicaksana Putra

| No. | Fitur                   | Deskripsi Uji                                         | Status     | Tanggal Mulai    |
|-----|-------------------------|-------------------------------------------------------|------------|------------------|
| 1   | Desain ERD              | ERD disusun dan disesuaikan dengan kebutuhan sistem   | ✅ Selesai | 29 November 2025 |
| 2   | CRUD Kategori & topping | Operasi tambah, ubah, hapus, dan tampil data berjalan | ✅ Selesai | 29 November 2025 |
| 3   | Validasi Form           | Validasi input dan format data berjalan sesuai aturan | ✅ Selesai | 29 November 2025 |
| 4   | Upload Gambar Menu      | Upload dan preview gambar menu berhasil               | ✅ Selesai | 29 November 2025 |

### 3. Aditya Nur Lintang

| No. | Fitur                    | Deskripsi Uji                                    | Status     | Tanggal Mulai    |
|-----|--------------------------|--------------------------------------------------|------------|------------------|
| 1   | Setup Laravel & Filament | Proyek berhasil dijalankan dan panel admin siap  | ✅ Selesai | 26 November 2025 |
| 2   | Role & Policy            | Hak akses Admin dan Staf terdefinisi dengan baik | ✅ Selesai | 26 November 2025 |
| 3   | Manajemen User           | CRUD user berjalan tanpa error                   | ✅ Selesai | 26 November 2025 |

### 4. Alip Khoeril Akbar

| No. | Fitur               | Deskripsi Uji                                       | Status           | Tanggal Mulai    |
|-----|---------------------|-----------------------------------------------------|------------------|------------------|
| 1   | Tampilan Grid Menu  | Grid menu tampil responsif di berbagai ukuran layar | ✅ Selesai       | 30 November 2025 |
| 2   | Responsivitas UI    | Tampilan konsisten di mobile dan desktop            | ✅ Selesai       | 30 November 2025 |

### 5. Revalina Adelia

| No. | Fitur                  | Deskripsi Uji                                    | Status      | Tanggal Mulai    |
|-----|------------------------|--------------------------------------------------|-------------|------------------|
| 1   | Dokumentasi Awal       | Struktur README dan folder dokumentasi disiapkan | 🔄 Berjalan | 26 November 2025 |

---
## Tahap 2 - Pengembangan Fitur Inti & Frontend (Rabu, 3 Desember 2025 - Selasa, 9 Desember 2025)

### 1. Chaerul Cahyadi (Ketua)

| No. | Fitur                       | Deskripsi Uji                                                                                              | Status      | Tanggal Mulai    |
|-----|-----------------------------|------------------------------------------------------------------------------------------------------------|-------------|------------------|
| 1   | Review & Validasi Lanjutan  | Validasi hasil card menu, filter kategori dan harga, penambahan item transaksi, dan dropdown menu & varian | 🔄 Berjalan | 26 November 2025 |

### 2. Alip Khoeril Akbar

| No. | Fitur               | Deskripsi Uji                              | Status     | Tanggal Mulai    |
|-----|---------------------|--------------------------------------------|------------|------------------|
| 1   | Komponen Card Menu  | Informasi menu tampil lengkap              | ✅ Selesai | 6 Desember 2025  |
| 2   | Filter Kategori     | Menu menyesuaikan kategori yang dipilih    | ✅ Selesai | 8 Desember 2025  |
| 3   | Filter Harga        | Filter harga minimum dan maksimum berjalan | ✅ Selesai | 8 Desember 2025  |

### 3. Muhammad Fauzan

| No. | Fitur                     | Deskripsi Uji                        | Status           | Tanggal Mulai    |
|-----|---------------------------|--------------------------------------|------------------|------------------|
| 1   | Penambahan Item Transaksi | Item transaksi dapat ditambahkan     | ✅ Selesai       | 5 Desember 2025  |
| 2   | Dropdown Menu & Varian    | Harga dan varian terupdate otomatis  | ✅ Selesai       | 8 Desember 2025  |

---
## Tahap 3 - Integrasi Sistem & Penyempurnaan (Rabu, 10 Desember 2025 - Selasa, 16 Desember 2025)

### 1. Chaerul Cahyadi (Ketua)

| No. | Fitur                       | Deskripsi Uji                                   | Status      | Tanggal Mulai    |
|-----|-----------------------------|-------------------------------------------------|-------------|------------------|
| 1   | Review & Validasi Lanjutan  | Validasi hasil detail menu dan POS              | 🔄 Berjalan | 26 November 2025 |

### 2. Alip Khoeril AKbar

| No. | Fitur               | Deskripsi Uji                              | Status     | Tanggal Mulai    |
|-----|---------------------|--------------------------------------------|------------|------------------|
| 1   | Halaman Detail Menu | Informasi detail menu ditampilkan lengkap  | ✅ Selesai | 12 Desember 2025 |

### 3. Muhammad Fauzan

| No. | Fitur                    | Deskripsi Uji                            | Status     | Tanggal Mulai    |
|-----|--------------------------|------------------------------------------|------------|------------------|
| 1   | Tampilan Awal POS        | Struktur dasar halaman POS ditampilkan   | ✅ Selesai | 10 Desember 2025 |
| 2   | Kalkulasi Total Otomatis | Subtotal & total transaksi valid         | ✅ Selesai | 10 Desember 2025 |
| 3   | Input Bayar & Kembalian  | Logika pembayaran dan kembalian berjalan | ✅ Selesai | 10 Desember 2025 |
| 4   | Cetak Struk              | Template struk HTML/PDF berhasil dicetak | ✅ Selesai | 12 Desember 2025 |

### 4. Revalina Adelia

| No. | Fitur             | Deskripsi Uji                        | Status           | Tanggal Mulai    |
|-----|-------------------|--------------------------------------|------------------|------------------|
| 1   | Halaman Laporan   | Data laporan transaksi ditampilkan   | 🔄 Dalam Progres | 17 Desember 2025 |
| 2   | Filter Laporan    | Filter tanggal & status dikembangkan | 🔄 Dalam Progres | 17 Desember 2025 |
| 3   | Export PDf/Excel  | Fitur ekspor laporan dikembangkan    | 🔄 Dalam Progres | 17 Desember 2025 |

---
## Tahap 4 - Finalisasi & Validasi Akhir (Rabu, 17 Desember 2025 - Selasa, 23 Desember 2025)

### 1. Chaerul Cahyadi (Ketua)

| No. | Fitur                       | Deskripsi Uji                                   | Status      | Tanggal Mulai    |
|-----|-----------------------------|-------------------------------------------------|-------------|------------------|
| 1   | Review Akhir                | Pengecekan akhir pada keseluruhan sistem        | ✅ Selesai  | 26 November 2025 |
| 2   | Integrasi Logika Transaksi  | Relasi transaksi dan item terhubung dengan baik | ✅ Selesai  | 17 Desember 2025 |

### 2. Revalina Adelia

| No. | Fitur                     | Deskripsi Uji                                | Status     | Tanggal Mulai    |
|-----|---------------------------|----------------------------------------------|------------|------------------|
| 1   | Halaman Laporan           | Tabel laporan tervalidasi                    | ✅ Selesai | 17 Desember 2025 |
| 2   | Filter Laporan            | Filter berfungsi sesuai kebutuhan            | ✅ Selesai | 17 Desember 2025 |
| 3   | Export PDf/Excel          | Laporan dapat diekspor dengan benar          | ✅ Selesai | 17 Desember 2025 |
| 4   | Workflow Status Transaksi | Status transaksi terintegrasi penuh          | ✅ Selesai | 17 Desember 2025 |
| 5   | Dokumentasi & README      | Dokumentasi lengkap dan siap dipresentasikan | ✅ Selesai | 17 Desember 2025 |

---
# Midtrans

## Deskripsi Midtrans

Midtrans adalah layanan payment gateway di Indonesia yang membantu bisnis menerima pembayaran online lewat berbagai metode dalam satu integrasi, seperti transfer bank, virtual account, kartu kredit dan debit, e-wallet, serta pembayaran di minimarket. Kamu bisa menghubungkan Midtrans ke website atau aplikasi lewat API dan dashboard untuk membuat invoice, memproses pembayaran, memantau status transaksi secara real time, dan mengelola fitur seperti notifikasi webhook, pembayaran otomatis, hingga laporan transaksi. Midtrans juga menyediakan fitur keamanan dan deteksi risiko, sehingga alur pembayaran lebih rapi dan mudah dikelola dari sisi sistem.

## Lingkup Pendukung

1. Website Utama: https://midtrans.com/
2. Halaman Dashboard Production: https://dashboard.midtrans.com/l
3. Halaman Dashboard Sandbox: https://dashboard.sandbox.midtrans.com/
4. Github: https://github.com/Midtrans/midtrans-php

## Alur Kerja Midtrans secara Umum

Alur Midtrans di Cafelora itu sederhana dan rapi. Pelanggan cukup melihat daftar menu di website untuk menentukan pilihan makanan dan minuman, termasuk melihat detail menu agar pesanan lebih jelas. Setelah pelanggan menyampaikan pilihannya, kasir atau admin memasukkan pesanan ke sistem POS, memilih varian, menambahkan topping atau modifier bila diperlukan, lalu sistem otomatis menghitung total belanja. Saat proses checkout, kasir atau admin menekan tombol bayar, kemudian Midtrans menampilkan pilihan metode pembayaran seperti QRIS, e-wallet, transfer bank, kartu, atau minimarket. Pelanggan memilih metode yang paling nyaman, lalu melakukan pembayaran sesuai instruksi yang muncul di layar. Begitu pembayaran berhasil, Midtrans langsung mengirim notifikasi ke sistem Cafelora sehingga status transaksi otomatis berubah menjadi “paid” tanpa input manual. Setelah itu kasir tinggal menyiapkan pesanan, mencetak struk, menghitung kembalian jika ada pembayaran tunai di luar sistem, dan memastikan pesanan berjalan sesuai alur pelayanan. Di sisi admin, semua transaksi tercatat otomatis sehingga mudah dipantau melalui dashboard, bisa di filter berdasarkan tanggal dan status, terlihat pada grafik penjualan, dan bisa diekspor menjadi laporan PDF atau Excel. Jika pembayaran gagal, tertunda, atau dibatalkan, status transaksi ikut terupdate sehingga transaksi tidak dianggap selesai dan data tetap konsisten.

## Alur Kerja Midtrans secara Teknis

### 1. Setup Midtrans

1. Buat akun Midtrans dan pilih environment Sandbox atau Production.
2. Ambil Server Key dan Client Key.
3. Simpan key di env aplikasi, contoh MIDTRANS_SERVER_KEY, MIDTRANS_CLIENT_KEY, MIDTRANS_IS_PRODUCTION.
4. Set konfigurasi: isProduction, isSanitized, is3ds (untuk kartu).

---
### 2. Desain Data Transaksi di Database

1. Tabel transaksi minimal punya: invoice/order_id, gross_amount, status, payment_type, snap_token, midtrans_transaction_id, paid_at.
2. Simpan detail item: menu, varian, topping, qty, price, subtotal.
3. Status internal yang umum: draft, pending, paid, failed, expired, cancelled, refunded.

---
### 3. Flow Pembuatan Order dari POS

1. Kasir/admin buat order di POS.
2. Backend hitung ulang total (jangan percaya total dari frontend).
3. Backend generate order_id unik (misal INV-20251222202546-GCC1).
4. Simpan transaksi ke DB dengan status pending atau unpaid.

---
### 4. Request ke Midtrans untuk Generate Pembayaran

1. Backend panggil API Midtrans Snap untuk create transaction.

2. Kirim payload:

a. transaction_details: order_id, gross_amount

b. item_details: list item (menu, topping) dengan price dan qty

c. customer_details: nama, email, hp (bisa data kasir jika offline)

d. callbacks atau expiry jika dipakai

3. Midtrans balikin snap_token dan redirect_url.

4. Backend simpan snap_token dan redirect_url ke DB.

---
### 5. Menampilkan UI Pembayaran

1. Frontend POS load Snap.js pakai clientKey.

2. Saat klik “Bayar”, frontend panggil endpoint backend untuk ambil snap_token.

3. Frontend menjalankan snap.pay(snapToken, callbacks...) untuk munculin popup pembayaran.

4. Callback frontend:

onSuccess, onPending, onError, onClose

5. Catatan: callback frontend hanya untuk UX. Sumber kebenaran tetap webhook.

---
### 6. Notifikasi Status via Webhook

1. Midtrans kirim HTTP POST ke endpoint webhook kamu, contoh:

POST /api/midtrans/notify

2. Backend verifikasi:

a. validasi signature key (Midtrans signature)

b. cocokkan order_id dengan transaksi di DB

3. Backend mapping status Midtrans:

a. transaction_status=settlement atau capture -> set paid

b. pending -> set pending

c. deny, cancel, expire -> set sesuai

d. refund / chargeback -> set refunded / chargeback

4. Update DB secara idempotent:

a. kalau status sudah paid, jangan overwrite jadi pending

b. simpan raw payload untuk audit

5. Trigger proses lanjutan:

a. set paid_at

b. kurangi stok

c. generate nomor struk dan data print

---
### 7. Status Transaksi Real Time untuk POS

1. POS polling endpoint transaksi atau pakai WebSocket.
2. Kasir lihat status berubah otomatis jadi paid.
3. Workflow lanjut: paid -> processing -> done (sesuai alur Cafelora).

---
### 8. Rekonsiliasi dan Fallback

1. Jika webhook telat, backend bisa cek status via API Midtrans (Status API) berdasarkan order_id.

2. Jalankan cron job untuk transaksi pending yang lama:

a. query status ke Midtrans

b. update DB jika sudah settle atau expire

---
### 9. Keamanan dan Best Practice

1. Server Key hanya di backend. Jangan taruh di frontend.

2. Semua total dihitung di backend.

3. Endpoint webhook harus:

a. tanpa auth user biasa

b. diproteksi signature verification

c. rate limit dan log request

4. Pastikan order_id unik dan tidak dipakai ulang.

---
# Hasil Tampilan Aplikasi Cafelora

## Halaman Admin (Sabtu, 29 November 2025)

### 1. Halaman Dashboard Admin

<img width="1178" height="660" alt="DashboardAdmin" src="https://github.com/user-attachments/assets/2c824ddd-6163-44d7-8701-e77328341ca7" />

### 2. Halaman Users

<img width="1179" height="658" alt="UsersAdmin" src="https://github.com/user-attachments/assets/e873ec37-ca7e-4f48-83cb-b488b8dadae0" />

### 3. Halaman Categories

<img width="1185" height="668" alt="CategoriesAdmin" src="https://github.com/user-attachments/assets/b5ff2891-4a69-4205-b710-41cedda81c55" />

### 4. Halaman Menus

<img width="1183" height="660" alt="MenusAdmin" src="https://github.com/user-attachments/assets/388a1209-dfbf-4e7c-8c7c-4502aa3c7f64" />

### 5. Halaman Toppings

<img width="1191" height="668" alt="ToppingsAdmin" src="https://github.com/user-attachments/assets/c59e2670-e346-418e-b7cb-b35471b6e35e" />

### 6. Halaman Variants

<img width="1195" height="669" alt="VariantsAdmin" src="https://github.com/user-attachments/assets/8f960168-41e3-45e7-b5fb-f7382a83ba85" />

### 7. Halaman Admin Login (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/39ceb43d-e265-43f4-9a74-515b1545eef4" />

### 8. Halaman Dashboard Admin (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/230ab124-7553-43de-8b6f-cd7cc618c462" />

### 9. Halaman Users (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/b95ac81f-0dcb-4fe9-a058-c042f7f6766d" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/0b9cc913-f946-402e-8686-e59a47ab1eea" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/93551063-8ac2-4aff-8261-cd055c345fd1" />

### 10. Halaman Categories (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/42581c9c-171b-40d0-9418-090ccadde470" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/53d58490-bc4c-472d-adca-eccb5e1efaa9" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/cfb20564-49dc-451c-a9eb-33058792b83b" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/d00fdf87-aeb8-4475-9b54-cfd9f22b7b00" />

### 11. Halaman Menus (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/991c25ba-3864-4686-8114-a481ccaa5730" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/f73bd51a-57b2-4744-a610-8af84a168eb3" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/ff0434d1-8362-42eb-bb20-0cb8bc68a19a" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/385f0cba-413b-4be1-96d6-bc1d188ddebd" />

### 12. Halaman Toppings (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/b4535159-3e18-405f-acae-09e5f0fc5879" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/170fa002-0e17-4c3d-81be-b14d0f26f1f6" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/d12670a6-dbde-4c61-a68f-327bfc0ad5ae" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/ad47c425-550c-454d-9e06-323228878696" />

### 13. Halaman Variants (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/0e6af486-6b41-4939-9eed-0c184a7ce955" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/3e4f88a8-5d7f-4330-b491-58f87ab2d01b" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/61431e9f-1d87-40ef-9e03-d71096a65bbc" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/443e748e-36af-4e7d-b873-151ca66fa5e0" />

---
## Halaman Staf (Sabtu, 29 November 2025)

### 1. Halaman Dashboard Staf

<img width="1195" height="671" alt="DashboardStaf" src="https://github.com/user-attachments/assets/3268bdb1-0eac-4d35-a93a-577e60f5d845" />

### 2. Halaman Categories

<img width="1182" height="664" alt="CategoriesStaf" src="https://github.com/user-attachments/assets/ce82d8d1-96b8-40f5-8b0c-844bcdb45311" />

### 3. Halaman Menus

<img width="1193" height="668" alt="MenusStaf" src="https://github.com/user-attachments/assets/26f5956b-0b83-4423-a778-666502c1f6a6" />

### 4. Halaman Toppings

<img width="1193" height="666" alt="ToppingsStaf" src="https://github.com/user-attachments/assets/423844cf-556a-4506-95b5-bee5df5c8c0a" />

### 5. Halaman Variants

<img width="1194" height="669" alt="VariantsStaf" src="https://github.com/user-attachments/assets/8d8c4e89-f46c-4007-88c5-c1f831f2b6a8" />

### 6. Halaman Staf Login (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/39ceb43d-e265-43f4-9a74-515b1545eef4" />

### 7. Halaman Dashboard Staf (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/7f65f93d-c0d8-4c4f-a69f-0560bb0ea9ad" />

### 8. Halaman Categories (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/1df85c4d-927b-4508-ba12-69552d0bce3d" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/6dcbe68c-80de-4710-83f4-376931972d75" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/39b42851-66ab-4812-a9a4-af4ea16590ae" />

### 9. Halaman Menus (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/705710f3-78e4-4f1b-bb2f-ff591c95dc31" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/b693858f-f241-455b-b66f-cf5b82030f3f" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/3308f51a-7a17-4a4c-83b6-7a09772f43d7" />

### 10. Halaman Toppings (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/27159a2e-a3c7-4aa6-9173-dc2ee3ccd619" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/fba9a797-f921-4f10-89ef-2a919f137efc" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/336f09ea-deab-4839-bf56-6ab35f9c8bdc" />

### 11. Halaman Variants (Senin, 22 Desember 2025)

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/e7b05351-f0a9-43cc-8225-c7031a0c05f4" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/351c1170-ba8f-4592-8d57-b4cbaa641dd6" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/ddb321b2-c936-4ca8-9954-6a5d93c398d3" />

---
## Halaman Frontend Menu

### 1. Minggu, 30 November 2025

<img width="504" height="285" alt="FrontendMenu" src="https://github.com/user-attachments/assets/b342da7b-8046-47f3-99bc-3aec5a5e26a3" />

### 2. Sabtu, 6 Desember 2025

<img width="601" height="339" alt="FrontendMenu2" src="https://github.com/user-attachments/assets/5407770b-344e-4948-acf9-f05829e0a6bc" />

### 3. Senin, 8 Desember 2025

<img width="601" height="339" alt="FrontendMenu3" src="https://github.com/user-attachments/assets/045a6530-1f13-480b-a795-46c2a2d241f8" />

### 4. Sabtu, 13 Desember 2025

<img width="601" height="339" alt="FrontendMenu4" src="https://github.com/user-attachments/assets/27900b88-bbcd-4f7d-92c6-ee447e5a249d" />

<img width="601" height="339" alt="FrontendMenu5" src="https://github.com/user-attachments/assets/ad703878-2a74-45cb-8bbf-e1a1678ef3a1" />

### 5. Senin, 22 Desember 2025

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/add47c86-98af-413d-b6b5-4f1fbbd78db1" />

---
## Halaman POS dan Transaksi

### 1. Halaman POS Kasir

#### 1. Rabu, 10 Desember 2025

<img width="602" height="376" alt="POSKasir1" src="https://github.com/user-attachments/assets/ab126370-11de-407c-a475-c5cba12b2e48" />

#### 2. Jum'at, 12 Desember 2025

<img width="602" height="376" alt="POSKasir2" src="https://github.com/user-attachments/assets/77e39087-cf88-446c-94b5-03babb78d38a" />

<img width="602" height="376" alt="POSKasir3" src="https://github.com/user-attachments/assets/53dd2d12-700b-40ee-af9b-e650b6c05149" />

<img width="602" height="376" alt="KeranjangBelanja" src="https://github.com/user-attachments/assets/cd568563-1145-4741-8277-4a810c3cafce" />

#### 3. Sabtu, 13 Desember 2025

<img width="601" height="376" alt="POSTerbaru" src="https://github.com/user-attachments/assets/3c445698-9b95-4a30-9c9b-e5725dc578a1" />

<img width="601" height="376" alt="TransaksiBerhasil" src="https://github.com/user-attachments/assets/e68fdd03-c3b5-47ad-9950-a6f15484c298" />

#### 4. Senin, 22 Desember 2025

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/9820f87e-d994-4ebf-82ac-67282b435548" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/3b21d4d8-d211-4d26-8665-8d12df509f13" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/9f2925d9-f49d-4413-b6a4-642bbd3de5ba" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/e11b3e6e-5d46-4954-9af0-c1e0defa4170" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/e834b95c-479d-4555-bd74-4ba9571fef44" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/f5f1b7ad-f00f-4d0a-9ebc-d3898ca42939" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/8c3cd5ce-8f82-4b7c-a205-f7a1a1918fa6" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/5d77cad8-9be1-4e33-b6dd-1afa454c7a03" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/0872256a-0b80-420c-bf3b-5df542a836ca" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/ec2337bb-9182-4068-9be9-9d51a8e51403" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/92f94237-0e4f-439c-b6fe-43cfbf566641" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/31e02e97-2190-44c8-b95a-8d70c7fda880" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/9543ccf5-e890-4bc7-8731-8e5a5bf49d5e" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/c77e2c37-3eed-4eb2-9499-28635b58bb49" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/eed543b6-4943-4b0a-8d2c-efeaae282b81" />

---
### 2. Halaman Transactions 

#### 1. Rabu, 10 Desember 2025

<img width="602" height="376" alt="Transactions" src="https://github.com/user-attachments/assets/5a0c85a9-c85b-4d91-a676-ed7d37f29308" />

#### 2. Sabtu, 13 Desember 2025

<img width="601" height="376" alt="Transactions2" src="https://github.com/user-attachments/assets/3c1f8fdd-a1e0-4f8f-880d-a7adf27999cb" />

#### 3. Senin, 22 Desember 2025

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/e0c77264-2d23-4f52-93a4-97f45fca245c" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/4e11904b-e8d9-4a6a-9054-70f10da67776" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/f6134dc7-dba3-442e-aa84-d22813c6e9c7" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/8290f872-8484-4894-a7c4-abbd02b8da77" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/0841cd32-7d02-4faa-a2ad-c434ca90802c" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/eca6d02a-5334-412f-80d7-c4f7777fde5f" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/bbf58056-5c08-49a9-bc06-398ae0e81c68" />
<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/bd8ec9d7-4e66-48c2-8880-f9cdff1b5606" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/58ee1a85-dea8-4188-807b-9afd351fb052" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/da4a96cd-609c-424a-9553-f1e90bae0024" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/f117939a-3cd6-49da-87d5-1af19afc8ed2" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/03235692-12c7-48a3-a8d4-5e988e3f84ba" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/a346c130-65aa-494c-9b7c-86225042734e" />

<img width="1470" height="924" alt="Image" src="https://github.com/user-attachments/assets/7a1821f4-be71-43e9-bd35-baa297267fa0" />

---
### 3. Halaman Detail Transactions (Rabu, 10 Desember 2025)

<img width="602" height="376" alt="DetailTransactions" src="https://github.com/user-attachments/assets/d2e0c157-8997-4db0-8cdf-0080a72fb52c" />

---
