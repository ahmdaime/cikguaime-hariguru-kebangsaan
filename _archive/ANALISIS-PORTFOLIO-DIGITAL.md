# ANALISIS PORTFOLIO DIGITAL - cikguaime.vercel.app

**Sumber:** Kod sumber di `F:\Koleksi Coding\portfolio-cikguaime`
**Guru:** Ahmad Aiman Bin Mohamed (Cikgu Aiman / Cikgu Aime)
**Sekolah:** SK Putrajaya Presint 5(1)

---

## GAMBARAN KESELURUHAN

Portfolio digital ini adalah laman web profesional yang dibina sendiri oleh Cikgu Aiman menggunakan teknologi moden. Ia berfungsi sebagai:
1. **Showcase profesional** — Untuk pencalonan anugerah pendidikan
2. **Hub pengedaran alat pendidikan** — 10,700+ guru pengguna
3. **Platform perkhidmatan** — Auto eRPH (perkhidmatan berbayar)
4. **Platform kandungan** — Blog, tutorial, sumber pembelajaran

---

## TEKNOLOGI YANG DIGUNAKAN

| Komponen | Teknologi |
|----------|-----------|
| Framework | React 19.2 + TypeScript 5.8 |
| Bundler | Vite 6.2 |
| Styling | Tailwind CSS 3.4 |
| Animasi | Framer Motion 12.23 |
| Routing | React Router DOM 7.10 |
| Database | Supabase 2.90 |
| AI Chatbot | Google Gemini 1.5 Flash API |
| Borang | Formspree |
| Hosting | Vercel (serverless) |
| Ikon | Lucide React |
| Analitik | Google Analytics 4 |

**Saiz Kod:** ~3,500+ baris TypeScript/React merentas 50+ fail komponen

---

## STRUKTUR LAMAN WEB (4 Halaman Utama)

### 1. Homepage
- Hero Section dengan animated counters
- About (profil dengan badges: 3+ Extensions, 10K+ Users, TOP 150 CJD)
- Services (perkhidmatan pengajaran & inovasi digital)
- Featured Innovation
- Showcase Projek (3 projek utama)
- Student Innovations (7 alat pembelajaran)
- Blog (3 artikel)
- Media Content (YouTube & TikTok)
- Journey 2025 (anugerah & pencapaian)
- Testimonial Carousel (10+ ulasan)
- Contact Form
- Buy Me Coffee Widget (Ko-fi)

### 2. Auto eRPH Page
- Landing page perkhidmatan automasi RPH (Rancangan Pelajaran Harian)
- Harga: RM80 asas + RM80 slot tambahan
- Borang pesanan dengan muat naik bukti pembayaran
- Pengurusan slot melalui Supabase
- Demo video, FAQ, dokumentasi

### 3. Extensions Landing Page
- Showcase penuh 3 Chrome extensions
- Problem statement, demo, bukti impak
- Statistik impak, polisi privasi, FAQ
- Butang muat turun ke Chrome Web Store

### 4. Extensions Coming Soon
- Halaman teaser untuk bukan ahli (access control via sessionStorage)

---

## INOVASI DIGITAL UTAMA

### A. Chrome Extensions (3 aktif, 10,700+ pengguna keseluruhan)

#### 1. IDME PBD Helper
- **Pengguna:** 3,000+ guru
- **Rating:** 5.0/5 (Chrome Web Store)
- **Fungsi:** Automasi pengisian data Pentaksiran Bilik Darjah (PBD) dalam sistem IDME
- **Impak:** Menjimatkan jam kerja mengisi ratusan rekod murid

#### 2. MOIES Kehadiran Helper
- **Pengguna:** 3,000+ guru
- **Rating:** 5.0/5
- **Fungsi:** Automasi penandaan kehadiran dalam sistem MOIES
- **Impak:** Isi kehadiran 40 murid dalam <1 minit (berbanding 10-15 minit manual)

#### 3. PBD OnePage
- **Pengguna:** 4,000+ guru
- **Rating:** 5.0/5
- **Fungsi:** Tukar laporan PBD berbilang halaman kepada satu halaman
- **Impak:** Jimat 80% kertas (5-6 halaman → 1 halaman)

### B. Auto eRPH (Google Apps Script)
- **Jenis:** Perkhidmatan automasi custom
- **Fungsi:** Automasi penulisan RPH dalam Google Sheets
- **Pelanggan:** 50+ guru
- **Harga:** RM80 + RM80/slot tambahan
- **Status:** Aktif, projek utama

### C. TVPSS Booking System
- **Jenis:** Aplikasi web
- **Fungsi:** Sistem tempahan studio dan peralatan TVPSS
- **Ciri:** Tempahan studio, sewaan peralatan, dashboard admin, pengesanan konflik

### D. Inovasi Pembelajaran Murid (7 alat)

| # | Nama | Fungsi |
|---|------|--------|
| 1 | Relief Activity Hub | Permainan/kuiz interaktif untuk waktu relief |
| 2 | AI Tutor Sejarah Tahun 6 | GPT custom dilatih dengan kurikulum Sejarah |
| 3 | Bank Soalan UASA | Bank soalan peperiksaan (2,000+ percubaan) |
| 4 | Panduan Kerja Kursus | Panduan kerja kursus (200,000+ tontonan - viral) |
| 5 | Kuiz PSV Interaktif | Kuiz Pendidikan Seni Visual |
| 6 | Kuiz Sejarah Tahun 6 | Kuiz ulangkaji Sejarah Tahun 6 |
| 7 | Kuiz Sejarah Tahun 5 | Kuiz latihan Sejarah Tahun 5 |

---

## STATISTIK IMPAK (dari data laman web)

| Metrik | Nilai |
|--------|-------|
| Jumlah pengguna extensions | 10,700+ guru |
| Rating purata Chrome Store | 5.0 / 5 |
| Extensions aktif | 3 |
| Pelanggan Auto eRPH | 50+ |
| Testimoni terkumpul | 10+ ulasan 5 bintang |

---

## TESTIMONI (Sampel dari data laman web)

Semua extensions menerima ulasan 5 bintang daripada guru-guru yang memuji:
- Penjimatan masa (10x lebih pantas untuk sesetengah tugas)
- Pengurangan beban pentadbiran
- Pemasangan mudah dan mesra pengguna
- Peningkatan ketara dalam aliran kerja

---

## CIRI TEKNIKAL LANJUTAN

### Prestasi & SEO
- **Code splitting** — Lazy-loaded pages & components (React.lazy)
- **Imej optimum** — Format WebP, responsive srcset, LazyImage dengan Intersection Observer
- **Critical CSS** — Inline above-the-fold styles
- **Font optimization** — Preconnect, font-display: swap
- **Caching** — 1 tahun immutable cache untuk aset statik
- **Structured Data (JSON-LD)** — Person, WebSite, SoftwareApplication, ItemList schema
- **Meta Tags** — Open Graph, Twitter Cards, geo-targeting (MY)

### Keselamatan
- X-Content-Type-Options: nosniff
- X-Frame-Options: DENY
- XSS Protection
- Content Security Policy (CSP)
- Permissions-Policy (block camera, microphone, geolocation)

### Aksesibiliti
- Skip Link untuk navigasi papan kekunci
- HTML semantik dengan hierarki heading
- Focus states yang jelas
- WCAG AA compliant

### Integrasi AI
- Chatbot berkuasa Gemini 1.5 Flash
- Rate limiting: 10 request/minit per IP
- System prompt dalam Bahasa Melayu
- Respons dihadkan kepada 500 token

---

## PEMERHATIAN UTAMA UNTUK PENILAIAN

1. **Kemahiran teknikal tinggi** — Portfolio dibina sendiri menggunakan React 19 (versi terkini), TypeScript, dan infrastruktur moden. Ini bukan template — ia ditulis sepenuhnya dari awal.

2. **Impak nyata terhadap profesion perguruan** — 10,700+ guru Malaysia menggunakan alat yang dicipta, menjimatkan masa pentadbiran secara signifikan.

3. **Inovasi berterusan** — Bukan sahaja membina alat, tetapi menyelenggara, mengemas kini, dan menyokong pengguna secara aktif.

4. **Pendekatan "Cikgu Siang Hari, Vibe Coder Malam Hari"** — Tagline portfolio menggambarkan dualiti peranan: guru sepenuh masa pada siang hari, pembangun perisian pada waktu malam.

5. **Model perniagaan pendidikan** — Auto eRPH menunjukkan keupayaan mencipta perkhidmatan berbayar yang bernilai untuk guru-guru.

6. **Perkongsian percuma** — 3 Chrome extensions diberikan percuma kepada 10,700+ guru, menunjukkan semangat perkongsian ilmu.

7. **Kemahiran menyeluruh** — Menguasai frontend (React), backend (Supabase, serverless), AI (Gemini), SEO, aksesibiliti, dan keselamatan web dalam satu projek.

---

## STRUKTUR FAIL UTAMA

```
portfolio-cikguaime/
├── App.tsx                    # Routing utama
├── index.tsx                  # Entry point
├── constants.tsx              # Data utama (extensions, statistik)
├── types.ts                   # TypeScript interfaces
├── index.html                 # SEO, meta tags, structured data
├── components/
│   ├── Hero.tsx, About.tsx, Services.tsx, Showcase.tsx
│   ├── Blog.tsx, Footer.tsx, Contact.tsx, Navbar.tsx
│   ├── Testimonials.tsx, Journey.tsx, MediaContent.tsx
│   ├── ScrollReveal.tsx, LazyImage.tsx, ErrorBoundary.tsx
│   ├── extensions/            # 14 komponen Extensions page
│   ├── showcase/              # 4 komponen kad projek
│   ├── auto-erph/             # 6 komponen Auto eRPH page
│   └── ui/                    # Komponen UI generik
├── pages/
│   ├── HomePage.tsx
│   ├── AutoErphPage.tsx
│   ├── ExtensionsLanding.tsx
│   └── ExtensionsComingSoon.tsx
├── data/
│   ├── evidence.ts            # Statistik impak & testimoni
│   ├── extensions.ts          # Definisi extensions
│   └── journey2025.ts         # Anugerah & pencapaian
├── hooks/                     # 4 custom React hooks
├── api/chat.ts                # Serverless AI chatbot
├── public/images/             # 17 imej WebP optimum
├── vite.config.ts, tailwind.config.js, vercel.json
└── package.json
```
