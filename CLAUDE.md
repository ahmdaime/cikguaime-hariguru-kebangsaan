# Portfolio Anugerah Hari Guru Kebangsaan 2026

## Projek

Portfolio digital untuk pencalonan **Anugerah Khas Pencipta Kandungan Digital**, Hari Guru Peringkat Kebangsaan 2026. Calon: Ahmad Aiman Bin Mohamed (Cikgu Aime), SK Putrajaya Presint 5(1).

## Status Semasa (4 Feb 2026)

- **Jumlah halaman**: 61
- **Gambar**: 70+ gambar telah dimasukkan
- **Bahagian TVPSS FiveOne**: Lengkap dengan liputan, pertandingan, pencapaian, dan collage

## Struktur Fail

- `portfolio/portfolio.html` — Fail utama portfolio (satu fail HTML + CSS inline, 61 halaman A4)
- `index.html` — Salinan untuk GitHub Pages (MESTI sync selepas setiap perubahan)
- `portfolio/img/` — Semua gambar portfolio

## Struktur Portfolio (61 halaman)

| Bahagian | Halaman | Kandungan |
|----------|---------|-----------|
| Cover & TOC | 0-1 | Muka depan, isi kandungan |
| 01 Profil & Biodata | 2-3 | Maklumat peribadi, kemahiran |
| 02 Katalog Kandungan | 4-35 | Extensions, Apps, TVPSS, Blog |
| 03 Demo & Bukti | 36-40 | Rating, testimoni, tangkap layar |
| 04 Sumbangan & Impak | 41-50 | Impak guru/murid, keberlanjutan |
| 05 Sijil & Pencapaian | 51-57 | 76 pencapaian, sijil |
| 06 Etika & Privasi | 58-61 | Privasi, hak cipta, keselamatan |

## TVPSS FiveOne (ms 22-31)

| Halaman | Kandungan |
|---------|-----------|
| 22-23 | Studio & Pembangunan Kemahiran Murid |
| 24-25 | Behind The Scene |
| 26-27 | Liputan Antarabangsa, Kebangsaan, Negeri (15 gambar) |
| 28 | Penyertaan Pertandingan Video (5 gambar) |
| 29 | Tulang Belakang Sekolah - Collage (26 gambar) |
| 30-31 | Pencapaian & Bukti Gambar |

## Sync index.html

Selepas setiap perubahan pada `portfolio/portfolio.html`, jalankan:

```
node -e "const fs=require('fs');let h=fs.readFileSync('portfolio/portfolio.html','utf8');h=h.replace(/src=\"img\//g,'src=\"portfolio/img/');fs.writeFileSync('index.html',h);"
```

## Spesifikasi Teknikal

- **Format**: HTML5 statik, CSS inline, tiada JavaScript
- **Saiz halaman**: A4 (210mm × 297mm), height ~1122.52px pada 96dpi
- **Sistem halaman**: `.page` divs dengan `page-break-after: always`
- **Had overflow**: `scrollHeight` mesti ≤ 1125px setiap halaman
- **Tema warna**: Biru gelap `#0a1628` + Emas `#c8a84e` (CSS vars: `--primary`, `--accent`)
- **Font**: Segoe UI; minimum 8pt (labels), 9pt (secondary), 10pt (body)
- **Local server**: `npx serve -l 3847 .`

## Semakan Overflow

Selepas setiap edit, buka di browser dan jalankan di console:

```js
document.querySelectorAll('.page').forEach((p, i) => {
  if (p.scrollHeight > 1125) console.log(`Page ${i} OVERFLOW: ${p.scrollHeight}px`);
});
```

## Gaya Penulisan

- Bahasa Melayu formal, sesuai untuk juri
- **JANGAN** guna sempang/dashes dalam ayat
- **JANGAN** guna frasa generik AI ("dengan penuh dedikasi", "secara holistik", dll.)
- **JANGAN** sebut harga/PRO/komersial — fokus pada impak pendidikan percuma
- Tekankan extension hanya mempercepatkan **pengisian borang**, bukan menggantikan **penilaian guru**
- Pemberian TP kekal tanggungjawab guru berdasarkan penilaian berterusan melalui PdP
- **JANGAN** guna emoji bendera negara (🇲🇾) — tidak disokong semua sistem

## Renumber Halaman

Selepas tambah/buang halaman, jalankan untuk renumber:

```
node -e "const fs=require('fs');let h=fs.readFileSync('portfolio/portfolio.html','utf8');const lines=h.split('\n');let p=1;for(let i=0;i<lines.length;i++){if(lines[i].match(/Muka Surat <span>\d+<\/span>/)){lines[i]=lines[i].replace(/Muka Surat <span>\d+<\/span>/,'Muka Surat <span>'+p+'</span>');p++;}}fs.writeFileSync('portfolio/portfolio.html',lines.join('\n'));console.log('Total:',p-1);"
```
