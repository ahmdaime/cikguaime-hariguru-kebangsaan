# NOTA SESI CLAUDE — Portfolio Anugerah Hari Guru Kebangsaan 2026

**Tarikh terakhir dikemas kini:** 28 Januari 2026
**Deadline:** 9 Februari 2026
**Kategori:** Anugerah Khas Pencipta Kandungan Digital
**Calon:** Ahmad Aiman Bin Mohamed (Cikgu Aime), SK Putrajaya Presint 5(1)
**Repo:** git@github.com:ahmdaime/cikguaime-hariguru-kebangsaan.git

---

## STATUS SEMASA

### Siap
- [x] Semua kandungan 6 bahagian lengkap (40 halaman)
- [x] Data dikemas kini ke angka terkini (27 Jan 2026)
- [x] Font dinaikkan ke saiz profesional (minimum 8pt, body 10pt)
- [x] Penulisan diperbaiki (buang corak AI, tatabahasa BM betul)
- [x] 8 gambar dimasukkan (profil, 3 CWS, 4 extension interface)
- [x] CSS gambar diperbaiki (max-height 55mm dalam grid)

### Belum Siap
- [ ] **Gambar baki (~21 gambar)** — senarai penuh di bawah
- [ ] **Fasa layout/print** — auto-split overflow, renumber halaman, kemas kedudukan
- [ ] **Kemas kini TOC** — selepas layout fix, nombor halaman akan berubah
- [ ] **Sync index.html** — `cp portfolio/portfolio.html index.html` selepas setiap perubahan

---

## STRUKTUR PORTFOLIO (40 halaman)

| # | Bahagian | Halaman | Kandungan |
|---|----------|---------|-----------|
| - | Cover | 0 | Muka depan dengan foto profil |
| - | TOC | 1 | Isi kandungan |
| 01 | Profil & Biodata | ms 2–3 | Maklumat peribadi, kemahiran, peranan |
| 02 | Katalog Kandungan Digital | ms 4–19 | 330+ kandungan, kajian kes mendalam |
| 03 | Demo & Bukti Kualiti | ms 20–22 | Rating, testimoni, tangkap layar, senarai semak |
| 04 | Sumbangan & Impak | ms 23–34 | Impak guru/murid, TVPSS, perkongsian ilmu, timeline, analitik |
| 05 | Sijil & Pencapaian | ms 35–38 | 76 pencapaian, sijil terpilih |
| 06 | Etika & Privasi Digital | ms 39 | Privasi, hak cipta, keselamatan |

---

## FAIL UTAMA

- `portfolio/portfolio.html` — Fail utama portfolio (satu fail HTML dengan CSS inline)
- `index.html` — Salinan untuk GitHub Pages (MESTI sync selepas setiap perubahan)
- `portfolio/img/` — Folder gambar

---

## DATA TERKINI (27 Jan 2026)

| Metrik | Nilai |
|--------|-------|
| Episod TVPSS | 108 |
| Livestream | 14 |
| YouTube subscribers | 3,600 |
| TikTok TVPSS FiveOne | 15,400 followers, 130 video |
| TikTok @ahmdaime | 40,000 followers |
| Facebook | 8,800 followers |
| Chrome Extensions total | 14,900+ (MOEIS 5,770 / IDME 4,592 / PBD 4,565) |
| Blog pelawat | 3,545,773 |
| Blog bulanan | ~100,000 |
| Jumlah kandungan | 330+ |
| Jumlah video | 252 |
| Total capaian digital | ~4.5 Juta |
| MOEIS rating | 4.96/5 |
| IDME & PBD rating | 5.0/5 |

---

## GAMBAR YANG SUDAH ADA (portfolio/img/)

| Fail | Keterangan |
|------|------------|
| profil.jpg | Foto profil muka depan |
| cws-idme.png | Chrome Web Store — IDME PBD Helper |
| cws-moeis.png | Chrome Web Store — MOEIS Kehadiran |
| cws-pbd.png | Chrome Web Store — PBD OnePage |
| ext-idme.png | Antaramuka IDME PBD Helper |
| ext-moeis.png | Antaramuka MOEIS Kehadiran |
| ext-pbd.png | Antaramuka PBD OnePage |
| ext-erph.png | Antaramuka Auto eRPH |

## GAMBAR YANG MASIH DIPERLUKAN

### Analytics (4 gambar)
| Fail | Keterangan |
|------|------------|
| analytics-blog.png | Google Analytics cikguaime.com (3.5M pelawat) |
| analytics-yt.png | YouTube Analytics TVPSS FiveOne |
| analytics-tt.png | TikTok Analytics |
| yt-channel.png | YouTube channel page (3,600 subscribers) |

### Sijil (6 gambar)
| Fail | Keterangan |
|------|------------|
| sijil-johan-kebangsaan.jpg | Johan Kebangsaan TVPSS 2024 |
| sijil-johan-negeri.jpg | Johan Negeri TVPSS |
| sijil-cjd.jpg | Sijil Cikgu Juara Digital TOP 150 |
| sijil-edufluencer.jpg | Sijil Edufluencer KPM |
| sijil-google.jpg | Sijil Google Certified Educator |
| sijil-lain.jpg | Sijil pencapaian lain |

### Studio & Aktiviti (4 gambar)
| Fail | Keterangan |
|------|------------|
| studio-setup.jpg | Setup studio TVPSS FiveOne |
| studio-murid.jpg | Murid sedang rakam/sunting |
| foto-sharing.jpg | Sesi perkongsian ilmu |
| sijil-juri.jpg | Sijil pelantikan juri |

### Aplikasi & Blog (4 gambar)
| Fail | Keterangan |
|------|------------|
| app-relief.png | Relief Activity Hub |
| app-buku.png | Buku Tulis Digital |
| app-sahsiah.png | Sistem PBD Sahsiah |
| blog-utama.png | Halaman utama cikguaime.com |

### Video (3 gambar)
| Fail | Keterangan |
|------|------------|
| blog-artikel.png | Artikel popular cikguaime.com |
| yt-episod.png | Senarai episod YouTube |
| yt-johan.png | Bukti Johan (berita SinarBestari) |
| kuiz.png | Tangkap layar kuiz interaktif |

---

## LANGKAH SETERUSNYA (IKUT TURUTAN)

### 1. Masukkan baki gambar
- User simpan gambar ke `portfolio/img/` dengan nama yang ditetapkan
- Claude link gambar ke placeholder dalam HTML
- Commit setiap batch

### 2. Fasa layout/print fix
- Buka portfolio di browser dengan Playwright
- Ukur setiap halaman: `scrollHeight` vs A4 height (1122.52px)
- Auto-split halaman yang overflow (pindah elemen terakhir ke halaman sambungan)
- Pastikan tiada halaman terlalu kosong (min 35% terisi)
- Renumber semua halaman

### 3. Kemas kini TOC
- Selepas layout fix, nombor halaman akan berubah
- Kemas kini semua ms X–Y dalam TOC
- Kemas kini sub-references (kajian kes, dll)

### 4. Semakan akhir
- Print preview dalam browser (Ctrl+P)
- Pastikan tiada teks terpotong
- Pastikan semua gambar nampak
- Sync index.html dan push

---

## NOTA TEKNIKAL

- **A4 height dalam pixel:** 297 × (96/25.4) ≈ 1122.52px
- **CSS page system:** `.page` divs dengan `width: 210mm; min-height: 297mm`
- **Print CSS:** `page-break-after: always` pada `.page`
- **Tema warna:** Biru gelap (#0a1628) + Emas (#c8a84e)
- **Font minimum:** 8pt (labels), 9pt (secondary), 10pt (body text)
- **Local server:** `npx serve -l 3847 .` dari root folder
- **`:has()` CSS selector** digunakan untuk style placeholder yang ada gambar
