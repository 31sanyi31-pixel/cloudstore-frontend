# Cloud Store Frontend

Platform marketplace Cloud Store dengan sistem login, register, marketplace, dan admin dashboard. Dibangun dengan HTML, CSS, dan JavaScript vanilla.

## 🚀 Fitur

### 1. **Login Page**
- Form login dengan nomor handphone dan password
- Validasi input
- Link ke halaman register
- Local storage untuk menyimpan user session

### 2. **Register Page**
- Form pendaftaran dengan validasi lengkap
- Validasi password match
- Cek duplikasi nomor HP dan email
- Terms & conditions checkbox

### 3. **Marketplace Page**
- Navbar dengan logo dan search bar
- Hero section dengan branding
- Grid produk responsif
- Bottom navigation bar
- User greeting personalisasi

### 4. **Admin Dashboard**
- Sidebar menu dengan navigasi
- Statistics cards (Total Users, Active Users, Locked Accounts, Today's Accounts)
- Tabel daftar akun terdaftar
- Status badges untuk setiap akun
- Logout functionality

## 📋 Flow Aplikasi

```
Login Page
   ↓ (Belum punya akun? → Daftar)
   ↓
Register Page → (Sudah punya akun? → Masuk)
   ↓
Login Page (login)
   ↓
Marketplace Page
   ↓ (Klik avatar/Akun)
   ↓
Admin Dashboard
   ↓ (Keluar)
   ↓
Login Page
```

## 🎨 Design Highlights

- **Color Scheme**: Purple/Indigo gradient (#6366f1 - #7c3aed)
- **Dark Theme**: Background gelap (#1a2332, #1e293b)
- **Responsive Design**: Mobile-first approach
- **Modern UI**: Rounded corners, shadows, smooth transitions
- **Bahasa**: Indonesia

## 💾 Data Storage

Semua data disimpan di **Local Storage** browser:
- `cloudstore_users` - Array semua user terdaftar
- `cloudstore_current_user` - User yang sedang login

## 🔐 Akun Default

Untuk testing, gunakan akun ini:
- **Nomor HP**: 08125854558
- **Password**: Admin123

## 📱 Responsive Breakpoints

- **Desktop**: Full layout dengan sidebar
- **Tablet (768px)**: Layout terbatas
- **Mobile (480px)**: Condensed layout

## 🛠️ Cara Menggunakan

### 1. Download atau Clone
```bash
git clone https://github.com/31sanyi31-pixel/cloudstore-frontend.git
cd cloudstore-frontend
```

### 2. Buka di Browser
```bash
# Cukup buka file index.html dengan browser
open index.html
# atau
firefox index.html
```

### 3. Testing Flow

**Test Register:**
1. Klik "Daftar sekarang" di login page
2. Isi semua form
3. Klik "Daftar Akun"
4. Akan redirect ke login page

**Test Login:**
1. Masukkan nomor HP dan password
2. Klik "Masuk"
3. Akan masuk ke marketplace page

**Test Admin:**
1. Setelah login, klik icon user (avatar) di navbar
2. Akan masuk ke admin dashboard
3. Lihat statistik dan daftar user
4. Klik "Keluar" untuk logout

## 🎯 Fitur Interaktif

- ✅ Form validation (email, password, phone)
- ✅ Password mismatch checking
- ✅ Duplicate user prevention
- ✅ Local storage persistence
- ✅ Dynamic statistics update
- ✅ Menu navigation sidebar
- ✅ Status badges dengan warna berbeda
- ✅ Responsive tables

## 📝 Catatan

**Halaman ini FRONTEND ONLY**, artinya:
- ❌ Tidak terhubung ke database real
- ❌ Tidak bisa mengirim email verifikasi
- ❌ Data hilang saat clear browser cache/local storage
- ❌ Tidak ada backend authentication

Untuk production, Anda perlu:
1. Backend API (Node.js, PHP, Python, dll)
2. Database (MySQL, PostgreSQL, MongoDB, dll)
3. Authentication system (JWT, OAuth, dll)
4. Email verification service

## 🚀 Next Steps

Untuk menambahkan backend, Anda bisa:
1. Buat API endpoint untuk login/register
2. Replace local storage dengan API calls
3. Tambahkan JWT token untuk authentication
4. Integrasikan dengan database

## 📄 File Structure

```
cloudstore-frontend/
├── index.html          # Main file (HTML + CSS + JS)
└── README.md          # Documentation
```

## 👨‍💻 Author

Created by: 31sanyi31-pixel

## 📞 Support

Jika ada pertanyaan atau bug, buat issue di repository ini!

---

**Happy Coding! 🎉**
