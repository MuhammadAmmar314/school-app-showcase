# SekolahApp Enterprise Commercial License Agreement

Copyright (c) 2026 SekolahApp. All Rights Reserved.

Perjanjian Lisensi Komersial ini ("Perjanjian") dibuat antara pengembang/pemegang hak cipta SekolahApp ("Penyedia Lisensi") dan pihak pembeli ("Pemegang Lisensi").

Dengan membeli dan mengunduh kode sumber (source code) lengkap SekolahApp, Anda menyatakan menyetujui seluruh ketentuan dan batasan penggunaan di bawah ini:

---

## 1. Jenis Lisensi & Hak Penggunaan

### A. Lisensi Standar (Single School / 1 Domain)
- Diberikan hak untuk menginstal dan menggunakan SekolahApp pada **1 (satu) instansi sekolah / 1 nama domain**.
- Dilengkapi **License Key Kriptografis (HMAC SHA-256)** dengan kuota 1 domain aktif.
- Akses penuh terhadap seluruh source code Laravel & React untuk keperluan kustomisasi internal instansi tersebut.
- **Dilarang**: Menyebarkan, menjual ulang, atau memasang source code pada lebih dari 1 sekolah/domain tanpa membeli lisensi tambahan.

### B. Lisensi Multi-Sekolah (Hingga 5 Instansi)
- Diberikan hak untuk memasang dan menjalankan sistem pada hingga **5 (lima) instansi sekolah** di bawah payung yayasan yang sama atau dikelola oleh agensi yang sama.
- Dilengkapi **Multi-Domain License Key** dengan kuota auto-bind hingga 5 domain aktif secara teknis. Instalasi pada domain ke-6 akan otomatis terkunci kecuali dilakukan upgrade kuota.
- Akses penuh source code dan konfigurasi identitas sekolah dinamis (`config/school.php`).
- **Dilarang**: Menjual ulang kode sumber secara publik atau mengklaim kepemilikan hak cipta atas core framework.

### C. Lisensi White-Label & Developer (Unlimited Deployments)
- Diberikan hak penuh untuk melakukan *rebranding* (mengganti nama produk, logo, tema) dan menginstal pada jumlah instansi sekolah **tanpa batas**.
- Dilengkapi **Enterprise Unlimited License Key** (tanpa batasan kuota domain).
- Cocok untuk Software House, IT Consultant, atau Agensi EduTech yang menjual solusi turnkey ke sekolah-sekolah.
- **Dilarang keras**: Mengunggah kembali (*re-upload*) source code ke repositori publik (GitHub, GitLab publik, forum unduhan, dsb.) atau mendistribusikannya secara gratis.

---

## 2. Mekanisme Proteksi & Verifikasi Teknis (DRM & Activation)
1. **Verifikasi Kriptografis**: Setiap instalasi di luar server lokal pengujian diverifikasi menggunakan tanda tangan digital HMAC SHA-256 (`LicenseService`).
2. **Kloning & Kuota Domain**: Sistem mencatat domain resmi yang diaktivasi. Jika batas kuota paket Multi-School (5 domain) tercapai, sistem akan mengarahkan domain baru ke halaman aktivasi `/license/activate` dan menolak akses operasional sampai kuota ditambah.
3. **Bypass Pengembang Lokal**: Lingkungan lokal (`localhost`, `127.0.0.1`, `*.test`) otomatis dibebaskan (*bypassed*) agar proses development/coding pengembang tidak terganggu.

---

## 2. Batasan & Larangan Keras (Restrictions)
1. **Dilarang Publikasi Terbuka**: Anda tidak diizinkan untuk mempublikasikan source code lengkap SekolahApp di repositori publik (seperti GitHub publik), forum internet, situs torrent, atau media penyimpanan yang dapat diakses publik.
2. **Dilarang Menjual Ulang Kode Mentah**: Anda tidak diperbolehkan menjual source code sebagai produk template atau script mentah di marketplace script umum tanpa izin tertulis dari Penyedia Lisensi.
3. **Penyalahgunaan**: Segala bentuk pembajakan atau pelanggaran hak cipta akan mengakibatkan pencabutan lisensi secara sepihak dan dapat diproses sesuai Undang-Undang Hak Cipta yang berlaku.

---

## 3. Garansi & Pemeliharaan
- Kode sumber disediakan *"as is"* dengan jaminan telah melalui pengujian unit dan integrasi (PHPUnit feature tests).
- Update perbaikan bug dan pembaruan keamanan dasar disediakan sesuai paket pembelian yang disepakati.

---

## 4. Kontak Pemesanan & Klarifikasi Lisensi
Untuk pembelian lisensi resmi, invoice perusahaan, atau konsultasi kustomisasi:
- **WhatsApp**: +62 812-XXXX-XXXX
- **Email**: sales@sekolahapp.com / dev@sekolahapp.com
