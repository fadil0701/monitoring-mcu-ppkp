# 🏥 Sistem Monitoring MCU PPKP DKI Jakarta

Sistem monitoring dan penjadwalan Medical Check Up (MCU) terpadu untuk pegawai PPKP DKI Jakarta dengan antarmuka yang modern dan user-friendly.

## ✨ **Fitur Utama**

### 🎨 **Antarmuka Modern & Responsif**
- **Design System**: Menggunakan Bootstrap 5 dengan custom styling
- **Color Scheme**: Gradient modern dengan tema kesehatan
- **Typography**: Font Inter untuk keterbacaan optimal
- **Icons**: Font Awesome 6 untuk ikon yang konsisten
- **Responsive**: Fully responsive untuk desktop, tablet, dan mobile

### 🔐 **Sistem Autentikasi**
- **Login Page**: Halaman login yang menarik dengan fitur showcase
- **Registration**: Form pendaftaran MCU yang lengkap dan user-friendly
- **Role-based Access**: Super Admin, Admin, dan User
- **Security**: CSRF protection, password hashing, session management

### 📊 **Dashboard & Monitoring**
- **Admin Dashboard**: Filament admin panel dengan widgets dan charts
- **Client Dashboard**: Dashboard user dengan statistik real-time
- **Analytics**: Grafik dan laporan komprehensif
- **Real-time Updates**: Data yang selalu up-to-date

### 🗓️ **Penjadwalan MCU**
- **Auto Scheduling**: Sistem penjadwalan otomatis
- **3-Year Rule**: Validasi interval MCU 3 tahun
- **Status Tracking**: Tracking status jadwal (Terjadwal/Selesai/Batal)
- **Notifications**: Email dan WhatsApp notifications

### 📋 **Manajemen Data**
- **Participant Management**: CRUD lengkap untuk data peserta
- **Schedule Management**: Manajemen jadwal MCU
- **Results Management**: Upload dan download hasil MCU
- **File Management**: Support untuk PDF, DOC, dan gambar

### 📧 **Komunikasi Terpadu**
- **Email System**: SMTP integration dengan template
- **WhatsApp API**: Integration dengan WhatsApp Business API
- **Bulk Notifications**: Pengiriman notifikasi massal
- **Template Management**: Template yang dapat dikustomisasi

### 📈 **Reporting & Analytics**
- **Custom Reports**: Laporan komprehensif
- **Export Features**: Export ke Excel dan PDF
- **Charts & Graphs**: Visualisasi data yang informatif
- **Filtering**: Filter berdasarkan berbagai kriteria

## 🚀 **Teknologi yang Digunakan**

- **Backend**: Laravel 12 (PHP 8.2+ / 8.3+)
- **Admin Panel**: Filament 3.3
- **Frontend**: Bootstrap 5, Font Awesome 6
- **Database**: MySQL 8.0+
- **Authentication**: Laravel Breeze
- **File Storage**: Laravel Storage
- **Email**: SMTP dengan template
- **WhatsApp**: Business API integration

## ⚙️ **System Requirements**

### PHP Requirements
- **PHP Version**: 8.2.x or 8.3.x (Recommended: PHP 8.3 for better performance)
- **Required Extensions**:
  - cURL (HTTP requests & API)
  - Fileinfo (File type detection)
  - GD (Image manipulation)
  - Intl (Internationalization)
  - Mbstring (Multibyte strings)
  - MySQLi/PDO (Database)
  - OpenSSL (Encryption & HTTPS)
  - ZIP (File compression)
  - XML & DOM (PDF & XML processing)

### Recommended Extensions
- Redis (Caching & sessions)
- Imagick (Advanced image processing)
- OPcache (Performance optimization)

### Server Requirements
- **Web Server**: Apache 2.4+ / Nginx 1.18+
- **Database**: MySQL 8.0+ / MariaDB 10.6+
- **Memory**: Minimum 256MB, Recommended 512MB
- **Storage**: Minimum 500MB for application + data

### Tools & Dependencies
- **Composer**: 2.5+
- **Node.js**: 18.x or 20.x
- **NPM**: 9.x or 10.x

## 🔧 **Upgrade PHP ke 8.3**

Sistem ini sudah support PHP 8.3 untuk performa lebih baik! 

### Cara Upgrade:
1. Lihat panduan lengkap di **[UPGRADE_PHP.md](UPGRADE_PHP.md)**
2. Jalankan check kompatibilitas:
   ```bash
   php check-php-compatibility.php
   ```
3. Setelah upgrade, jalankan:
   ```bash
   after-php-upgrade.bat
   ```

### Benefits PHP 8.3:
- ⚡ 8-10% lebih cepat dari PHP 8.2
- 🧠 5% lebih hemat memory
- 🔒 Security improvements
- ✨ Better error messages

## 🚀 **Quick Start**

### 1. Check System Compatibility
```bash
php check-php-compatibility.php
```

### 2. Install Dependencies
```bash
composer install
npm install
```

### 3. Setup Environment
```bash
cp env.production .env
# Edit .env sesuai konfigurasi lokal Anda
```

### 4. Generate Application Key
```bash
php artisan key:generate
```

### 5. Run Migrations & Seeders
```bash
php artisan migrate --seed
```

### 6. Build Assets
```bash
npm run build
# atau untuk development:
npm run dev
```

### 7. Start Development Server
```bash
php artisan serve
# Buka: http://localhost:8000
```

## 📚 **Dokumentasi Tambahan**

### Getting Started
- 📖 [Quick Start](QUICK_START.md) - Panduan setup lokal cepat
- 📄 [Setup Manual](SETUP%20MANUAL.txt) - Setup lengkap step-by-step

### Deployment
- 🐳 **[Docker Deployment](DOCKER_DEPLOYMENT.md)** - **RECOMMENDED** untuk production
- 🐳 [Docker Quick Reference](DOCKER_QUICK_REFERENCE.md) - Command reference Docker
- 🚀 [Native Deployment](DEPLOY_NOW.md) - Deploy tanpa Docker

### Optimization & Maintenance
- 🔧 [PHP Upgrade Guide](UPGRADE_PHP.md) - Upgrade ke PHP 8.3
- ⚡ [Dashboard Optimization](OPTIMASI_DASHBOARD.md) - Optimasi performa
- 🧪 [Testing Guide](TESTING_GUIDE.md) - Panduan testing aplikasi

## 🛠️ **Development Tools**

### Available Scripts

#### Composer Scripts
```bash
composer dev        # Start development (server + queue + logs + vite)
composer test       # Run PHPUnit tests
```

#### Artisan Commands
```bash
php artisan serve           # Start development server
php artisan migrate         # Run migrations
php artisan db:seed         # Run seeders
php artisan optimize:clear  # Clear all caches
php artisan test            # Run tests
```

#### NPM Scripts
```bash
npm run dev         # Start Vite development server
npm run build       # Build for production
npm run watch       # Watch files for changes
```

## 🔐 **Default Admin Access**

Setelah menjalankan seeders, gunakan kredensial berikut:

### Super Admin
- Email: `superadmin@ppkp.jakarta.go.id`
- Password: `password`

### Admin
- Email: `admin@ppkp.jakarta.go.id`
- Password: `password`

⚠️ **PENTING**: Segera ganti password default setelah login pertama!

## 📞 **Support & Contact**

Untuk bantuan dan pertanyaan:
- **Email**: admin@ppkp.jakarta.go.id
- **Phone**: +62 812 345 678

---

**© 2025 PPKP DKI Jakarta. All rights reserved.**


