# PRAKTIKUM 11: PROGRES TUBES 1 - APLIKASI CAFELORA

# 📃 Identitas Diri

- **Kelompok**         : Kelompok 1
- **Anggota Kelompok** : 
  1. Arya Wicaksana Putra (4520210092)
  2. Aditya Nur Lintang (4523210003)
  3. Alip Khoeril Akbar (4523210009)
  4. Revalina Adelia (4523210091)
  5. Chaerul Cahyadi (4523210120)
- **Mata Kuliah**      : Pemrograman Berbasis Web (A)
- **Dosen Pengampu**   : Adi Wahyu Pribadi, S.Si., M.Kom.
- **Topik Proyek**     : Cafe

---
# 📋 Deskripsi Cafelora

**Cafelora** merupakan konsep aplikasi yang dikembangkan untuk mendukung operasional sebuah cafe modern dengan fokus pada kemudahan pemesanan, kejelasan informasi menu, dan proses transaksi yang efisien. Ide awal Cafelora muncul dari kebutuhan untuk menyediakan layanan cepat dan nyaman bagi pelanggan yang ingin menikmati makanan dan minuman berkualitas. Seluruh menu diolah menggunakan bahan segar setiap hari, dan sistem pemesanan dirancang agar mudah dipahami baik oleh pelanggan maupun kasir. Pelanggan dapat melihat menu dengan lebih informatif, sementara kasir dapat memproses transaksi secara ringkas dan terstruktur. Pendekatan ini membuat alur pelayanan menjadi rapi, meminimalkan kesalahan, serta meningkatkan kepuasan pelanggan. Seiring berjalannya waktu, Cafelora terus berkembang berkat kombinasi rasa yang konsisten, harga yang bersaing, dan pengalaman pemesanan yang praktis. Aplikasi ini hadir sebagai solusi pendukung digital untuk meningkatkan kualitas layanan dan efisiensi operasional cafe.

---
# 🚀 Fitur Aplikasi Cafelora

## Fitur Admin

1. CRUD menu, kategori, varian, dan topping.
2. Upload dan manajemen gambar menu.
3. Sistem manajemen stok otomatis.
4. Workflow status transaksi dari awal hingga selesai.
5. Pengelolaan user.
6. Dashboard pendapatan serta grafik penjualan harian dan bulanan.
7. Export laporan transaksi ke format PDF/Excel **(opsional)**.

## Fitur Kasir/Staff (POS)

1. Input pesanan menggunakan komponen Repeater.
2. Penambahan topping dan modifier secara dinamis.
3. Perhitungan total harga secara otomatis.
4. Fitur input uang bayar dan kalkulasi kembalian.
5. Cetak struk transaksi dalam bentuk PDF/HTML.
6. Akses halaman yang dibatasi sesuai role (khusus transaksi).

## Fitur Pelanggan (Frontend)

1. Melihat daftar menu makanan dan minuman.
2. Filter menu berdasarkan kategori dan varian.
3. Tampilan menu berbentuk kartu untuk memudahkan pemilihan.
4. Halaman detail menu untuk memberikan informasi lebih lengkap.

## Fitur Tambahan (Opsional)

1. Integrasi payment gateway (Midtrans atau Xendit).
2. Filter laporan berdasarkan tanggal dan status transaksi.
3. Fitur chart penjualan untuk monitoring transaksi 7 hari terakhir.

---
# 👥 Pembagian Jobdesk 

## 1. Chaerul Cahyadi (Ketua)

1. Menyusun struktur proyek secara keseluruhan.
2. Mengintegrasikan fitur transaksi dan perhitungan harga.
3. Menangani dashboard serta visualisasi data laporan.
4. Melakukan final review terhadap seluruh fitur.

## 2. Arya Wicaksana Putra

1. Mendesain ERD serta relasi antar tabel _database_.
2. Membuat CRUD data master seperti kategori dan topping.
3. Mengimplementasikan validasi _form_ dan upload gambar menu.

## 3. Aditya Nur Lintang

1. Melakukan setup awal Laravel dan Filament.
2. Mengimplementasikan role, Policy, dan access control.
3. Mengelola user Admin dan Staff.

## 4. Alip Khoeril Akbar

1. Mendesain UI untuk tampilan menu pelanggan (Frontend).
2. Mengatur layout grid pada halaman menu.
3. Membuat komponen kartu menu dan fitur filter.

## 5. Muhammad Fauzan

1. Mengembangkan fitur POS kasir.
2. Mengimplementasikan Repeater item transaksi dan kalkulasi otomatis.
3. Membuat fitur cetak struk dalam format HTML-PDF.

## 6. Revalina Adelia 

1. Mengembangkan fitur laporan dan export PDF/Excel.
2. Mengatur workflow status transaksi.
3. Meyusun dokumentasi teknis proyek dan README.

---
## 🛠 Teknologi yang Digunakan

Aplikasi ini dibangun menggunakan beberapa teknologi utama yang mendukung _backend_, _frontend_, dan _database_, sehingga aplikasi dapat berjalan dengan baik dan terstruktur. Berikut teknologi yang digunakan:

| Teknologi             | Versi  | Keterangan                                                                       |
|-----------------------|--------|----------------------------------------------------------------------------------|
| **PHP**               | 8.4.13 | Bahasa pemrograman server-side yang menjalankan logika aplikasi                  |
| **Laravel Framework** | ^12.0  | Framework PHP berbasis MVC untuk mengatur _routing_, controller, model, dan view |
| **Composer**          | Latest | Dependency manager untuk mengelola library dan package PHP                       |
| **NPM**               | Latest | Package manager untuk mengelola library dan modul JavaScript                     |
| **Vite**              | Latest | Build tool untuk mengompilasi dan mengelola file _frontend_ (CSS, JS)            |
| **MySQL/PostgreSQL**  | Latest | _Database_ relasional untuk menyimpan semua data aplikasi                        |

---
## ⚙️ Persyaratan Sistem

Sebelum menjalankan aplikasi, pastikan perangkat sudah memenuhi persyaratan berikut:

1. **PHP >= 8.2** : Versi PHP yang kompatibel dengan Laravel 12.
2. **Composer** : Untuk mengelola _dependency_ PHP.
3. **Node.js & NPM** : Untuk menjalankan script _frontend_ dan _build assets_.
4. **MySQL atau PostgreSQL** : _Database_ untuk menyimpan data aplikasi.
5. **Web Server** : Seperti Apache atau Nginx, atau bisa menggunakan Laravel _built-in server_.

Untuk pengguna **Windows**, disarankan menggunakan salah satu dari:
1. **Laragon** : Sudah termasuk PHP, MySQL, dan Apache, memudahkan setup lingkungan _development_.
2. **XAMPP** : Paket server populer untuk PHP dan MySQL.
3. **Herd** : Alternatif ringan untuk _development_ lokal.

---
## 🛠️ Langkah Instalasi

### 1. Clone atau Download Repository

```bash
# Clone repository (jika menggunakan git)
https://github.com/xnoname2003/cafelora.git
cd cafelora
```

Langkah ini digunakan untuk mengambil kode sumber aplikasi dari _repository_ Git. Jika menggunakan Git, perintah `git clone` akan menyalin seluruh project ke komputer kita, kemudian `cd cafelora` masuk ke folder proyek agar siap untuk langkah selanjutnya.

### 2. Install Dependencies PHP

```bash
composer install
```

Perintah ini digunakan untuk menginstal **library dan package PHP** yang dibutuhkan oleh Laravel. Semua dependensi sudah didefinisikan di file `composer.json`, sehingga aplikasi bisa berjalan dengan baik.

### 3. Install Dependencies JavaScript

```bash
npm install
```

Laravel menggunakan JavaScript untuk _frontend_ (misal interaksi UI atau _build assets_). Perintah ini akan menginstal semua _package_ JavaScript yang diperlukan sesuai definisi di `package.json`.

### 4. Konfigurasi Environment

```bash
# Copy file .env.example menjadi .env
copy .env.example .env

# Generate application key
php artisan key:generate
```

1. `copy .env.example .env` : Membuat salinan file konfigurasi _environment_ agar bisa diubah sesuai pengaturan lokal.
2. `php artisan key:generate` : Membuat **_aplication key_** yang digunakan Laravel untuk keamanan, misalnya enkripsi session dan data sensitif.
   
### 5. Konfigurasi Database

Edit file `.env` untuk menyesuaikan pengaturan _database_:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=cafelora
DB_USERNAME=root
DB_PASSWORD=
```

Di sini kita menentukan tipe _database_ (MySQL), alamat server _database_, nama _database_, _username_, dan _password_. Ini agar Laravel bisa terhubung ke _database_ lokal.

### 6. Jalankan Migration & Seeder

```bash
# Membuat tabel-tabel di database
php artisan migrate

# (Optional) Generate data dummy untuk testing
php artisan db:seed
```

1. `php artisan migrate` : Membuat semua **tabel di _database_** sesuai file migration.
2. `php artisan db:seed` : Opsional, untuk mengisi _database_ dengan **data _dummy_** agar bisa langsung dicoba tanpa menambahkan data manual.
   
### 7. Build Assets Frontend

```bash
# Untuk development (dengan hot reload)
npm run dev

# Untuk production
npm run build
```

1. `npm run dev` : Membangun aset _frontend_ untuk **_development_**, termasuk _hot reload_ agar perubahan langsung terlihat di browser.
2. `npm run build` : Membangun aset _frontend_ untuk **_production_**, biasanya lebih optimal dan sudah terminify.
   
### 8. Jalankan Aplikasi

```bash
# Menggunakan Laravel built-in server
php artisan serve
```

Perintah ini menjalankan **Laravel built-in server** sehingga aplikasi bisa diakses melalui browser. Default URL:`http://127.0.0.1:8000`

---
## 💾 Database Aplikasi Cafelora

### Entity Relationship Diagram

_Entity Relationship Diagram_ (ERD) ini menggambarkan struktur _database_ dari sistem manajemen Cafelora, yang mencakup pengguna, menu, kategori, varian, topping, transaksi, hingga detail item pesanan.

1. User adalah entitas inti yang mewakili admin, staff kasir, dan customer. Akses kontrol diatur menggunakan role dan permission.
2. Menu terbagi menjadi kategori seperti makanan dan minuman. Menu dapat memiliki banyak varian serta banyak topping.
3. Transaksi dicatat ketika kasir membuat pesanan. Setiap transaksi memiliki banyak item pesanan. Setiap item dapat memiliki topping tambahan.
4. Varian dan topping membantu menyesuaikan harga akhir berdasarkan pilihan pelanggan.
5. Relasi _Many-to-Many_ digunakan pada menu ↔ varian, menu ↔ topping, user ↔ role, serta role ↔ permission.
6. Transaksi berjalan sesuai alur operasional cafe seperti pemesanan, perhitungan total, pembayaran, hingga pencetakan struk.

<img width="1479" height="1028" alt="Image" src="https://github.com/user-attachments/assets/61072427-f297-4a3a-8c9e-2d04573c1559" />

---
### Penjelasan Relasi antar Tabel

| No | Entitas 1                  | Entitas 2                  | Tipe Relasi    | Penjelasan                                                                |
|----|----------------------------|----------------------------|----------------|---------------------------------------------------------------------------|
| 1  | users                      | roles                      | Many-to-Many   | Satu user dapat memiliki banyak role dan sebaliknya.                      |
| 2  | roles                      | permissions                | Many-to-Many   | Role bisa memiliki banyak permission.                                     |
| 3  | users                      | permissions                | Many-to-Many   | User bisa diberi permission langsung.                                     |
| 4  | categories                 | menus                      | One-to-Many    | Satu kategori memiliki banyak menu.                                       |
| 5  | menus                      | variants                   | Many-to-Many   | Satu menu bisa memiliki banyak varian.                                    |
| 6  | menus                      | toppings                   | Many-to-Many   | Satu menu bisa memiliki banyak topping.                                   |
| 7  | users                      | transactions               | One-to-Many    | Satu user (kasir) dapat membuat banyak transaksi.                         |
| 8  | transactions               | transaction_items          | One-to-Many    | Satu transaksi terdiri dari banyak item pesanan.                          |
| 9  | menus                      | transaction_items          | Many-to-One    | Satu item pesanan merujuk ke satu menu.                                   |
| 10 | variants                   | transaction_items          | Many-to-One    | Item pesanan hanya memakai satu varian.                                   |
| 11 | transaction_items          | transaction_item_toppings  | One-to-Many    | Setiap item pesanan dapat memiliki beberapa topping.                      |
| 12 | toppings                   | transaction_item_toppings  | Many-to-One    | Topping digunakan sebagai tambahan pada item tertentu.                    |

---
### Tabel: users (Tabel Master)

Berfungsi untuk menyimpan data user (Admin, Staff).  
**Relasi:**  
- One-to-Many → transactions  
- Many-to-Many → roles  
- Many-to-Many → permissions  

| Kolom              | Tipe Data      | Fungsi                          |
|--------------------|----------------|---------------------------------|
| id                 | bigint         | Primary key user                |
| name               | varchar        | Nama user                       |
| email              | varchar        | Email login                     |
| password           | varchar        | Password bcrypt                 |
| email_verified_at  | datetime       | Verifikasi email                |
| remember_token     | varchar        | Token login                     |
| created_at         | datetime       | Waktu dibuat                    |
| updated_at         | datetime       | Waktu update                    |

### Tabel: roles (Tabel Master)

Berfungsi untuk menyimpan daftar peran.  
**Relasi:**  
- Many-to-Many → permissions  
- Many-to-Many → users  

| Kolom      | Tipe Data | Fungsi                     |
|------------|-----------|----------------------------|
| id         | bigint    | Primary key                |
| name       | varchar   | Nama role                  |
| guard_name | varchar   | Guard spatie               |
| created_at | datetime  | Waktu dibuat               |
| updated_at | datetime  | Waktu update               |

### Tabel: permissions (Tabel Master)

Berfungsi untuk menyimpan daftar permission.  
**Relasi:**  
- Many-to-Many → roles  
- Many-to-Many → users  

| Kolom      | Tipe Data | Fungsi                     |
|------------|-----------|----------------------------|
| id         | bigint    | Primary key                |
| name       | varchar   | Nama permission            |
| guard_name | varchar   | Guard permission           |
| created_at | datetime  | Waktu dibuat               |
| updated_at | datetime  | Waktu update               |

### Tabel: role_has_permissions (Tabel Relasi Many-to-Many)

Menghubungkan role ↔ permission.  
**Relasi:**  
- Many-to-Many → roles  
- Many-to-Many → permissions  

| Kolom         | Tipe Data | Fungsi                 |
|---------------|-----------|------------------------|
| permission_id | bigint    | FK permissions.id      |
| role_id       | bigint    | FK roles.id            |

### Tabel: model_has_roles (Tabel Relasi Many-to-Many)

Assign role ke user.  
**Relasi:**  
- Many-to-Many → users  
- Many-to-Many → roles  

| Kolom      | Tipe Data | Fungsi                  |
|------------|-----------|-------------------------|
| role_id    | bigint    | FK roles.id             |
| model_type | varchar   | Model type (User)       |
| model_id   | bigint    | FK users.id             |

### Tabel: model_has_permissions (Tabel Relasi Many-to-Many)

Memberi permission langsung ke user.  
**Relasi:**  
- Many-to-Many → users  
- Many-to-Many → permissions  

| Kolom         | Tipe Data | Fungsi                    |
|---------------|-----------|---------------------------|
| permission_id | bigint    | FK permissions.id         |
| model_type    | varchar   | Model type (User)         |
| model_id      | bigint    | FK users.id               |

---
## Menu System

### Tabel: categories (Tabel Master)

Berfungsi untuk menyimpan kategori menu.  
**Relasi:**  
- One-to-Many → menus  

| Kolom      | Tipe Data | Fungsi              |
|------------|-----------|---------------------|
| id         | int       | Primary key         |
| name       | varchar   | Nama kategori       |
| created_at | datetime  | Waktu dibuat        |
| updated_at | datetime  | Waktu update        |

### Tabel: variants (Tabel Master)

Berfungsi untuk menyimpan varian menu.  
**Relasi:**  
- Many-to-Many → menus  

| Kolom            | Tipe Data | Fungsi                          |
|------------------|-----------|---------------------------------|
| id               | int       | Primary key                     |
| name             | varchar   | Nama varian                     |
| price_adjustment | int       | Tambahan harga                  |
| created_at       | datetime  | Waktu dibuat                    |

### Tabel: toppings (Tabel Master)

Berfungsi untuk menyimpan topping menu.  
**Relasi:**  
- Many-to-Many → menus  
- Many-to-Many → transaction_items  

| Kolom      | Tipe Data | Fungsi                |
|------------|-----------|-----------------------|
| id         | int       | Primary key           |
| name       | varchar   | Nama topping          |
| price      | int       | Harga topping         |
| created_at | datetime  | Waktu dibuat          |
| updated_at | datetime  | Waktu update          |


### Tabel: menus (Tabel Master)

Berfungsi untuk menyimpan menu makanan/minuman.  
**Relasi:**  
- One-to-Many ← categories  
- Many-to-Many → variants  
- Many-to-Many → toppings  
- One-to-Many → transaction_items  

| Kolom       | Tipe Data | Fungsi                         |
|-------------|-----------|--------------------------------|
| id          | int       | Primary key                    |
| category_id | int       | FK kategori                    |
| name        | varchar   | Nama menu                      |
| description | text      | Deskripsi                      |
| base_price  | int       | Harga dasar                    |
| image       | varchar   | Gambar                         |
| stock       | int       | Stok menu                      |
| created_at  | datetime  | Waktu dibuat                   |
| updated_at  | datetime  | Waktu update                   |

### Tabel: menu_variant (Tabel Relasi Many-to-Many)

Relasi menu ↔ varian.  
**Relasi:**  
- Many-to-Many → menus  
- Many-to-Many → variants  

| Kolom     | Tipe Data | Fungsi            |
|-----------|-----------|-------------------|
| id        | int       | Primary key       |
| menu_id   | int       | FK menus.id       |
| variant_id| int       | FK variants.id    |

### Tabel: menu_topping (Tabel Relasi Many-to-Many)

Relasi menu ↔ topping.  
**Relasi:**  
- Many-to-Many → menus  
- Many-to-Many → toppings  

| Kolom     | Tipe Data | Fungsi              |
|-----------|-----------|---------------------|
| id        | int       | Primary key         |
| menu_id   | int       | FK menus.id         |
| topping_id| int       | FK toppings.id      |

---
## Transaction System (POS)

### Tabel: transactions (Tabel Master Transaksi)

Berfungsi untuk menyimpan transaksi kasir.  
**Relasi:**  
- Many-to-One → users (kasir)  
- One-to-Many → transaction_items  

| Kolom         | Tipe Data    | Fungsi                 |
|---------------|--------------|------------------------|
| id            | int          | Primary key            |
| user_id       | bigint       | FK kasir               |
| invoice       | varchar      | Nomor invoice          |
| status        | enum         | pending/paid/completed |
| total         | int          | Total transaksi        |
| paid_amount   | int          | Uang bayar             |
| change_amount | int          | Kembalian              |
| created_at    | datetime     | Waktu dibuat           |
| updated_at    | datetime     | Waktu update           |

### Tabel: transaction_items (Tabel Detail Transaksi)

Berfungsi untuk menyimpan item dalam transaksi.  
**Relasi:**  
- Many-to-One → transactions  
- Many-to-One → menus  
- Many-to-One → variants  
- One-to-Many → transaction_item_toppings  

| Kolom          | Tipe Data | Fungsi                 |
|----------------|-----------|------------------------|
| id             | int       | Primary key            |
| transaction_id | int       | FK transaksi           |
| menu_id        | int       | FK menu                |
| variant_id     | int       | FK varian              |
| quantity       | int       | Jumlah                 |
| price          | int       | Harga satuan           |
| subtotal       | int       | Total harga            |
| created_at     | datetime  | Waktu dibuat           |
| updated_at     | datetime  | Waktu update           |

### Tabel: transaction_item_toppings (Relasi Many-to-Many per Item Transaksi)

Berfungsi untuk menyimpan topping tambahan pada item transaksi.  
**Relasi:**  
- Many-to-One → transaction_items  
- Many-to-One → toppings  

| Kolom                | Tipe Data | Fungsi                |
|----------------------|-----------|-----------------------|
| id                   | int       | Primary key           |
| transaction_item_id  | int       | FK item transaksi     |
| topping_id           | int       | FK topping            |
| price                | int       | Harga topping         |

---
## 📈 Rekap Uji Fungsionalitas & Status Progres Fitur

Bagian ini digunakan untuk mengetahui fitur apa saja yang **sudah selesai dan sudah diuji** serta fitur yang **masih dalam proses pengembangan**. Pengerjaan dimulai pada tanggal **26 November 2025** sampai saat ini.

### 1. Chaerul Cahyadi (Ketua): Struktur Proyek, Integrasi Transaksi, Dashboard, Review Fitur

| No. | Fitur yang Diuji                  | Deskripsi Uji                                                            | Status                                  | Tanggal Mulai     |
|-----|-----------------------------------|--------------------------------------------------------------------------|-----------------------------------------|-------------------|
| 1   | Struktur Proyek & Routing         | Mengecek konsistensi struktur folder, routing utama, dan manajemen modul | ✅ Selesai & Stabil                     | 26 November 2025  |
| 2   | Integrasi Logika Transaksi (Awal) | Memastikan relasi model transaksi & item berjalan awalnya                | 🔄 Dalam Progres (Bergantung POS Kasir) | 2-8 November 2025 |
| 3   | Dashboard Admin                   | Visualisasi dasar sudah tampil, grafik belum 100% data real-time         | 🔄 Dalam Progres                        | 2-8 November 2025 |
| 4   | Review & Validasi Fitur           | Pengecekan keseluruhan fitur anggota lain                                | 🔄 Berjalan Bertahap                    | 26 November 2025  |

### 2. Arya Wicaksana Putra: ERD, CRUD Master Data, Validasi Form, Upload Gambar

| No. | Fitur yang Diuji   | Deskripsi Uji                                                  | Status                       | Tanggal Mulai    |
|-----|--------------------|----------------------------------------------------------------|------------------------------|------------------|
| 1   | Desain ERD         | ERD diverifikasi dan konsisten dengan model Laravel            | ✅ Selesai                   | 26 November 2025 |
| 2   | CRUD Kategori      | Tambah, edit, hapus, dan list kategori berjalan baik           | ✅ Selesai & Berjalan Normal | 26 November 2025 |
| 3   | CRUD Topping       | Form & relasi topping berhasil disimpan                        | ✅ Selesai                   | 26 November 2025 |
| 4   | Validasi Form      | Field wajib terisi, format harga, dan input gambar tervalidasi | ✅ Selesai                   | 26 November 2025 |
| 5   | Upload Gambar Menu | Mengunggah gambar ke storage dan menampilkannya di card menu   | ✅ Selesai                   | 26 November 2025 |

### 3. Aditya Nur Lintang: Setup Laravel, Filament, Role, Policy, User Management

| No. | Fitur yang Diuji                | Deskripsi Uji                                            | Status                 | Tanggal Mulai    |
|-----|---------------------------------|----------------------------------------------------------|------------------------|------------------|
| 1   | Setup Laravel & Filament        | Proyek berhasil berjalan dan panel admin siap digunakan  | ✅ Selesai             | 26 November 2025 |
| 2   | Implementasi Role (Admin/Staff) | Pengujian akses halaman sesuai role                      | ✅ Selesai & Berfungsi | 26 November 2025 |
| 3   | Policy & Permission             | Staff dibatasi untuk akses tertentu (tanpa delete)       | ✅ Selesai             | 26 November 2025 |
| 4   | Manajemen User                  | CRUD user admin/staff berjalan optimal                   | ✅ Selesai             | 26 November 2025 |

### 4. Alip Khoeril Akbar: Frontend Pelanggan – Tampilan Menu & Filter

| No. | Fitur yang Diuji    | Deskripsi Uji                      | Status     | Tanggal Mulai    |
|-----|---------------------|------------------------------------|------------|------------------|
| 1   | Tampilan Grid Menu  | Card tampil responsif              | ✅ Selesai | 26 November 2025 |
| 2   | Filter Kategori     | Menu menyesuaikan pilihan kategori | ✅ Selesai | 26 November 2025 |
| 3   | Filter Varian       | Menu berganti sesuai varian        | ✅ Selesai | 26 November 2025 |
| 4   | Komponen Card Menu  | Gambar, nama, harga tampil baik    | ✅ Selesai | 26 November 2025 |
| 5   | Halaman Detail Menu | Informasi menu tampil lengkap      | ✅ Selesai | 26 November 2025 |
| 6   | Responsivitas UI    | Mobile & desktop tampak konsisten  | ✅ Selesai | 26 November 2025 |

### 5. Muhammad Fauzan: POS Kasir – Repeater Item, Perhitungan, Cetak Struk

| No. | Fitur yang Diuji          | Deskripsi Uji                                     | Status                   | Tanggal Mulai     |
|-----|---------------------------|---------------------------------------------------|--------------------------|-------------------|
| 1   | Tampilan Awal POS         | Repeater dasar tampil                             | ✅ UI Dasar Berjalan     | 2-8 November 2025 |
| 2   | Penambahan Item Transaksi | Penambahan baris item berhasil                    | 🟡 Perlu Logika Tambahan | 2-8 November 2025 |
| 3   | Dropdown Menu & Varian    | Dropdown tampil, harga belum sepenuhnya otomatis  | 🔄 Dalam Progres         | 2-8 November 2025 |
| 4   | Kalkulasi Total Otomatis  | Subtotal & total belum final                      | ⏳ Belum Selesai         | 2-8 November 2025 |
| 5   | Input Bayar & Kembalian   | Field muncul, logika backend belum lengkap        | 🔄 Dalam Progres         | 2-8 November 2025 |
| 6   | Cetak Struk HTML/PDF      | Template awal ada, belum final                    | 🔄 Dalam Progres         | 2-8 November 2025 |

### 6. Revalina Adelia: Laporan, Export PDF/Excel, Workflow Transaksi, Dokumentasi

| No. | Fitur yang Diuji           | Deskripsi Uji                                        | Status               | Tanggal Mulai     |
|-----|----------------------------|------------------------------------------------------|----------------------|-------------------|
| 1   | Halaman Laporan            | Tabel laporan tampil                                 | ✅ UI Dasar Berjalan | 2-8 November 2025 |
| 2   | Filter Laporan             | Filter tanggal & status belum terhubung backend      | 🔄 Dalam Progres     | 2-8 November 2025 |
| 3   | Export PDf                 | Tombol tampil, backend belum final                   | 🔄 Dalam Progres     | 2-8 November 2025 |
| 4   | Workflow Status Transaksi  | Status pending → paid → completed belum terintegrasi | ⏳ Belum Selesai     | 2-8 November 2025 |
| 5   | Dokumentasi README         | Struktur sudah tersusun dan sedang diisi             | 🔄 Dalam Progres     | 2-8 November 2025 |

---
## 🗺️ Rencana Pengembangan Berikutnya

Pada tahap pengembangan selanjutnya, fokus utama yang akan dikerjakan adalah:

1. Menyelesaikan logika POS kasir (perhitungan otomatis, kembalian, dan update stok).
2. Mengintegrasikan workflow status transaksi dengan dashboard dan laporan.
3. Mengimplementasikan fitur export laporan ke PDF dan Excel.
4. Menyempurnakan tampilan dashboard dengan grafik penjualan harian dan bulanan.
5. Melakukan pengujian _end-to-end_ dari sudut pandang Admin, Kasir, dan Pelanggan.
   
---
# 📸 Hasil Tampilan

## 1. Halaman Frontend (Pelanggan)

<img width="504" height="285" alt="Frontend Pelanggan" src="https://github.com/user-attachments/assets/73459cf4-dd58-438b-9254-514062b02287" />

## 2. Halaman Admin

### Halaman Dashboard

<img width="453" height="254" alt="Dashboard Admin" src="https://github.com/user-attachments/assets/a9b8eb3a-47cc-431e-9dd2-6ad6e2cf6621" />

### Halaman Users

<img width="451" height="253" alt="Users" src="https://github.com/user-attachments/assets/20f0b504-8937-44fd-b0db-a0628bd296d5" />

### Halaman Categories

<img width="453" height="254" alt="Categories" src="https://github.com/user-attachments/assets/b48dfa33-bb41-47d6-8832-4dae243c95d2" />

### Halaman Menus

<img width="451" height="253" alt="Menus" src="https://github.com/user-attachments/assets/04786e34-bf23-4367-bc8d-f3fde87574b8" />

### Halaman Toppings

<img width="454" height="254" alt="Toppings" src="https://github.com/user-attachments/assets/33a8e1c8-6869-4a15-a02f-3356f53ca9bc" />

### Halaman Variants

<img width="456" height="256" alt="Variants" src="https://github.com/user-attachments/assets/2a598f82-c424-457f-b3e7-1c3a0a638878" />

## 3. Halaman Staff

### Halaman Dashboard

<img width="456" height="258" alt="Dashboard Staff" src="https://github.com/user-attachments/assets/8a5e5100-521a-45dd-a603-2447b991ac19" />

### Halaman Categories

<img width="453" height="254" alt="Categories Staff" src="https://github.com/user-attachments/assets/5df4f0ad-dfc1-4a97-b8dc-aaef87bd8fc3" />

### Halaman Menus

<img width="456" height="258" alt="Menus Staff" src="https://github.com/user-attachments/assets/3d57babe-019e-49b1-b45a-bc61550c947f" />

### Halaman Toppings

<img width="454" height="254" alt="Toppings Staff" src="https://github.com/user-attachments/assets/f485a112-f540-4abd-ac75-2adce2dd5208" />

### Halaman Variants

<img width="454" height="258" alt="Variants Staff" src="https://github.com/user-attachments/assets/a78c759b-000a-4fcc-89a4-ff38ea4f0ade" />
