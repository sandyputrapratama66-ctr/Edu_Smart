# EduSmart — Platform E-Learning Sekolah

Aplikasi web e-learning sekolah (single-file HTML/CSS/JS) untuk 4 peran pengguna: **Siswa, Guru, Kepala Sekolah, dan Admin**. Semua data disimpan di `localStorage` browser — tidak butuh server/database, cukup buka file `index.html` di browser.

## ✨ Fitur Utama
- Login multi-role (Siswa / Guru / Kepsek / Admin)
- Dashboard sesuai peran
- Data Siswa, Manajemen Akun, Absensi, Nilai, Rapor/Leger
- Tugas & Materi, Forum Diskusi, Pengumuman
- Laporan Keuangan & Fasilitas Sekolah
- Absen Kehadiran Guru + Scan Barcode/QR Kelas
- Notifikasi, cetak (print-friendly), export Excel (xlsx)
- **Navigasi responsif**: sidebar penuh di laptop/desktop, menu geser (off-canvas) dengan tombol hamburger di HP/tablet

## 🗂️ Struktur Folder
```
edusmart/
├── index.html   # seluruh aplikasi (HTML + CSS + JS jadi satu file)
├── README.md    # dokumentasi ini
└── .gitignore
```

## 🚀 Cara Menjalankan
Karena aplikasi ini murni client-side, cukup:

1. Clone repo ini
   ```bash
   git clone https://github.com/USERNAME/edusmart.git
   cd edusmart
   ```
2. Buka `index.html` langsung di browser, **atau** jalankan local server (disarankan agar semua fitur berjalan normal, misalnya kamera untuk scan barcode):
   ```bash
   python3 -m http.server 8000
   # lalu buka http://localhost:8000
   ```

## 🌐 Deploy Gratis (GitHub Pages)
1. Push repo ini ke GitHub (lihat langkah di bawah).
2. Buka **Settings → Pages** di repo GitHub.
3. Pilih branch `main` dan folder `/ (root)`, klik **Save**.
4. Aplikasi akan aktif di `https://USERNAME.github.io/edusmart/`.

## 💾 Catatan Data
Data (akun, nilai, absensi, dll) disimpan di `localStorage` browser masing-masing pengguna. Artinya:
- Data **tidak** tersinkronisasi antar perangkat/browser.
- Membersihkan cache/localStorage browser akan menghapus data.
- Cocok untuk demo, latihan, atau penggunaan single-device. Untuk penggunaan produksi banyak pengguna, perlu backend/database terpisah.

## 🛠️ Teknologi
- HTML, CSS, JavaScript murni (tanpa framework)
- [xlsx.js](https://github.com/SheetJS/sheetjs) — export Excel
- [html5-qrcode](https://github.com/mebjas/html5-qrcode) — scan QR/barcode
- qrcodejs — generate QR code

## 📄 Lisensi
Bebas digunakan dan dimodifikasi untuk keperluan sekolah/pendidikan.
