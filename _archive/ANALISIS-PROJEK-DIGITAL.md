# ANALISIS PROJEK DIGITAL - Inovasi untuk Guru & Murid

**Pembangun:** Ahmad Aiman Bin Mohamed (Cikgu Aiman / Cikgu Aime)
**Sekolah:** SK Putrajaya Presint 5(1)
**Sumber:** Kod sumber di `F:\Koleksi Coding`

---

## RINGKASAN KESELURUHAN

| # | Projek | Sasaran | Platform |
|---|--------|---------|----------|
| 1 | IDME PBD Helper | Guru | Chrome Extension |
| 2 | MOIES Kehadiran Helper | Guru | Chrome Extension |
| 3 | PBD OnePage | Guru | Chrome Extension |
| 4 | Apps Script RPH Helper (Auto eRPH) | Guru | Google Apps Script |
| 5 | Nexus Admin Dashboard | Pentadbir/Pembangun | Web App (Vite) |
| 6 | Landing Page MOIES | Guru (pemasaran) | Web App (React) |
| 7 | CikguAime Platform | Guru & Murid | Web App + Apps Script |
| 8 | Sistem Perekodan PBD Sahsiah | Guru, Ibu Bapa | Web App (Next.js) |
| 9 | Web App Headcount | Guru & Pentadbir | Web App (Next.js + Python) |
| 10 | Relief Activity Hub | Guru & Murid | Web App (React) |
| 11 | Buku Tulis Digital | Guru & Murid | Standalone HTML |

**Jumlah projek:** 11 projek digital
**Pengguna keseluruhan:** 10,700+ guru (Chrome extensions sahaja)

---

## PROJEK UNTUK GURU (Automasi & Produktiviti)

### 1. IDME PBD Helper (Chrome Extension)
- **Versi:** v3.9.0 | **Pengguna:** 3,000+ guru | **Rating:** 5.0/5
- **Fungsi:** Automasi pengisian data Pentaksiran Bilik Darjah (PBD) dalam sistem IDME KPM
- **Masalah diselesaikan:** Guru perlu isi borang PBD untuk 30+ murid satu per satu secara manual
- **Impak:** Proses 30 minit dikurangkan kepada 2-5 minit
- **Ciri utama:**
  - Pilihan TP (Tahap Penguasaan 1-6) secara pukal
  - Auto Usaha Murid berdasarkan TP
  - Auto Ulasan Guru
  - Sokongan Kemahiran Bahasa (BM/BI)
  - PRO: Cadangan TP pintar berdasarkan markah peperiksaan
- **Model:** Freemium (Percuma + PRO RM10/bulan)

### 2. MOIES Kehadiran Helper (Chrome Extension)
- **Versi:** v1.4.0 | **Pengguna:** 3,000+ guru | **Rating:** 5.0/5
- **Fungsi:** Automasi rekod kehadiran murid dalam sistem MOIES KPM
- **Masalah diselesaikan:** Guru perlu isi kehadiran 30-40 murid secara manual setiap hari
- **Impak:** Proses 30-40 minit dikurangkan kepada 2-3 minit
- **Ciri utama:**
  - Parse mesej WhatsApp ibu bapa secara automatik
  - Padanan nama pintar (fuzzy matching untuk typo)
  - Pengkategorian sebab ketidakhadiran automatik (98 kod KPM)
  - PRO: AI Gemini untuk ketepatan ~100%
  - Pemprosesan 100% tempatan (tiada data murid dihantar ke server)
- **Model:** Freemium (Percuma + PRO RM10/60 hari)

### 3. PBD OnePage (Chrome Extension)
- **Versi:** v2.0 | **Pengguna:** 4,000+ guru | **Rating:** 5.0/5
- **Fungsi:** Tukar laporan PBD berbilang halaman kepada satu halaman untuk cetakan
- **Masalah diselesaikan:** Slip PBD memerlukan 5-6 halaman per murid — membazir kertas dan masa
- **Impak:** Jimat 80% kertas (5-6 halaman → 1 halaman)
- **Ciri utama:**
  - Sokongan Slip PBD dan Slip Kemahiran
  - Pilihan orientasi (Landscape/Portrait)
  - Pratetap konfigurasi (Ultra Compact, Standard, Professional)
  - Tandatangan digital (Guru Kelas & Guru Besar)
  - Pengesanan jenis halaman automatik
- **Model:** Percuma

### 4. Apps Script RPH Helper / Auto eRPH (Google Apps Script)
- **Versi:** v2.6.1-stable | **Pelanggan:** 50+ guru
- **Fungsi:** Automasi penulisan RPH (Rancangan Pelajaran Harian) dalam Google Sheets
- **Masalah diselesaikan:** Guru habiskan 10+ minit per RPH untuk copy-paste dan format
- **Impak:** 10 minit → 2 minit per RPH (80% pengurangan); 70+ jam dijimatkan setahun per guru
- **Ciri utama:**
  - Parsing pintar objektif dan aktiviti
  - Sistem template tanpa had per subjek
  - Navigasi multi-sheet (ISNIN-JUMAAT / AHAD-KHAMIS)
  - Penjejak kemajuan mingguan
  - Pangkalan data DSKP (56,813+ entri kurikulum)
  - Pengekstrakan dokumen Word melalui AI Gemini
- **Model:** RM80 asas + RM80/slot tambahan
- **Variasi:** Versi asas, versi pelanggan individu, versi KPM rasmi

### 5. Sistem Perekodan PBD Sahsiah (Web App — Next.js)
- **Fungsi:** Sistem pengurusan rekod PBD dan sahsiah murid untuk guru
- **Sasaran:** Guru kelas, ibu bapa, pentadbir sekolah
- **Ciri utama:**
  - **Modul PBD:** Rekod pencapaian subjek (BM, Sejarah, PSV) mengikut TP 1-6
  - **Modul Token Sahsiah:** Sistem token tingkah laku (+1/+3/+5 positif, tolak negatif)
  - **Modul Bukti PSV:** Pengurusan tugasan dan bukti PSV
  - **Portal Ibu Bapa:** Papan pendahulu token, akses rekod anak (dilindungi kata laluan)
  - **Panel Admin:** Togol keterlihatan PBD, reset data pukal
  - Eksport ke Excel
- **Teknologi:** Next.js 14, React 18, TypeScript, Supabase, Zustand

### 6. Web App Headcount (Web App — Next.js + Python)
- **Fungsi:** Alat pemindahan markah murid dari fail CSV/Excel ke fail Headcount sedia ada
- **Sasaran:** Guru dan pentadbir sekolah yang urus rekod markah peperiksaan
- **Masalah diselesaikan:** Proses manual memindahkan markah UASA/PBD ke fail Headcount
- **Ciri utama:**
  - Aliran kerja 5 langkah (wizard)
  - Padanan nama pintar (fuzzy matching dengan skor keyakinan)
  - Sokongan UASA (peratusan) dan PBD (tahap penguasaan)
  - Pratonton perubahan sebelum eksport
  - Format asal fail Excel dikekalkan 100%
  - Pemprosesan di pelayar (privasi terjamin)
- **Teknologi:** Next.js (frontend), Python API (backend pemprosesan Excel)

### 7. Nexus Admin Dashboard (Web App — Vite)
- **Fungsi:** Dashboard pentadbiran untuk pengurusan lesen semua produk digital
- **Sasaran:** Pembangun (Cikgu Aiman sendiri) sebagai alat dalaman
- **Ciri utama:**
  - Penjanaan dan pengurusan kunci lesen
  - Sokongan pelbagai produk (IDME, MOEIS, RPH, RPH-AI, Custom)
  - Penjejak status lesen (aktif, tersedia, tamat, dibatalkan)
  - Pengurusan senarai putih peranti
  - Eksport data ke CSV
  - Panel pembelian dan transaksi
- **Teknologi:** Vite, Vanilla JS, Alpine.js, Tailwind CSS, Supabase

### 8. Landing Page MOIES (Web App — React)
- **Fungsi:** Laman pemasaran untuk extension MOIES Kehadiran Helper
- **Sasaran:** Guru-guru Malaysia yang berpotensi menjadi pengguna
- **Ciri utama:**
  - Penerangan masalah dan penyelesaian
  - Demo ciri percuma vs PRO
  - Testimoni pengguna
  - Harga dan FAQ
  - Integrasi pembayaran
- **Teknologi:** React 19, TypeScript, Vite, Framer Motion, Tailwind CSS

---

## PROJEK UNTUK GURU & MURID (Pembelajaran & Bilik Darjah)

### 9. CikguAime Platform (Web + Google Apps Script)
- **Fungsi:** Platform pendidikan menyeluruh dan sistem perniagaan lesen
- **Sasaran:** Guru (alat produktiviti), Murid (kuiz interaktif)
- **Ciri utama:**
  - **Kuiz Interaktif Murid:** Sejarah (Tahun 5 & 6), PSV, soal jawab seret-dan-lepas
  - **Sistem Lesen IDME PRO:** Pengurusan lesen premium (RM10/bulan)
  - **Automasi Pembelian:** Penjanaan kunci lesen automatik, e-mel automatik, muat naik resit ke Drive
  - Perlindungan keselamatan (pengesanan DevTools, penjejak peranti)
- **Teknologi:** HTML/CSS/JS, Google Apps Script, Google Drive, Gmail

### 10. Relief Activity Hub (Web App — React)
- **Fungsi:** Platform permainan interaktif untuk kelas ganti (relief)
- **Sasaran:** Guru relief dan murid sekolah rendah
- **Masalah diselesaikan:** Guru relief sering tiada aktiviti terancang untuk murid
- **Ciri utama:**
  - **6 mod permainan:** Simpulan Bahasa, Peribahasa, Math Quick Fire, Sains Benar/Palsu, Susun Huruf, Teka Negara
  - Pertandingan berpasukan (Lelaki vs Perempuan) dengan skor langsung
  - 3 tahap kesukaran (Mudah, Sederhana, Mencabar)
  - Penjejak sesi dan sejarah permainan
  - Reka bentuk optimum untuk projektor bilik darjah
  - Reset automatik setiap hari
- **Liputan subjek:** Bahasa Melayu, Matematik, Sains, Bahasa Inggeris, Geografi
- **Teknologi:** React 19, TypeScript, Vite, Tailwind CSS

### 11. Buku Tulis Digital (Standalone HTML)
- **Fungsi:** Aplikasi buku tulis dan lukisan digital berasaskan web
- **Sasaran:** Guru dan murid untuk nota dan aktiviti bilik darjah
- **Ciri utama:**
  - **Alat lukisan:** Pen, pemadam, bentuk (segi empat, bulatan, anak panah, garisan)
  - **Teks kaya:** Saiz fon 8-200px, bold, warna tersuai
  - **Jadual:** Cipta, gabung/pisah sel, tambah baris/lajur
  - **Berbilang halaman:** Cipta, navigasi, padam halaman
  - **4 templat halaman:** Bergaris, 4 bahagian, berpetak, kosong
  - **Saiz halaman:** A4, A5, saiz tersuai
  - **Pemasa:** Kira detik untuk aktiviti bermasa
  - **Mod persembahan:** Skrin penuh tanpa toolbar
  - **Import imej** dan simpan sebagai gambar
  - **Pintasan papan kekunci** (P, T, B, J, E, F, C, G, Ctrl+S)
- **Saiz fail:** 212KB sahaja — satu fail HTML, tiada pergantungan luaran
- **Teknologi:** HTML5 Canvas, CSS, JavaScript (vanilla)

---

## ANALISIS IMPAK KESELURUHAN

### Impak terhadap Guru

| Aspek | Impak |
|-------|-------|
| **Penjimatan masa** | PBD: 30 min → 2 min, Kehadiran: 40 min → 3 min, RPH: 10 min → 2 min, Headcount: jam → minit |
| **Penjimatan kertas** | PBD OnePage: 80% pengurangan kertas cetakan |
| **Pengurangan kesilapan** | Automasi menghapus kesilapan kemasukan data manual |
| **Kebolehcapaian** | Chrome extensions — pasang dan guna serta-merta |
| **Jangkauan** | 10,700+ guru pengguna merentas seluruh Malaysia |

### Impak terhadap Murid

| Aspek | Impak |
|-------|-------|
| **Pembelajaran interaktif** | Relief Activity Hub, Kuiz Sejarah/PSV, Buku Tulis Digital |
| **Penilaian sahsiah** | Sistem Token PBD Sahsiah dengan portal ibu bapa |
| **Kemahiran digital** | Pendedahan kepada alat digital dalam pembelajaran |

### Impak terhadap Sistem Pendidikan

| Aspek | Impak |
|-------|-------|
| **Sistem KPM** | Integrasi terus dengan IDME, MOIES, ISSPPB (portal rasmi KPM) |
| **Standard** | Menyokong format RPH rasmi KPM dan DSKP (56,813 entri) |
| **Privasi** | Pemprosesan data tempatan — tiada data murid dihantar ke server luar |
| **Kos** | Majoriti alat percuma atau sangat murah (RM10/bulan) |

---

## EKOSISTEM PRODUK

```
EKOSISTEM CIKGUAIME
│
├── CHROME EXTENSIONS (3 produk, 10,700+ pengguna)
│   ├── IDME PBD Helper ──── automasi PBD
│   ├── MOIES Kehadiran Helper ──── automasi kehadiran
│   └── PBD OnePage ──── jimat kertas cetakan
│
├── GOOGLE APPS SCRIPT (1 produk, 50+ pelanggan)
│   └── Auto eRPH ──── automasi RPH
│
├── WEB APPS (5 produk)
│   ├── Sistem PBD Sahsiah ──── rekod PBD + tingkah laku
│   ├── Web App Headcount ──── pemindahan markah
│   ├── Relief Activity Hub ──── aktiviti kelas ganti
│   ├── CikguAime Platform ──── kuiz murid + lesen
│   └── Buku Tulis Digital ──── buku tulis digital
│
├── INFRASTRUKTUR DALAMAN (2 produk)
│   ├── Nexus Admin Dashboard ──── pengurusan lesen
│   └── Landing Page MOIES ──── pemasaran
│
└── PORTFOLIO (sudah didokumentasikan berasingan)
    └── portfolio-cikguaime ──── laman web profesional
```

---

## TEKNOLOGI YANG DIKUASAI

| Kategori | Teknologi |
|----------|-----------|
| Frontend | React 19, Next.js 14, TypeScript, Tailwind CSS, Framer Motion, Alpine.js |
| Backend | Google Apps Script, Python, Vercel Serverless, Supabase |
| Extension | Chrome Manifest V3, Chrome Storage API, Content Scripts |
| AI | Google Gemini API (parsing dokumen & pengkategorian) |
| Database | Supabase (PostgreSQL), Google Sheets, localStorage |
| Build | Vite, esbuild |
| Lain-lain | HTML5 Canvas, SEO, JSON-LD, Excel/CSV processing |
