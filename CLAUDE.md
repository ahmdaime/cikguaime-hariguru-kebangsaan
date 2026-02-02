# Portfolio Anugerah Hari Guru Kebangsaan 2026

## Projek

Portfolio digital untuk pencalonan **Anugerah Khas Pencipta Kandungan Digital**, Hari Guru Peringkat Kebangsaan 2026. Calon: Ahmad Aiman Bin Mohamed (Cikgu Aime), SK Putrajaya Presint 5(1).

## Struktur Fail

- `portfolio/portfolio.html` — Fail utama portfolio (satu fail HTML + CSS inline, ~40 halaman A4)
- `index.html` — Salinan untuk GitHub Pages (MESTI sync selepas setiap perubahan)
- `portfolio/img/` — Semua gambar portfolio
- `CLAUDE-SESSION-NOTES.md` — Nota sesi, status, dan senarai gambar yang diperlukan

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

Selepas setiap edit, buka di Playwright dan jalankan:

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
