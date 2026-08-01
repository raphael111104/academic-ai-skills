---
name: reference-manager-bibtex
description: Panduan dan resep pengurusan referensi, sitasi, dan file BibTeX/RIS/APA/IEEE untuk karya tulis ilmiah. Gunakan saat pengguna meminta bantuan memformat sitasi, memeriksa metadata DOI, merapikan file BibTeX, mengonversi gaya sitasi (APA 7th, IEEE, Vancouver, Harvard), atau mendeteksi sitasi gantung dan referensi kadaluarsa.
---

# Reference Manager & BibTeX Specialist

Skill ini memberikan panduan komprehensif, standar pemformatan file BibTeX/RIS, verifikasi metadata sitasi (DOI, volume, isu, halaman), konversi gaya sitasi (APA 7th, IEEE, Vancouver, Harvard), serta teknik pemeriksaan sitasi gantung dan kemutakhiran pustaka untuk publikasi ilmiah.

## When to Use

Gunakan skill ini saat pengguna:

- Meminta pembuatan, perapihan, atau validasi sintaks file BibTeX (`.bib`) atau RIS (`.ris`).
- Membutuhkan konversi gaya sitasi antarstandar (misal: dari APA 7th ke IEEE atau sebaliknya).
- Meminta verifikasi kelengkapan metadata referensi (DOI, nama jurnal, nomor volume/isu, rentang halaman).
- Ingin melakukan pemeriksaan konsistensi antara sitasi di dalam teks (*in-text citations*) dan Daftar Pustaka (*References list*).
- Membutuhkan analisis kemutakhiran pustaka (persentase referensi 5–10 tahun terakhir).

---

## Standar Entri & Metadata BibTeX Spesifik

Setiap entri BibTeX wajib memuat atribut utama sesuai tipe dokumen:

### 1. Jurnal ilmiah (`@article`)
```bibtex
@article{Arrasyid2026AI,
  author    = {Arrasyid, Rafli and Pratama, Budi},
  title     = {Implementation of {AI} Agents in Academic Publishing: A Systematic Review},
  journal   = {Journal of Educational Technology and Innovation},
  year      = {2026},
  volume    = {14},
  number    = {2},
  pages     = {105--120},
  doi       = {10.1016/j.jeti.2026.01.005}
}
```

### 2. Prosiding Konferensi (`@inproceedings`)
```bibtex
@inproceedings{Arrasyid2025Design,
  author    = {Arrasyid, Rafli},
  title     = {Designing Gamified Learning Platforms Using {Design-Based Research}},
  booktitle = {Proceedings of the 2025 International Conference on Learning Sciences},
  year      = {2025},
  pages     = {45--52},
  publisher = {IEEE},
  doi       = {10.1109/ICLS54321.2025.101234}
}
```

### 3. Buku & Bab Buku (`@book` & `@incollection`)
```bibtex
@book{Branch2009Instructional,
  author    = {Branch, Robert Maribe},
  title     = {Instructional Design: The {ADDIE} Approach},
  publisher = {Springer},
  address   = {New York, NY},
  year      = {2009},
  doi       = {10.1007/978-0-387-09506-6}
}
```

---

## Aturan Kunci Pemformatan BibTeX Ilmiah

1. **Preservasi Kapitalisasi (*Capital Preservation*)**: Gunakan kurung kurawal `{}` pada kata bersurat kapital khusus, nama diri, akronim, atau nama negara agar tidak diubah menjadi huruf kecil oleh compiler LaTeX (misal: `{AI}`, `{Indonesia}`, `{Sinta}`).
2. **Karakter Khusus LaTeX**: Selalu gunakan *escape character* untuk simbol khusus:
   - `&` -> `\&`
   - `%` -> `\%`
   - `_` -> `\_`
   - `$` -> `\$`
3. **Format Nama Penulis**: Gunakan format `Marga, Nama Depan` atau pisahkan antarpenulis dengan kata kunci `and`:
   - ✅ `author = {Smith, John and Doe, Jane}`
   - ❌ `author = {John Smith, Jane Doe}`
4. **Rentang Halaman**: Gunakan dua tanda hubung (`--`) untuk rentang halaman (misal: `105--120`).

---

## Konversi Gaya Sitasi Utama (*Citation Style Matrix*)

| Parameter | APA 7th Edition | IEEE Style | Vancouver Style | Harvard Style |
| --- | --- | --- | --- | --- |
| **Tipe Sitasi Teks** | Author-Date: `(Arrasyid & Pratama, 2026)` | Angka Siku: `[1]` | Angka Kurung/Superskrip: `(1)` atau `¹` | Author-Date: `(Arrasyid and Pratama 2026)` |
| **Urutan Daftar Pustaka** | Alfabetis nama belakang penulis | Berdasarkan urutan kemunculan di teks | Berdasarkan urutan kemunculan di teks | Alfabetis nama belakang penulis |
| **Nama Penulis** | Marga, Inisial. (`Arrasyid, R.`) | Inisial. Marga (`R. Arrasyid`) | Marga Inisial tanpa titik (`Arrasyid R`) | Marga, Inisial. (`Arrasyid, R.`) |
| **Judul Artikel** | Sentence case (Kapital kata pertama) | Title Case dalam tanda petik `"Implementation..."` | Sentence case | Sentence case dalam tanda petik tunggal |
| **Nama Jurnal** | Italic Title Case (*Journal of Educational...*) | Italic Abbreviated (*J. Educ. Technol.*) | Abbreviated tanpa titik (*J Educ Technol*) | Italic Title Case (*Journal of Educational...*) |
| **Format DOI** | URL Lengkap (`https://doi.org/...`) | Frasa DOI (`doi: 10.1109/...`) | URL atau DOI identifier | URL Lengkap |

---

## Audit Konsistensi Sitasi (*Citation Audit & Quality Control*)

Saat meninjau daftar pustaka karya ilmiah, lakukan 3 tahap verifikasi:

1. **Deteksi Sitasi Gantung (*Orphan Citations*)**:
   - Pastikan setiap rujukan yang ditulis di dalam teks (*in-text*) memiliki entri lengkap di Daftar Pustaka.
   - Pastikan setiap entri di Daftar Pustaka pernah disitasi minimal satu kali di dalam teks.
2. **Uji Kemutakhiran Pustaka (*Currency Ratio*)**:
   - Untuk bidang ilmu dinamis (Teknologi, AI, Pendidikan, Kesehatan), **minimal 80%** dari total pustaka wajib berasal dari terbitan **5–10 tahun terakhir**.
   - Utamakan sumber dari artikel jurnal bereputasi (*primary sources*) daripada buku teks umum atau blog.
3. **Verifikasi Ketersediaan DOI**:
   - Pastikan semua artikel jurnal memiliki nomor DOI yang valid dan dapat diakses.

---

## Resep Prompt Siap Pakai (*Interactive Prompt Templates*)

### Templat 1: Merapikan & Memvalidasi File BibTeX
> *"Berikut adalah daftar entri BibTeX saya. Tolong rapikan sintaksnya, pastikan preservasi kapitalisasi pada akronim/nama diri menggunakan kurung kurawal, perbaiki format nama penulis, dan periksa apakah ada field penting (seperti DOI/volume/pages) yang kurang."*

### Templat 2: Konversi Gaya Sitasi (APA 7th ke IEEE / Vancouver)
> *"Konversikan daftar pustaka berformat APA 7th berikut ke dalam format IEEE. Berikan output berupa: (1) Sitasi Teks berurutan [1], [2], dan (2) Daftar Pustaka IEEE yang telah diurutkan."*

---

## Quality Audit Checklist Sebelum Submit

- [ ] Sintaks BibTeX bebas dari kesalahan *missing brace* `{}` atau *missing comma* `,`.
- [ ] Akronim dan nama diri pada judul artikel BibTeX telah diikat kurung kurawal `{}`.
- [ ] Nama penulis ditulis konsisten menggunakan `Marga, Nama Depan` dan dipisahkan kata `and`.
- [ ] Karakter khusus (`&`, `%`, `_`) telah di-*escape* dengan benar.
- [ ] Tidak ada sitasi gantung (*orphan citations*) antara teks dan daftar pustaka.
- [ ] Lebih dari 80% pustaka berasal dari artikel jurnal bereputasi 5–10 tahun terakhir.
