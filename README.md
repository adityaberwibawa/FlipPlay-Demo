# FlipPlay

Landing page dan katalog anime **FlipPlay** — dibuat untuk Tugas Praktikum Pemrograman Web Modul 1.

Proyek ini terdiri dari dua halaman statis yang bisa langsung dibuka di browser tanpa proses build.

## Halaman

### 1. `index.html` — Landing Page
- Hero "Satu Aplikasi. Semua Cerita." dengan navigasi responsif dan menu seluler.
- Statistik platform dan empat fitur utama: Streaming Anime, Drama Asia, Manga Digital, Light Novel.
- Section streaming, bacaan, katalog orisinal, dan tabel harga (Pemula, Plus, Keluarga).
- Form kontak dengan validasi HTML5 dan simulasi pengiriman (tanpa backend).

### 2. `vibe-grid.html` — The Vibe Grid
- Katalog 20 judul anime populer dari [Kitsu API](https://kitsu.app), diambil lewat Fetch API.
- Pencarian judul secara langsung (real-time).
- Filter aura: **High Energy**, **Melancholy**, dan **Binge Mode**.
- Kartu judul berisi poster, rating, genre, tipe, dan tautan trailer.
- Statistik total judul dan rata-rata rating.
- State loading, hasil kosong, dan error dengan tombol coba lagi.

## Teknologi

- HTML5 dan CSS (custom properties)
- [Tailwind CSS](https://tailwindcss.com) via CDN dengan konfigurasi tema inline
- Vanilla JavaScript (ES6)
- Fetch API + Kitsu API

## Menjalankan

Buka `index.html` langsung di browser, atau jalankan server statis lokal:

```bash
python -m http.server 8000
```

Lalu akses <http://localhost:8000>.

> Diperlukan koneksi internet karena Tailwind dimuat dari CDN dan data anime diambil dari Kitsu API.

## Struktur Proyek

```
.
├── index.html        # Landing page
├── vibe-grid.html    # Katalog anime
├── .gitignore
└── README.md
```

## Catatan

- Form kontak hanya simulasi di sisi klien; tidak ada data yang dikirim ke server.
- Data anime dimuat langsung dari Kitsu API saat halaman dibuka.

## Kredit

Tugas Praktikum Pemrograman Web — Modul 1 · FlipPlay Labs, Malang.

Sumber data: [Kitsu API](https://kitsu.app).
