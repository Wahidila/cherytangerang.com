# Chery Tangerang — Design System

> Landing page resmi sales Chery untuk wilayah Tangerang.
> Domain: **cherytangerang.com**

---

## 1. Brand Identity

| Aspek | Nilai |
|---|---|
| **Brand Name** | Chery Tangerang |
| **Tagline** | "Smart, Stylish, Sustainable — Dealer Resmi Chery di Tangerang" |
| **Positioning** | Dealer resmi Chery di Tangerang yang menawarkan rangkaian SUV & EV terkini, didampingi sales konsultan profesional, harga transparan, dan promo terbaik (cash bertahap, kredit 0%, tukar tambah). |
| **Audience** | Profesional, keluarga muda, pengusaha, ASN/BUMN/tenaga medis di Tangerang & sekitarnya, usia 28-55, segment menengah-atas. |
| **Tone of Voice** | Premium, trustworthy, modern, tenang. Tidak salesy norak. |

---

## 2. Color System

Palette mengadopsi DNA brand Chery (merah signature) dipadu navy-charcoal yang premium dan aksen gold tipis untuk kelas atas.

| Token | Hex | Role | Usage |
|---|---|---|---|
| `--c-ink` | `#0B1220` | Primary surface (dark) | Background hero, footer, nav saat scrolled |
| `--c-ink-soft` | `#131C2E` | Surface secondary | Card dark, section CTA |
| `--c-crimson` | `#E11D2E` | Accent primary (Chery red) | Tombol CTA utama, harga highlight, badge "NEW" |
| `--c-crimson-deep` | `#B7141F` | Accent dark | Hover state, gradien |
| `--c-gold` | `#C9A24C` | Accent secondary (luxury) | Garis tipis, sparkle, separator |
| `--c-cream` | `#F6F1E7` | Surface light | Background section terang |
| `--c-snow` | `#FFFFFF` | Surface base | Background card, body utama |
| `--c-slate` | `#4A5468` | Body text on light | Paragraf, deskripsi |
| `--c-mist` | `#E5E8EE` | Border / divider | Garis pembatas card, input |

**Aturan kontras:**
- Heading di atas `--c-snow` selalu pakai `--c-ink`.
- Tombol CTA utama: `--c-crimson` background + `--c-snow` text.
- Tombol CTA sekunder (outline): border `--c-ink` + text `--c-ink`.
- HINDARI text gold di atas snow (kontras buruk). Gold hanya untuk garis & dekorasi.

---

## 3. Typography System

Pasangan distinctive yang modern-premium, bukan generic.

| Role | Font | Weight | Source |
|---|---|---|---|
| **Display / Headline** | `Sora` | 600 / 700 / 800 | Google Fonts |
| **Body / UI** | `Manrope` | 400 / 500 / 600 / 700 | Google Fonts |
| **Numerik harga** | `Sora` | 800 (tabular-nums) | — |

### Skala (mobile-first, naik di desktop)

| Level | Mobile | Desktop | Line | Use |
|---|---|---|---|---|
| Display | 40px / 700 | 72px / 800 | 1.05 | Hero headline |
| H1 | 32px / 700 | 48px / 700 | 1.15 | Section title |
| H2 | 24px / 700 | 32px / 700 | 1.2 | Card title |
| H3 | 18px / 600 | 20px / 600 | 1.3 | Sub-title |
| Body-lg | 17px / 400 | 18px / 400 | 1.6 | Paragraf utama |
| Body | 15px / 400 | 16px / 400 | 1.6 | Body default |
| Caption | 13px / 500 | 13px / 500 | 1.4 | Label, badge |

Tracking heading: `-0.02em`. Body: normal.

---

## 4. Layout Blueprint (Top → Bottom) — Revisi Klien

Urutan section sesuai permintaan klien (final):

1. **Top Announce Bar** — strip atas tipis, link sosmed Nayla (IG @cherypik2_, TikTok @nalavyu).
2. **Sticky Top Nav** — logo Chery + menu (Beranda · Special Offer · Mobil · Profil Sales · Galeri · Lokasi) + CTA WhatsApp merah.
3. **Section 1 — Hero: Chery Q Pre-Book** — headline "Pre-Book Chery Q di Tangerang", foto produk Chery Q (chery-q-prebook.jpg) sebagai visual utama, dual CTA (Pre-Book WA + Lihat Mobil Lain), social proof avatar customer.
4. **Section 2 — Special Offer J6 Hitam NIK 2025** — banner full dengan gambar `j6-special-price.png`, 4 benefit highlight (discount, cash bertahap, garansi, free aksesoris), CTA klaim WA.
5. **Section 3 — Foto Produk (Lineup 10 Mobil)** — grid card responsif 1/2/3 kolom, tiap card foto + nama + harga + 4 tombol promo WA dinamis.
6. **Section 4 — Profil Sales (Nayla Juliana)** — foto Nayla + perkenalan + grid 5 kontak (WhatsApp, Telepon, Instagram @cherypik2_, TikTok @nalavyu, Email naylajuliana16@gmail.com).
7. **Section 5 — Galeri Sales Bersama Konsumen** — grid 3-4 kolom, 7 foto delivery + 1 stat card "500+ customer".
8. **Section 6 — Lokasi (Maps)** — info alamat + jam ops + kontak (kiri) dan Google Maps embed iframe (kanan).
9. **Footer** — logo, copy, sosmed (WA + IG + TikTok + Email), navigasi, kontak Nayla, copyright.
10. **Floating WhatsApp Button** — fixed bottom-right, animasi pulse, link langsung ke WA Nayla.

**Section yang DIHAPUS** dari versi sebelumnya: Trust Strip, Showcase Featured 4 mobil, Promo Banner generic, Test Drive & Trade-In CTA section, Tentang Chery (sejarah brand). Klien mau halaman lebih ringkas dan langsung fokus ke produk + sales.

---

## 5. Visual Style

| Property | Value |
|---|---|
| Border radius | Card: `16px` · Button: `9999px` (pill) · Image: `12px` |
| Shadow card light | `0 12px 32px -16px rgba(11,18,32,.18)` |
| Shadow card hover | `0 24px 48px -20px rgba(11,18,32,.28)` |
| Card padding | `28px` desktop · `20px` mobile |
| Section padding-y | `96px` desktop · `64px` mobile |
| Container max-width | `1240px` |
| Gutter | `24px` (mobile) / `32px` (desktop) |

**Card pattern (mobil):**
- White surface, radius 16, shadow-card.
- Gambar mobil di top, aspect 16:10, object-contain.
- Padding bawah 24px berisi: nama (H2) → "Start dari" (caption gray) → harga (Sora 800, crimson) → list 4 tombol WA pill outline kecil.

**Tombol patterns:**
- **Primary** (crimson pill): `bg-crimson text-snow px-7 py-3.5 rounded-full font-semibold` + hover `bg-crimson-deep` + scale 1.02.
- **Outline ink**: `border-2 border-ink text-ink px-7 py-3.5 rounded-full font-semibold` + hover bg-ink text-snow.
- **Pill kecil promo** (di card): `border border-mist text-ink px-3.5 py-2 rounded-full text-[13px]` + hover border-crimson + text-crimson.

---

## 6. Motion & Animation

| Animation | Spec |
|---|---|
| Scroll reveal | `opacity 0 → 1`, `translateY(24px → 0)`, 600ms ease-out, IntersectionObserver `threshold:0.1`, stagger 80ms |
| Float decorative | 7s ease-in-out infinite, `translateY(-10px)` + `rotate(4deg)` |
| Float slow | 11s ease-in-out infinite, `translateY(-14px)` |
| Hover card | `translateY(-4px)` + shadow naik, 280ms cubic-bezier(.2,.8,.2,1) |
| Hover button | `scale(1.02)`, 220ms |
| Nav scrolled | Background `--c-ink` 95% blur 12px, 240ms |
| WA float pulse | 2s infinite, ring crimson opacity 0.4 → 0 |

Respect `prefers-reduced-motion: reduce` → matikan float & scale.

---

## 7. Decorative Elements (inline SVG)

Seluruh elemen dekoratif memakai **inline SVG** (transparan, tajam, ringan, terkontrol penuh), bukan PNG.

| Element | Fungsi | Warna | Size |
|---|---|---|---|
| 8-point sparkle | Floating accent hero & section header | `--c-gold` opacity 0.7 | 24-40px |
| Diamond rhombus | Floating accent CTA banner | `--c-crimson` opacity 0.55 | 16-22px |
| Thin ring outline | Decoration sudut hero & footer | `--c-gold` opacity 0.35 | 96-160px |
| Shield emblem | Trust badge "Authorized Dealer" | `--c-gold` | 28px inline |
| Diagonal line group | Section divider | `--c-mist` | full-width |

Aturan: max 6 elemen floating per viewport, semua `pointer-events:none`, `aria-hidden="true"`.

---

## 8. Content Architecture

### Hero
- Eyebrow: `DEALER RESMI CHERY · TANGERANG`
- Headline: `Mobil Chery Resmi, Harga Terbaik di Tangerang.`
- Sub: `Pilihan SUV dan EV terlengkap — Tiggo Series, J6, C5, E5. Konsultasi gratis, test drive di rumah, promo cash bertahap & kredit 0%.`
- CTA-1: `Konsultasi WhatsApp` (crimson)
- CTA-2: `Lihat Semua Mobil` (outline → anchor #lineup)

### Trust Strip (4 item)
1. `Authorized Dealer` · ikon shield
2. `10+ Model SUV & EV` · ikon mobil
3. `Test Drive Gratis` · ikon kunci
4. `Bunga Kredit 0%*` · ikon persen

### Lineup (10 mobil)
| # | Nama | Start Harga | Image |
|---|---|---|---|
| 1 | Chery J6 | Rp 565.500.000 | `j6-special-price.png` |
| 2 | Chery J6T | Rp 585.500.000 | `j6t.png` |
| 3 | Tiggo Cross Sport | Rp 281.900.000 | `tiggo-cross-sport.png` |
| 4 | Tiggo 8 CSH | Rp 454.900.000 | `tiggo-8-csh.png` |
| 5 | Tiggo 8 | Rp 367.500.000 | `tiggo-8.png` |
| 6 | Tiggo Cross CSH | Rp 334.900.000 | `tiggo-cross-csh.png` |
| 7 | Tiggo Cross | Rp 269.500.000 | `tiggo-cross.png` |
| 8 | Tiggo 9 CSH | Rp 749.900.000 | `tiggo-9-csh.png` |
| 9 | Chery C5 | Rp 321.000.000 | `c5.png` |
| 10 | Chery C5 CSH | Rp 404.900.000 | `c5-csh.webp` |

Tombol per card (4): Cash 50:50 · Cek Angsuran · Promo Kredit 0% · Tukar Tambah — semua link `wa.me/<NUMBER>` dengan text dinamis nama mobil.

### Showcase Featured (4 spec card)
- **Tiggo 8 CSH** — 1.5L Hybrid · 204 Ps · 310 Nm
- **Chery J6** — 65,69 kWh · 418 km · Charging 30m (30-80%)
- **Tiggo Cross CSH** — 1.5L DHE · 204 Ps · 310 Nm
- **Chery C5 CSH** — 1.5L TGDI · 204 Ps · 310 Nm

### Test Drive & Trade-In
- Test Drive: "Coba langsung mobil Chery favorit Anda. Kami antar unit ke rumah."
- Trade-In: "Tukar mobil lama Anda jadi Chery. Penilaian fair dan transparan."

### Sales Profile (FINAL — Nayla Juliana)
- **Nama:** Nayla Juliana
- **Jabatan:** Sales Consultant Chery Tangerang
- **WhatsApp:** `+62 812-3456-7890` (placeholder — ganti sebelum live)
- **Instagram:** [@cherypik2_](https://instagram.com/cherypik2_)
- **TikTok:** [@nalavyu](https://tiktok.com/@nalavyu)
- **Email:** naylajuliana16@gmail.com

---

## 9. Responsive Breakpoints

| Range | Layout |
|---|---|
| `< 640px` | 1 kolom, hamburger nav, hero stack |
| `640-1024px` | 2 kolom card, nav full, hero side-by-side |
| `> 1024px` | 3 kolom card, full design system |
| `> 1280px` | Container 1240px center, padding generous |

---

## 10. Accessibility

- WCAG AA contrast minimum (cek `crimson` di atas snow untuk text → cukup; di atas ink → gunakan crimson lebih terang atau snow).
- Semua dekorasi `aria-hidden="true"`.
- Tombol WA punya `aria-label` lengkap (target nama mobil + tipe promo).
- Skip-to-content link tersembunyi.
- Focus ring visible: `outline: 2px solid var(--c-crimson); outline-offset: 3px`.
- `alt` deskriptif pada foto mobil & customer.
- Form/input (jika ada) pakai label visible.

---

## 11. Asset Map

```
D:\cherytangerang\
├── index.html
├── design.md
└── assets\
    ├── Chery_logo.png            ← logo brand (header)
    ├── cars\
    │   ├── c5.png
    │   ├── c5-csh.webp
    │   ├── j6-special-price.png
    │   ├── j6t.png
    │   ├── tiggo-8.png
    │   ├── tiggo-8-csh.png
    │   ├── tiggo-8-alt.png
    │   ├── tiggo-9-csh.png
    │   ├── tiggo-cross.png
    │   ├── tiggo-cross-csh.png
    │   ├── tiggo-cross-sport.png
    │   └── chery-q-prebook.jpg   ← dipakai di promo banner
    ├── customers\
    │   └── customer-1.jpg .. customer-7.jpg
    └── sales\
        └── profile.jpg
```

---

## 12. Quality Checklist

- [x] design.md lengkap
- [x] Color palette terdefinisi dengan role + hex
- [x] Tipografi non-generic (Sora + Manrope)
- [x] 11 section blueprint jelas
- [x] Asset map komplit, semua file path benar
- [x] Decorative menggunakan inline SVG transparan
- [x] Responsive breakpoints terdefinisi
- [x] Accessibility rules ditetapkan
- [x] Motion respects `prefers-reduced-motion`
- [x] CTA pattern konsisten (crimson primary, outline secondary)

---

## 13. Notes for Handoff

- **Nomor WhatsApp** di file HTML saat ini placeholder `6281234567890` — ganti ke nomor WA Nayla sebenarnya (find & replace di seluruh file).
- **Alamat showroom** & **Google Maps embed link** di section #lokasi & footer placeholder — sesuaikan ke alamat showroom Chery Tangerang yang asli (saat ini "Jl. Raya Serpong, Tangerang Selatan").
- **Foto sales** di `assets/sales/profile.jpg` saat ini orientasi portrait, sudah dipakai ratio 4:5 di section profile. Crop ulang jika perlu.
- Foto customer ditampilkan dalam grid 7 foto + 1 stat card. Bila ingin diperluas, tambah file dan tinggal append di `<section id="gallery">`.
- **Sosmed yang sudah dipasang:**
  - Instagram: `@cherypik2_` → https://instagram.com/cherypik2_
  - TikTok: `@nalavyu` → https://tiktok.com/@nalavyu
  - Email: `naylajuliana16@gmail.com`
- **Maps iframe** memakai query string `Chery+Tangerang+Serpong`. Ganti ke koordinat / nama tempat pasti showroom (atau gunakan Google Maps Embed API key untuk styling lebih baik).
