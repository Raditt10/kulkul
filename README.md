# Kul-Kul: Sistem Informasi Manajemen Ekstrakurikuler

![Laravel](https://img.shields.io/badge/Laravel-v10.x-FF2D20?style=flat&logo=laravel)
![PHP](https://img.shields.io/badge/PHP-%5E8.1-777BB4?style=flat&logo=php)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=flat&logo=mysql)
![Vite](https://img.shields.io/badge/Vite-Frontend-646CFF?style=flat&logo=vite)
![License](https://img.shields.io/badge/License-MIT-green)

**Kul-Kul** adalah aplikasi berbasis web yang dibangun untuk memodernisasi pengelolaan kegiatan ekstrakurikuler di sekolah. Aplikasi ini menggantikan sistem pencatatan manual dengan platform digital yang terintegrasi, memudahkan siswa dalam mendaftar dan admin dalam mengelola data kegiatan, anggota, serta penilaian.

## 📌 Deskripsi Project
Sistem ini memfasilitasi interaksi antara sekolah (Admin/Pembina) dan Siswa:
* **Siswa** dapat melihat katalog ekstrakurikuler, mendaftar secara online, melihat jadwal, dan memantau riwayat aktivitas mereka.
* **Admin/Pembina** memiliki kendali penuh untuk mengelola master data ekstrakurikuler, memvalidasi pendaftaran, mengatur jadwal latihan, mencatat prestasi, hingga memberikan penilaian (e-rapor ekskul).

## 🛠️ Tech Stack
Teknologi utama yang digunakan dalam pengembangan:

* **Backend Framework:** Laravel 10 (PHP)
* **Frontend:** Blade Templating Engine
* **Styling & UI:** CSS3, JavaScript (Vanilla & jQuery), Bootstrap (via CDN/Local)
* **Database:** MySQL
* **Build Tool:** Vite (untuk manajemen aset CSS/JS)
* **Server:** Apache / Nginx

## 🚀 Fitur Utama

### 👥 Halaman Siswa (User Interface)
* **Landing Page Interaktif**: Informasi visual mengenai kegiatan sekolah.
* **Katalog Ekstrakurikuler**: Daftar lengkap ekskul dengan deskripsi detail.
* **Formulir Pendaftaran Online**: Proses pendaftaran anggota baru yang mudah.
* **Dashboard Siswa**: Halaman profil, status keanggotaan, dan notifikasi.
* **Informasi Jadwal**: Kalender kegiatan latihan rutin.

### 🛡️ Dashboard Admin & Pembina
* **Dashboard Statistik**: Ringkasan jumlah siswa, ekskul aktif, dan pendaftaran baru.
* **Manajemen Master Data**: CRUD untuk data Ekstrakurikuler, Pembina, dan Tahun Ajaran.
* **Validasi Pendaftaran**: Fitur untuk menerima atau menolak calon anggota baru.
* **Manajemen Anggota**: Database lengkap siswa yang aktif di setiap ekskul.
* **Manajemen Jadwal**: Pembuatan jadwal latihan dan event.
* **Pencatatan Prestasi**: Input data kejuaraan yang diraih oleh ekskul.
* **Penilaian Anggota**: Input nilai kinerja, kedisiplinan, dan keaktifan siswa.
* **Laporan**: Rekapitulasi data untuk keperluan administrasi sekolah.
* **Pengaturan Akun**: Manajemen profil dan password pengguna.

## 📁 Struktur Folder Project
Berikut adalah struktur direktori utama yang relevan dalam project ini:

```text
kul-kul/
├── app/
│   ├── Http/Controllers/   # Logika bisnis (AdminController, EkskulController, dll)
│   ├── Models/             # Model Database (Ekskul, Member, Nilai, Prestasi, dll)
├── database/
│   ├── migrations/         # Struktur tabel database
│   ├── seeders/            # Data dummy untuk pengujian
├── public/
│   ├── css/                # File style kustom (style.css, sidebarscroll.css)
│   ├── images/             # Aset gambar (logo, foto kegiatan)
│   ├── js/                 # Script interaktif (sidebar.js, modal.js, notif.js)
├── resources/
│   ├── css/                # Source CSS (Tailwind/Bootstrap jika ada)
│   ├── js/                 # Source JavaScript (app.js, bootstrap.js)
│   ├── views/              # Tampilan aplikasi (Blade)
│       ├── admin/          # View khusus halaman Admin (dashboard, form, tabel)
│       ├── user/           # View khusus halaman Siswa (home, profile, daftar)
│       └── layouts/        # Template utama (navbar, sidebar, footer)
├── routes/
│   ├── web.php             # Definisi routing aplikasi
│   └── admin.php           # Routing khusus admin (jika dipisah)
└── .env.example            # Template konfigurasi environment

