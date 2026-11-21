# Kelola Langganan

Aplikasi web sederhana untuk mencatat penjualan langganan, seat per akun, biaya, dan laba.

## Menu
- **Dashboard:** pendapatan diterima, laba bersih, sisa tagihan, langganan aktif, seat tersedia, utilisasi seat, grafik 6 bulan, daftar langganan yang perlu diperpanjang (dengan tombol WhatsApp), dan daftar yang belum dibayar.
- **Penjualan:** catat, ubah, perpanjang, tandai lunas, cari, dan ekspor CSV.
- **Seat:** akun induk yang Anda beli, berisi jumlah seat dan biaya modal per bulan.
- **Biaya:** biaya tambahan di luar modal akun (iklan, pulsa, dll).
- **Pengaturan:** nama usaha, paket dan harganya, serta cadangan data.

## Cara hitung
- **Pendapatan diterima:** penjualan berstatus lunas, dihitung menurut tanggal bayar.
- **Biaya modal:** biaya per bulan setiap akun, dihitung untuk tiap bulan akun itu aktif (sampai bulan berjalan).
- **Laba bersih:** pendapatan diterima dikurangi biaya modal dan biaya tambahan.
- **Sisa tagihan:** penjualan belum lunas yang mulai di periode terpilih.

## Data
Data tersimpan di browser perangkat masing-masing (tidak ada server). Unduh cadangan secara rutin di Pengaturan, lalu gunakan "Pulihkan dari file" untuk memindahkan data ke perangkat lain.

## Memperbarui
Setelah mengedit `index.html`, naikkan versi `const CACHE = "langganan-v1";` di `sw.js` (misalnya menjadi `v2`) supaya perangkat yang sudah meng-install aplikasi ikut mendapat versi terbaru.
