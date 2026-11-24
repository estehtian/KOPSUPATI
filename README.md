# KOPSUPATI WEB — Versi 1.1

Website KOPSUPATI (Kopi Susu Pati Kidul), desain modern-futuristic responsif, menggunakan foto outlet dan materi visual yang diberikan.

## Fitur
- Beranda dengan foto outlet asli dan navigasi responsif.
- Halaman menu Coffee, Non Coffee, dan Tea berdasarkan daftar harga yang diberikan.
- Keranjang belanja dengan tambah/kurang jumlah dan penyimpanan browser (localStorage).
- Checkout membuat ringkasan pesanan dan membuka WhatsApp.
- Galeri foto, promo, tentang, kontak, lokasi, FAQ, dan panduan pemesanan.
- Workflow GitHub Actions untuk deploy ke GitHub Pages.

## Pengaturan sebelum online
1. Buka `assets/js/config.js`.
2. Ganti `6281234567890` dengan nomor WhatsApp bisnis KOPSUPATI dalam format internasional, tanpa tanda + atau spasi.
3. Periksa kembali harga dan ketersediaan menu.
4. Upload seluruh isi folder ini ke repository GitHub pada branch `main`.
5. Di GitHub buka **Settings → Pages**, pilih **GitHub Actions** sebagai Build and deployment source.
6. Tunggu workflow selesai pada tab **Actions**.

## Struktur
- `index.html` — beranda
- `pages/` — menu, galeri, promo, tentang, kontak, lokasi, FAQ, pemesanan
- `assets/css/style.css` — desain dan responsive layout
- `assets/js/app.js` — keranjang, filter menu, checkout WhatsApp
- `assets/js/config.js` — konfigurasi WhatsApp dan info outlet
- `assets/images/` — foto asli outlet, menu, promosi, dan pelanggan
- `data/products.json` — data produk dan harga
- `.github/workflows/deploy.yml` — deployment otomatis

## Catatan teknis
Checkout menggunakan WhatsApp, bukan payment gateway. Data keranjang disimpan lokal di browser pengguna. Nomor WhatsApp contoh wajib diganti sebelum menerima pesanan.
