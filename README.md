# Chery Tangerang

Landing page resmi Chery Tangerang — `cherytangerang.com`.
Single-file static site (HTML + TailwindCSS via CDN + vanilla JS).

## Struktur

```
cherytangerang/
├── index.html         # Landing page
├── design.md          # Design system & blueprint
└── assets/
    ├── Chery_logo.png
    ├── cars/          # Foto produk mobil Chery
    ├── customers/     # Galeri sales bersama konsumen
    └── sales/         # Foto profil sales (Nayla Juliana)
```

## Section Homepage

1. **Hero** — Pre-Book Chery Q (full image)
2. **Special Offer** — J6 Hitam NIK 2025 (banner promo)
3. **Foto Produk** — Lineup 10 mobil Chery
4. **Profil Sales** — Nayla Juliana + kontak (WA, IG, TikTok, Email)
5. **Galeri** — Sales bersama konsumen
6. **Lokasi** — Maps showroom

## Kontak Sales

- WhatsApp: `+62 812-3456-7890` (placeholder, ganti sebelum live)
- Instagram: [@cherypik2_](https://instagram.com/cherypik2_)
- TikTok: [@nalavyu](https://tiktok.com/@nalavyu)
- Email: naylajuliana16@gmail.com

## Cara Preview

Buka `index.html` langsung di browser. Tailwind dan Google Fonts dimuat via CDN (butuh koneksi internet).

## Catatan Handoff

- Ganti placeholder WhatsApp `6281234567890` ke nomor asli (find & replace di `index.html`).
- Sesuaikan alamat showroom & query Google Maps di section `#lokasi` dan footer.
- Untuk production sebaiknya Tailwind di-build statis (Tailwind CLI / PostCSS) supaya tidak bergantung CDN.
