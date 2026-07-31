# UKOM_web-umkm
Berisi Penjelasan, Dokumentasi, tentang apa web yang di buat. Saya membuat web UMKM dengan layout mengikuti MUSICVILLA.COM

============================================================================

## 1. Ringkasan Proyek
Loopora adalah antarmuka toko daring (e-commerce) yang berfokus pada produk buatan tangan (handmade crochet/crafts). Desain antarmuka mengusung estetika cozy, hangat, dan ceria (cheerful) dengan skema warna pastel serta palet utama charcoal untuk menjaga keterbacaan teks.

## 2. Struktur Utama HTML (index.html)
Halaman web dibangun menggunakan struktur semantik HTML5 murni:
### A. Elemen Navigasi & Header (<header>)
- Sticky Navigation (.header): Menggunakan position: sticky agar header tetap berada di bagian atas layar saat pengguna melakukan scroll.
- Mega Menu / Dropdown (.dropdown-menu): Navigasi multi-kolom yang muncul saat hover pada menu seperti SHOP, COLLECTIONS, SERVICES, dan ABOUT US.
- Header Actions (.header-actions): Menyediakan tombol aksi cepat seperti Account, Search, dan Cart dalam bentuk ikon.

### B. Area Utama (<main>)
- Hero Banner (.hero-banner): Area promosi tunggal (single static hero) dengan teks tipografi tebal (EVERY LOOP TELLS A STORY), subteks, serta tombol Call-to-Action (CTA).
- Grid Produk (.product-section): Menampilkan daftar produk menggunakan layout CSS Grid 4 kolom. Elemen gambar produk menggunakan latar warna-warni pastel (pink-bg, yellow-bg, mint-bg, lavender-bg, coral-bg).
- Ulasan Pelanggan (.review-section): Menampilkan kartu ulasan dengan elemen rating bintang 5 dan badge Verified Customer.
-Video Stories (.video-section): Menampilkan konten visual/cerita di balik pembuatan produk (Behind The Loop).
- Trending & Newsletter (.trending, .newsletter): Bagian tautan navigasi tren serta form berlangganan buletin.
- Peta Lokasi Toko (.location-section): Menggabungkan visual peta lokasi toko fisik dengan kartu informasi alamat (.location-card).

### C. Footer (<footer>)
Menyajikan informasi lokasi toko, jam operasional (Store Hours), tautan bantuan/layanan (Support), form berlangganan newsletter, serta tautan media sosial (Instagram, Facebook, YouTube, TikTok).

## 3. Sistem Desain & Styling CSS (style.css)
### A. Palet Warna Utama
- Latar Belakang Utama: #fff8ec (Cream/Pastel Off-White hangat)
- Teks & Akses Utama: #413b48 (Charcoal Muted)
- Warna Akses Pastel (Aksen Produk):
- Pink: #f5b6c1
- Yellow: #f7d774
- Coral: #f6a790
- Mint: #bfe3c6
- Lavender: #cbb6f3

### B. Teknik Layout & Posisi
CSS Grid: Digunakan pada .product-grid, .review-grid, .video-grid, .trending-grid, dan .footer-main untuk kemudahan pengaturan kolom secara simetris.
<br>
Flexbox: Digunakan pada area navigasi (.main-nav), susunan kartu (.header-actions), serta perataan isi dalam kartu produk/ulasan.
<br>
Responsive Typography: Header menggunakan fungsi clamp(45px, 7vw, 90px) agar ukuran font h1 menyesuaikan secara otomatis dengan lebar layar tanpa membuat teks terpotong (overflow).
