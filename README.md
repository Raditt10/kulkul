Kul-Kul: Sistem Informasi Manajemen Ekstrakurikuler

Kul-Kul adalah aplikasi berbasis web yang dirancang untuk memodernisasi dan mempermudah pengelolaan kegiatan ekstrakurikuler di sekolah. Aplikasi ini menyediakan platform terpusat bagi siswa untuk mendaftar dan melihat informasi, serta bagi admin dan pembina untuk mengelola jadwal, anggota, penilaian, dan prestasi secara efisien.
📌 Deskripsi Project

Sistem ini dibangun untuk mengatasi kendala administrasi manual dalam kegiatan ekstrakurikuler. Dengan Kul-Kul, sekolah dapat memiliki database kegiatan yang terorganisir, transparan, dan mudah diakses.

Tujuan Utama:

    Memudahkan proses pendaftaran siswa baru ke dalam ekstrakurikuler.

    Menyediakan manajemen data anggota, pembina, dan jadwal latihan yang rapi.

    Mencatat rekam jejak prestasi dan penilaian siswa secara digital.

🚀 Fitur Utama
🎓 Halaman Pengunjung & Siswa

    Landing Page Informatif: Menampilkan informasi umum tentang kegiatan sekolah.

    Katalog Ekstrakurikuler: Daftar lengkap ekstrakurikuler beserta deskripsi dan kegiatannya.

    Pendaftaran Online: Formulir digital untuk siswa yang ingin bergabung dengan ekstrakurikuler.

    Profil Siswa: Halaman bagi siswa untuk melihat status keanggotaan mereka.

🛠️ Dashboard Admin & Pembina

    Manajemen Master Data: Pengelolaan data ekstrakurikuler, pembina, dan tahun ajaran.

    Verifikasi Pendaftaran: Fitur untuk menyetujui atau menolak pendaftaran siswa baru.

    Manajemen Jadwal: Pembuatan dan pengaturan jadwal latihan rutin.

    Pencatatan Prestasi: Input data prestasi yang diraih oleh siswa atau tim ekstrakurikuler.

    Input Penilaian: Sistem penilaian kinerja anggota ekstrakurikuler.

    Laporan: Pembuatan laporan kegiatan dan keanggotaan.

    Manajemen Pengguna & Role: Pengaturan hak akses untuk Admin, Pembina, dan Siswa.

🛠️ Tech Stack

Project ini dikembangkan menggunakan teknologi berikut:

    Backend Framework: Laravel 10 (PHP Framework)

    Frontend: Blade Templating Engine, HTML5, CSS3, JavaScript (Vanilla/jQuery)

    Database: MySQL

    Styling: Custom CSS (public/css/style.css)

    Web Server: Apache/Nginx

    Package Manager: Composer (PHP) & NPM (Node.js)

📁 Struktur Folder

Berikut adalah gambaran umum struktur direktori penting dalam proyek ini:
Plaintext

├── app/
│   ├── Http/Controllers/  # Logika kontroler (Admin, Ekskul, Pendaftaran, dll)
│   ├── Models/            # Model Eloquent (Ekskul, Member, Prestasi, dll)
├── database/
│   ├── migrations/        # Struktur skema database
│   ├── seeders/           # Data dummy untuk testing
├── public/
│   ├── css/               # File CSS statis
│   ├── js/                # File JavaScript statis
│   ├── images/            # Aset gambar (logo, foto kegiatan)
├── resources/
│   ├── views/             # Template Blade (admin/, user/, layouts/)
├── routes/
│   ├── web.php            # Definisi rute aplikasi web
├── .env.example           # Contoh konfigurasi environment
└── composer.json          # Dependensi PHP

⚙️ Instalasi & Setup

Ikuti langkah-langkah berikut untuk menjalankan proyek di komputer lokal Anda:
Prasyarat

Pastikan Anda telah menginstal:

    PHP >= 8.1

    Composer

    MySQL Database

    Node.js & NPM (Opsional, jika ada aset yang perlu dikompilasi)

Langkah Instalasi

    Clone Repository
    Bash

    git clone https://github.com/raditt10/kul-kul.git
    cd kul-kul

    Instal Dependensi PHP
    Bash

    composer install

    Instal Dependensi Frontend (Jika diperlukan)
    Bash

    npm install

    Konfigurasi Environment Salin file .env.example menjadi .env:
    Bash

    cp .env.example .env

    Buka file .env dan sesuaikan konfigurasi database Anda:
    Ini, TOML

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=nama_database_anda
    DB_USERNAME=root
    DB_PASSWORD=

    Generate Application Key
    Bash

    php artisan key:generate

    Migrasi dan Seeding Database Jalankan migrasi untuk membuat tabel dan seeder untuk mengisi data awal (dummy data):
    Bash

    php artisan migrate --seed

🖥️ Cara Menjalankan Project

Untuk menjalankan server pengembangan lokal:
Bash

php artisan serve

Akses aplikasi melalui browser di alamat: http://localhost:8000
🔐 Environment Variable Penting

Selain koneksi database, pastikan variabel berikut diatur di .env sesuai kebutuhan (terutama jika menggunakan fitur upload gambar):
Key	Deskripsi
APP_URL	URL aplikasi (misal: http://localhost:8000)
FILESYSTEM_DISK	Driver penyimpanan file (default: local atau public)
🤝 Kontribusi

Kontribusi sangat diterima! Jika Anda ingin berkontribusi pada proyek ini:

    Fork repository ini.

    Buat branch fitur baru (git checkout -b fitur-keren).

    Commit perubahan Anda (git commit -m 'Menambahkan fitur keren').

    Push ke branch tersebut (git push origin fitur-keren).

    Buat Pull Request.

📄 Lisensi

Proyek ini dilisensikan di bawah MIT License. Silakan gunakan dan modifikasi sesuai kebutuhan.

Dibuat oleh [Raditt10]
