# PRAKTIKUM 9: BOOKLY - APLIKASI MANAJEMEN BUKU DENGAN LARAVEL DAN FILAMENT 3.x

Kustomisasi dan Pengembangan

# 📃 Identitas Diri

- **Nama**             : Revalina Adelia
- **NPM**              : 4523210091
- **Mata Kuliah**      : Pemrograman Berbasis Web (A)
- **Dosen Pengampu**   : Adi Wahyu Pribadi, S.Si., M.Kom.
- **Tanggal**          : 21 November 2025

---
## 🎯 Tujuan Pembelajaran

Pada praktikum ini mahasiswa mempelajari bagaimana mengembangkan aplikasi manajemen data modern dengan memanfaatkan Laravel sebagai backend dan Filament 3.x sebagai admin panel. Setelah menyelesaikan praktikum ini, mahasiswa diharapkan mampu:
1. Memahami konsep MVC dalam Laravel.
2. Mengimplementasikan CRUD lengkap menggunakan Filament Resource.
3. Membangun relasi database (one-to-many & many-to-many).
4. Membuat form, table, filter, infolist, dan UI yang dinamis.
5. Melakukan upload file (cover buku) dengan storage management.
6. Menggunakan Factory & Seeder untuk data dummy.
7. Mengimplementasikan Role-Based Access Control (RBAC) dengan Policy.
8. Membuat dashboard widget untuk statistik data.

---
## 📰 Deskripsi Aplikasi

Bookly adalah aplikasi manajemen buku berbasis web yang dibangun menggunakan Laravel 12 dan Filament 3.x. Bookly dirancang sebagai aplikasi admin panel untuk mengelola data perpustakaan, mencakup:
1. Data buku
2. Data penulis
3. Data kategori buku
4. Status ketersediaan buku
5. Statistik data dalam bentuk widget

Aplikasi ini mengikuti filosofi Filament yaitu "Make the common things easy, and the hard things possible" yang membuat pengembangan aplikasi menjadi lebih cepat, elegan, dan efisien.

---
## ✨ Fitur Utama

### 1. CRUD Lengkap untuk Buku & Penulis

1. Tambah, ubah, hapus, dan lihat detail buku.
2. Tambah, edit, hapus penulis.
3. Kolom pencarian & sorting otomatis bawaan Filament.

### 2. Upload Cover Buku

1. Upload cover melalui FileUpload Filament.
2. Penyimpanan file pada `storage/app/public/book-covers`.
3. Gambar ditampilkan pada tabel & halaman detail.

### 3. Relasi Database

1. One-to-Many: Author -> Books.
2. Many-to-Many: Books -> Categories.
3. Select input relasional dengan fitur searchable & preload.

### 4. Fitur Filtering & Searching

1. Filter berdasarkan status (available/borrowed).
2. Filter berdasarkan tahun terbit.
3. Filter berdasarkan penulis.
4. Searching otomatis untuk judul & ISBN.

### 5. View Detail Buku (Infolist)

1. Menampilkan detail buku secara rapi menggunakan Infolist.
2. Menampilkan cover, ISBN, penulis, tahun, status, serta timestamp.
   
### 6. Role-Based Access Control (RBAC)

Role ditambahkan pada tabel users:

| Role   | Hak Akses                         |
|--------|-----------------------------------|
| Admin  | Full akses CRUD                   |
| Staff  | Create, Edit, View (tanpa Delete) |
| Viewer | View only                         |

Diimplementasikan melalui BookPolicy & AuthorPolicy

### 7. Dashboard Widgets

Widget yang ditambahkan:
1. Total Books
2. Total Authors
3. Statistik jumlah buku available vs borrowed.
   
### 8. Kategori Buku (Many-to-Many)

1. Model `Category` dibuat.
2. Buku dapat memiliki banyak kategori.
3. Multiple select di form create/edit book.

### 9. Data Dummy menggunakan Factory & Seeder

1. 10 data Author
2. 50 data Book
3. Generator otomatis menggunakan Faker
4. Menjamin ISBN unik dan hubungan author terdistribusi acak.

### 10. Admin Panel Filament

1. Panel `/admin` untuk login.
2. UI modern dan responsif powered by Fiament + Tailwind.
3. Aksi cepat: Create, Eidt, Delete, Bulk Delete, View.

---
## 📂 Struktur Folder Penting

```
manajemen-buku/
├── app
│   ├── Filament
│   │   ├── Resources
│   │   │   ├── AuthorResource
│   │   │   │   ├── Pages
│   │   │   │   │   ├── CreateAuthor.php
│   │   │   │   │   ├── EditAuthor.php
│   │   │   │   │   └── ListAuthors.php
│   │   │   │   └── AuthorResource.php
│   │   │   ├── BookResource
│   │   │   │   ├── Pages
│   │   │   │   │   ├── CreateBook.php
│   │   │   │   │   ├── EditBook.php
│   │   │   │   │   ├── ListBooks.php
│   │   │   │   │   └── ViewBook.php
│   │   │   │   └── BookResource.php
│   │   ├── Widgets
│   │   │   ├── BooksChart.php
│   │   │   └── LibraryStatsWidget.php
│   ├── Http
│   │   └── Controllers
│   ├── Models
│   │   ├── Author.php
│   │   ├── Book.php
│   │   ├── Category.php
│   │   └── User.php
│   ├── Policies
│   │   ├── AuthorPolicy.php
│   │   └── BookPolicy.php
│   └── Providers
│
├── bootstrap
├── config
├── database
│   ├── factories
│   │   ├── AuthorFactory.php
│   │   ├── BookFactory.php
│   │   └── UserFactory.php
│   ├── migrations
│   │   ├── 0001_01_01_000000_create_users_table.php
│   │   ├── 0001_01_01_000001_create_cache_table.php
│   │   ├── 0001_01_01_000002_create_jobs_table.php
│   │   ├── 2025_11_14_023152_create_authors_table.php
│   │   ├── 2025_11_14_023422_create_books_table.php
│   │   ├── 2025_11_20_023259_create_categories_table.php
│   │   └── 2025_11_20_023726_create_book_category_table.php
│   └── seeders
│       ├── CategorySeeder.php
│       └── DatabaseSeeder.php
│
└── .gitignore
```

**Penjelasan:**
1. `app/Models/Author.php`: Model untuk data penulis.
2. `app/Models/Book.php`: Model utama untuk entitas buku di Bookly.
3. `app/Models/Category.php`: Model kategori buku (many-to-many dengan Book).
4. `app/Models/User.php`: Model user aplikasi (admin, staff, viewer).
5. `app/Filament/Resources/AuthorResource.php`: Resource Filament untuk mengelola penulis.
6. `app/Filament/Resources/BookResource.php`: Resource Filament untuk mengelola buku.
7. `app/Filament/Widgets/BooksChart.php`: Widget chart (statistik buku).
8. `app/Filament/Widgets/LibraryStatsWidget.php`: Widget statistik ringkas (total buku, penulis, dll).
9. `app/Policies/BookPolicy.php`: Aturan akses (RBAC) untuk buku.
10. `app/Policies/AuthorPolicy.php`: Aturan akses untuk penulis.
11. `database/factories/*.php`: Factory untuk generate data dummy (Author, Book, User).
12. `database/migrations/*create_authors_table.php`: Skema tabel `authors`.
13. `database/migrations/*create_books_table.php`: Skema tabe; `books`.
14. `database/migrations/*create_categories_table.php` & `*create_book_category_table.php`: Skema tabel kategori & pivot.
15. `database/seeders/CategorySeeder.php`: Seeder data kategori awal.
16. `database/seeders/DatabaseSeeder.php`: Seeder utama yang memanggil factory & seeder lain.
    
---
## ⚙️ Prasyarat & Peralatan

### 1. Pengetahuan yang Diperlukan

Sebelum mengikuti praktikum ini, mahasiswa diharapkan telah memahami hal-hal berikut:

1. Dasar-dasar pemrograman **PHP**, termasuk konsep OOP, penggunaan namespace, dan traits.
2. Pemahaman mengenai **SQL** serta prinsip dasar _database_ relasional.
3. Dasar-dasar **HTML** dan **CSS** (pemahaman Tailwind CSS akan menjadi nilai tambah).
4. Kemampuan menggunakan **_command line_** atau terminal.
5. Pemahaman konsep **MVC** serta dasar penggunaan _framework_ PHP, khususnya Laravel.

### 2. Perangkat Lunak yang Diperlukan

Aplikasi dan perangkat berikut harus sudah terpasang pada komputer:

1. **PHP** versi 8.1 atau lebih baru.
2. **Composer** sebagai _dependency_ manager untuk PHP.
3. **_Database engine_** seperti SQLite, MySQL, atau PostgreSQL.
4. **Text editor atau IDE**, misalnya Visual Studio Code atau PHPStorm.
5. **Git** sebagai alat version control.
6. **Web browser modern** untuk menjalankan dan menguji aplikasi.

---
## 🛠️ Langkah Implementasi

---
## 💻 Penjelasan Kode

### 1. Penambahan Field Description pada Book

#### a. Migration (Penambahan Kolom Description)

`database/migrations/xxxx_create_books_table.php`

Kode berikut menambahkan kolom description bertipe text yang dapat bernilai null:

`$table->text('description')->nullable();`

Kolom ini menjadi penyimpanan utama untuk ringkasan buku. 

#### b. Model (Menambah Description ke `$fillable`

`app/Models/Book.php`

```php
protected $fillable = [
    'isbn',
    'title',
    'author_id',
    'publisher',
    'year',
    'cover',
    'status',
    'description', // Tambah Ini
];
```

Menaruh `description` di `$fillable` memungkinkan Laravel melakukan mass assignment dari form Filament.

#### c. Resource (Menambahkan Textarea pada Form Book

`app/Filament/Resources/BookResource.php`

Kode berikut menambahkan komponen input deskripsi pada form:

```php
Forms\Components\Textarea::make('description')
    ->label('Description')
    ->rows(4)
    ->columnSpanFull();
```

Textarea ditampilkan dalam section "Book Information" sehingga pengguna dapat menuliskan ringkasan buku secara lengkap.

#### d. Factory (Generate Description Dummy)

`database/factories/BookFactory.php`

`'description' => fake()->paragraph(3, true),`

Saat melakukan seeding, setiap buku otomatis memiliki deskripsi realistis. Ini juga memenuhi poin "menambah field description pada factory".

### 2. Implementasi Role-Based Access

#### a. Migration (Menambah Kolom Role)

`database/migrations/xxxx_create_users_table.php`

`$table->enum('role', ['admin', 'staff', 'viewer'])->default('viewer');`

Dengan ini, setiap user memiliki role yang menentukan hak akses.

#### b. Model (Menambah Role ke `$fillable`

`app/Models/User.php`

`protected $fillable = ['name', 'email', 'password', 'role'];`

Agar role bisa diisi saat seeding atau registrasi.

#### c. Seeder (Membuat User Admin, Staff, Viewer)

`database/seeders/DatabaseSeeder.php`

```php
// Admin
        User::factory()->create([
            'name' => 'Admin User',
            'email' => 'admin@example.com',
            'password' => 'admin',
            'role' => 'admin',
            // Kalau mau pasti: 'password' => bcrypt('password'),
        ]);

        // Staff
        User::factory()->create([
            'name' => 'Staff User',
            'email' => 'staff@example.com',
            'password' => 'pwstaff',
            'role' => 'staff',
        ]);

        // Viewer
        User::factory()->create([
            'name' => 'Viewer User',
            'email' => 'viewer@example.com',
            'password' => 'pwviewer',
            'role' => 'viewer',
        ]);
```

Tiga akun dibuat untuk pengujian RBAC:
1. Admin -> akses penuh
2. Staff -> bisa create/view
3. Viewer -> hanya bisa view

#### d. Policy (Aturan Akses pada Buku)

`app/Policies/BookPolicy.php`

```php
public function create(User $user): bool {
    return $user->role !== 'viewer';
}

public function update(User $user, Book $book): bool {
    return $user->role !== 'viewer';
}

public function delete(User $user, Book $book): bool {
    return $user->role === 'admin';
}
```

**Implementasi**

| Role   | View | Create | Update | Delete |
|--------|------|--------|--------|--------|
| Admin  | ✔    | ✔     | ✔      | ✔     |
| Staff  | ✔    | ✔     | ✔      | ✖     |
| Viewer | ✔    | ✖     | ✖      | ✖     |

#### e. Pembatasan Akses pada Table Actions

`BookResource.php -> table()`

```php
Tables\Actions\DeleteAction::make()
    ->visible(fn () => auth()->user()?->role == 'admin'),
```

Tombol delete hanya muncul untuk admin.

### 3. Widget Dashboard

#### a. Widget Statistik

`app/Filament/Widgets/LibraryStatsWidget.php`

Menampilkan:
1. Total Books
2. Total Authors
3. Available vs Borrowed

```php
stat::make('Total Books', Book::count())
    ->description('Books in the library')
    ->color('primary');
```

Widget ini muncul di dashboard Filament dan sesuai dengan instruksi tugas.

#### b. Widget Grafik Pie Chart

`app/Filament/Widgets/BooksChart.php`

```php
$available = Book::where('status', 'available')->count();
$borrowed = Book::where('status', 'borrowed')->count();
```

Pie chart menampilkan rasio:
1. Buku Available
2. Buku Borrowed

Menggunakan Chart.js bawaan Filament.

### 4. Kategori Buku (Many-to-Many)

#### a. Model Category

`app/Models/Category.php`

```php
public function books() {
    return $this->belongsToMany(Book::class);
}
```

#### b. Relasi pada Book

`app/Models/Book.php`

```php
public function categories() {
    return $this->belongsToMany(Category::class);
}
```

#### c. Migration Category dan Pivot

`xxxx_create_categories_table.php`

`xxxx_create_book_category_table.php`

Kode pivot:

```php
$table->foreignId('book_id')->constrained()->cascadeOnDelete();
$table->foreignId('category_id')->constrained()->cascadeOnDelete();
```

Ini memastikan relasi bersih saat sebuah buku dihapus.

#### d. Form Input Categories di BookResource

`BookResource.php -> form()`

```php
Forms\Components\Select::make('categories')
    ->multiple()
    ->relationship('categories', 'name')
    ->preload()
    ->searchable();
```

Pengguna dapat memilih banyak kategori menggunakan dropdown multi-select.

#### 5. Seeder Kategori

`CategorySeeder.php`

Berisi 20 kategori bawaan.

Semua kategori otomatis dibuat dan siap dihubungkan ke buku.

#### 6. Seeder Buku (Attach Kategori)

`DatabaseSeeder.php`

```php
$book->categories()->attach(
    $categories->random(rand(1, 3))->pluck('id')->toArray()
);
```

Setiap buku mendapat 1-3 kategori acak.

---
## 📈 Uji Fungsionalitas CRUD

Pengujian ini dilakukan untuk memastikan seluruh fitur CRUD, relasi, upload file, serta kustomisasi pada aplikasi Bookly berjalan sesuai ketentuan dalam Tugas 2: Kustomasisasi & Pengembangan.

| No. | Fitur yang Diuji            | Deskripsi Uji Singkat                                            | Hasil        |
|-----|-----------------------------|------------------------------------------------------------------|--------------|
| 1   | Tambah Data Author          | Mengisi form dan menyimpan data penulis baru                     | ✅ Berhasil  |
| 2   | Edit Data Author            | Mengubah nama penulis melalui halaman edit                       | ✅ Berhasil  |
| 3   | Hapus Data Author           | Menghapus salah satu data author dari database                   | ✅ Berhasil  |
| 4   | Tambah Data Buku            | Menambah buku dengan ISBN, penulis, status, dan data pendukung   | ✅ Berhasil  |
| 5   | Edit Data Buku              | Mengubah informasi judul, tahun terbit, publisher, atau status   | ✅ Berhasil  |
| 6   | Hapus Data Buku             | Menghapus data buku dari tabel (single delete & bulk delete)     | ✅ Berhasil  |
| 7   | Upload Cover Buku           | Mengunggah gambar cover melalui FileUpload Filament              | ✅ Berhasil  |
| 8   | Relasi Penulis -> Buku      | Memastikan dropdown author berfungsi & data tersimpan            | ✅ Berhasil  |
| 9   | Menambahkan Kategori Buku   | Mengelola kategori & menyimpan hubungan many-to-many             | ✅ Berhasil  |
| 10  | Filter Buku                 | Menyaring data berdasarkan status, tahun terbit, atau author     | ✅ Berhasil  |
| 11  | Pencarian Buku              | Mencari berdasarkan judul, ISBN, atau penulis                    | ✅ Berhasil  |
| 12  | View Detail Buku (Infolist) | Menampilkan detail lengkap buku termasuk cover                   | ✅ Berhasil  |
| 13  | Role Admin                  | Admin dapat melakukan semua aksi (create/edit/delete)            | ✅ Berhasil  |
| 14  | Role Staff                  | Staff hanya dapat create, edit, view (tanpa delete)              | ✅ Berhasil  |
| 15  | Role Viewer                 | Viewer hanya dapat melihat data tanpa akses edit/delete          | ✅ Berhasil  |
| 16  | Widget Dashboard            | Menampilkan total buku, total author, dan chart status           | ✅ Berhasil  |
| 17  | Seeder dan Factory          | Generate dummy data (Author, Book, Category) tanpa error         | ✅ Berhasil  |
| 18  | Validation Input            | Validasi: ISBN unik, field wajib, format tahun                   | ✅ Berhasil  |
| 19  | Storage Link                | File cover tampil benar pada `storage/book-covers`               | ✅ Berhasil  |
| 20  | Pivot Category Buku         | Buku dapat memiliki banyak kategori & tampil di tabel            | ✅ Berhasil  |

---
## ⚠️ Troubleshooting

### 1. Error "Class 'App\Models\Book' not found"

Solusi:

```
composer dump-autoload
php artisan optimize:clear
```

### 2. Migration Error "Table already exists"

Solusi:

`php artisan migrate:fresh --seed`

### 3. Filament Page Not Found (404)

Solusi:

```
php artisan optimize:clear
php artisan route:clear
```

### 4. Upload Error "The file could not be uploaded"

Solusi:

```

php artisan storage:link
# Cek permission folder storage
chmod -R 775 storage
```

### 5. Seeder Error "Call to undefined method factory()"

Solusi:

Pastikan model menggunakan trait `HasFactory`:

```

use Illuminate\Database\Eloquent\Factories\HasFactory;

class Book extends Model
{
    use HasFactory;
    // ...
}
```

### 6. Login Redirect Loop

Solusi:

```
# Clear semua cache
php artisan cache:clear
php artisan config:clear
php artisan view:clear
php artisan route:clear
```

---
## 📸 Hasil Tampilan

### 1. Kolom Description

<img width="1918" height="1079" alt="Kolom Deskripsi Bookly" src="https://github.com/user-attachments/assets/516a10d8-03b6-4dbf-8e8f-dd0aa578aa89" />

### 2. Admin (CRUD)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eac56b52-11a1-45d0-abb7-2820cb31ba6a" />

#### Create

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/bb1c902b-ebe0-4ca0-996d-be10add8d1f0" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/bceec15a-094d-4127-9241-53f79c2cd333" />

#### Read

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/14a429b5-b182-49e2-8926-51499598cff5" />

#### Update

<img width="1919" height="1079" alt="Edit Buku Admin" src="https://github.com/user-attachments/assets/cb58772b-a316-4ecd-9195-d99328e707db" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/02fd287c-e4f9-44ff-bb53-17d1ef1b4959" />

#### Delete

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a39d15bb-8217-4627-a795-737e512b23b7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/874d0f91-0269-4ca7-9e8c-1b36557a7780" />

### 3. Staff (Create, Edit, View)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/678b67f7-4235-4286-a66e-632cb53b6850" />

#### Create

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6c72e068-3203-444f-a01d-7381a4961e11" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/958901c7-e300-424a-bced-d9cb9ddcfddb" />

#### Edit

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/adb7f2c7-667a-4724-a773-daec967fb3c3" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d81f85c5-50b8-44ec-b671-07a81d9b07c5" />

#### View

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/df499fa6-aedd-4155-9b03-2db8f806c8a4" />

### 4. Viewer (View)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1e32d433-7a5f-4645-a58e-5691d0b7c106" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7438c91f-5078-4e72-a0a1-7c2b3c9d463d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1cce5123-07ea-4f28-a2e0-2c6e68cecb7f" />

### 5. Widget (Total Books, Total Authors, dan Books Available vs Borrowed (Chart/Stats))

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dd7c6a19-43bb-4ba2-877c-9af36a6812c8" />

### 6. Model Category & Multiple Select

#### Model Category

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/df7a92c3-5472-45c7-bcf2-2a59ba8dbe5c" />

#### Multiple Select

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/777cd50b-b59e-40ba-879f-2f4436d327d3" />

---
## 🏁 Kesimpulan
