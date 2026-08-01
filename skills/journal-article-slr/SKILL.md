---
name: journal-article-slr
description: Panduan dan resep penulisan artikel jurnal ilmiah berbasis Systematic Literature Review (SLR) menggunakan standar PRISMA 2020 dan Kitchenham. Gunakan saat pengguna meminta bantuan menyusun, menulis, mengedit, atau menganalisis draf artikel jurnal SLR untuk publikasi di jurnal bereputasi (Sinta 1-3 atau Scopus).
---

# journal-article-slr

Skill ini memberikan panduan komprehensif dan terstruktur untuk menyusun, menulis, mengevaluasi, dan merevisi artikel jurnal ilmiah berbasis Systematic Literature Review (SLR) sesuai standar publikasi bereputasi (Sinta 1-3 dan Scopus) dengan acuan utama PRISMA 2020 (*Preferred Reporting Items for Systematic Reviews and Meta-Analyses*) dan protokol Kitchenham (2007).

## When to Use

Gunakan skill ini saat pengguna:
- Meminta panduan penulisan artikel jurnal Systematic Literature Review (SLR).
- Meminta analisis struktur, evaluasi kritis, atau review draf artikel SLR.
- Membutuhkan penentuan *Research Questions* (RQ), kriteria inklusi/eksklusi, string pencarian Boolean, atau diagram alir PRISMA.
- Ingin menyusun sintesis literatur, *Risk of Bias/Quality Assessment*, *gap analysis*, dan agenda penelitian masa depan berbasis SLR.

---

## Standar Kerangka Kerja SLR

### 1. Protokol Kitchenham (2007)
Terdiri dari 3 fase utama:
- **Planning the Review**: Identifikasi kebutuhan review, pendaftaran protokol (OSF/PROSPERO), formulasi *Research Questions* (RQ), penyusunan kriteria seleksi.
- **Conducting the Review**: Strategi pencarian literatur (Boolean string), seleksi studi (inklusi/eksklusi), evaluasi *Risk of Bias* & *Quality Assessment*, ekstraksi data, dan sintesis data.
- **Reporting the Review**: Penulisan artikel ilmiah, penyusunan lampiran/PRISMA checklist, dan diseminasi hasil.

### 2. Panduan PRISMA 2020
Mewajibkan alur seleksi literatur yang transparan dan *replicable* melalui 4 tahapan utama pada *PRISMA 2020 Flowchart*:
1. **Identification**: Rekaman yang ditemukan dari database akademik utama (Scopus, IEEE Xplore, ScienceDirect, Web of Science, SpringerLink, PubMed) dan sumber lain, beserta penghapusan duplikasi (*deduplication*).
2. **Screening**: Penyaringan judul dan abstrak berdasarkan kriteria kelayakan awal.
3. **Eligibility**: Penilaian kelayakan teks lengkap (*full-text review*) berdasarkan kriteria inklusi & eksklusi secara spesifik beserta alasan eksklusi artikel teks lengkap.
4. **Included**: Jumlah studi primer akhir yang dimasukkan dalam sintesis (*primary studies*).

---

## Formulasi Pertanyaan Penelitian (PICOC / PICOS)

Gunakan kerangka PICOC / PICOS untuk menyusun *Research Questions* (RQ) yang terarah:

- **P (Population / Problem)**: Subjek atau domain fokus (misal: Siswa SMA, UMKM, Software Developers, Patient Care).
- **I (Intervention / Topic)**: Teknologi, pendekatan, atau metode yang diterapkan (misal: AI-Tutoring, Gamifikasi, Agile Methodology).
- **C (Comparison / Control)**: Pembanding jika ada (misal: Pembelajaran Tradisional, Metode Non-AI).
- **O (Outcome)**: Hasil yang diukur (misal: Hasil Belajar Kognitif, Efisiensi Operasional, Kepuasan Pengguna).
- **C/S (Context / Study Design)**: Lingkungan riset, konteks industri, atau desain studi yang ditinjau.

**Contoh Struktur RQ**:
- **RQ1 (Tren & Bibliometrik)**: Bagaimana tren volume publikasi, distribusi geografis, dan sumber terbitan dari tahun Y hingga Z?
- **RQ2 (Metodologi & Teknik)**: Metode, algoritma, atau instrumen apa yang paling dominan digunakan dalam studi primer?
- **RQ3 (Temuan & Dampak)**: Apa saja temuan kunci dan dampak penerapan X terhadap O?
- **RQ4 (Tantangan & Future Agenda)**: Apa tantangan utama, *limitations*, dan kesenjangan penelitian (*research gaps*) untuk arah penelitian mendatang?

---

## Panduan Penulisan Bagian demi Bagian

### 1. Judul & Abstrak
- **Judul**: Wajib mencantumkan frasa "Systematic Literature Review" atau "SLR". Contoh: *"Systematic Literature Review: Adopsi Artificial Intelligence dalam Pendidikan Dasar (2020-2025)"*.
- **Abstrak (150-250 kata)**: Berisi latar belakang singkat, tujuan SLR, database yang digunakan, periode tahun, jumlah artikel akhir yang diulas (*n = X artikel*), hasil sintesis utama sesuai RQ, serta implikasi/kesimpulan utama.

### 2. Pendahuluan (Introduction)
- Paragraf 1: Latar belakang, konteks, dan urgensi topik.
- Paragraf 2: Rasionalkan mengapa Systematic Review diperlukan (dibandingkan review tradisional/naratif).
- Paragraf 3: Kebaruan (*Novelty*) & Perbandingan dengan SLR Terdahulu (jelaskan perbedaan fokus/rentang waktu dengan SLR yang sudah ada).
- Paragraf 4: Tujuan penelitian dan daftar eksplisit *Research Questions* (RQ1 - RQ4).

### 3. Metode Penelitian (Methodology)
Tuliskan metode secara rinci agar memenuhi prinsip *replicability*:

- **3.1 Protocol & Registration**: Sebutkan apakah protokol SLR didaftarkan di registri publik (misal: OSF / PROSPERO) atau jelaskan kepatuhan pada PRISMA 2020.
- **3.2 Search Strategy & String Query**:
  - Sebutkan database spesifik (misal: Scopus, Web of Science, IEEE Xplore, ScienceDirect).
  - Sertakan rumus string pencarian Boolean lengkap dengan operator (`AND`, `OR`, `NOT`, wildcards `*`). Contoh: `("Systematic Literature Review" OR "SLR") AND ("AI in Education" OR "Intelligent Tutoring")`.
- **3.3 Inclusion & Exclusion Criteria**:
  - Tampilkan tabel kriteria inklusi dan eksklusi secara eksplisit (bahasa, rentang tahun, tipe dokumen, *peer-reviewed status*, ketersediaan *full-text*).
- **3.4 Selection Process & PRISMA Flowchart**:
  - Sajikan diagram alir *PRISMA 2020 Flowchart*. Sertakan jumlah penilai (*reviewers*) dan mekanisme resolusi ketidaksepakatan (misal: *inter-rater reliability* / diskusi dengan penilai ketiga).
- **3.5 Risk of Bias & Quality Assessment (QA)**:
  - Berikan 3-5 kriteria penilaian kualitas metodologi dan *risk of bias* (misal: kejelasan tujuan, kelayakan desain, reliabilitas analisis data).
  - Tentukan sistem skoring (misal: Ya=1, Sebagian=0.5, Tidak=0) dan ambang batas kelayakan studi.
- **3.6 Data Extraction & Synthesis Methods**:
  - Uraikan matriks ekstraksi data (penulis, tahun, negara, metode, variabel, temuan utama).
  - Jelaskan teknik sintesis data: sintesis kualitatif/tematik (misal: *Thematic Analysis* Braun & Clarke) atau sintesis kuantitatif/deskriptif.
- **3.7 Transparency on AI Tool Usage**:
  - Ungkapkan secara jujur jika ada penggunaan perangkat lunak atau *AI-assisted tools* (misal: Rayyan, Covidence, ChatGPT/Claude untuk ekstraksi/klasifikasi) sesuai regulasi etika penerbit.

### 4. Hasil dan Analisis (Results & Analysis)
Strukturkan bagian hasil secara logis mengikuti urutan *Research Questions* (RQ):

- **Pemetaan Studi Primer (Overview)**: Ringkasan karakteristik umum (tren tahunan, peta geografis, jenis jurnal). Bila relevan, kombinasikan dengan analisis peta ko-oksistensi kata kunci / pemetaan bibliometrik.
- **Jawaban RQ1 - RQ4**: Sajikan analisis tematik dan taksonomi yang menjawab masing-masing RQ didukung oleh tabel sintesis, diagram, atau matriks perbandingan dari *primary studies*.

### 5. Pembahasan (Discussion)
- **Sintesis Temuan Utama**: Intepretasikan hasil SLR dan hubungkan dengan teori atau kerangka kerja utama di bidang terkait.
- **Theoretical & Practical Implications**: Jelaskan bagaimana temuan SLR berkontribusi pada pengembangan teori dan praktik profesional.
- **Research Gaps & Future Research Framework**: Petakan secara sistematis celah penelitian (*knowledge gaps*) dan formulasikan *Research Roadmap* / rekomendasi konkret bagi peneliti mendatang.
- **Limitations of the Review**: Ungkapkan keterbatasan SLR secara terbuka (misal: pembatasan bahasa, keterbatasan akses database, atau potensi bias publikasi).

### 6. Kesimpulan (Conclusion)
- Sajikan kesimpulan padat yang menjawab seluruh RQ secara lugas tanpa mengulang abstrak secara harfiah.
- Tekankan kontribusi/nilai tambah ilmiah (*value-added*) dari SLR ini bagi komunitas akademis.

---

## Quality Checklist untuk Publikasi Sinta 1-3 / Scopus

- [ ] Judul memuat frasa "Systematic Literature Review" atau "SLR".
- [ ] Pertanyaan penelitian (*Research Questions*) dirumuskan secara terukur (minimal 3-4 RQ) menggunakan PICOC/PICOS.
- [ ] Pendaftaran protokol atau acuan PRISMA 2020 disebutkan secara eksplisit.
- [ ] Database akademik bereputasi (Scopus, WoS, IEEE, ScienceDirect, dll.) disebutkan beserta string pencarian Boolean yang dapat direplikasi.
- [ ] Kriteria inklusi dan eksklusi tersaji rinci dalam tabel.
- [ ] Terdapat diagram alir *PRISMA 2020 Flowchart* lengkap dengan alasan eksklusi *full-text*.
- [ ] Penilaian *Risk of Bias* / *Quality Assessment* (QA) dilakukan dengan kriteria dan kualifikasi terukur.
- [ ] Terdapat kejelasan jumlah penilai dan resolusi ketidaksepakatan (*inter-rater agreement*).
- [ ] Tabel ekstraksi data studi primer (*Primary Studies*) terstruktur rapi.
- [ ] Penggunaan perangkat AI/automasi (jika ada) diungkapkan secara transparan.
- [ ] Bagian Pembahasan menghasilkan *Research Gaps* dan *Future Research Roadmap* yang konkret.

---

## Gotchas & Reviewer Red Flags

- **Menyamakan SLR dengan Review Naratif Biasa**: SLR wajib transparan, terstruktur, berbasis string pencarian eksplisit, dan dapat direplikasi (*replicable*).
- **Hanya Mengandalkan Google Scholar**: Reviewer Sinta 1-3 dan Scopus kerap menolak SLR yang hanya menggunakan Google Scholar tanpa menyaring kualitas database utama (Scopus, WoS, IEEE, ScienceDirect, Springer, PubMed).
- **Tidak Menyajikan Diagram PRISMA 2020**: Kelalaian menyertakan diagram PRISMA adalah penyebab utama *desk rejection* pada tahap awal penerimaan naskah.
- **Tidak Ada Sintesis (Hanya Summarizing/Copy-Paste Abstrak)**: Hasil SLR bukan sekadar rangkuman paragraf demi paragraf dari naskah lain, melainkan sintesis tematik, pemetaan taksonomi, dan analisis kritis yang menjawab RQ.
- **Tidak Mengukur Risk of Bias / Quality Assessment**: Menganggap semua artikel yang lolos pencarian memiliki kualitas setara tanpa ada penyaringan QA/RoB.
- **Ketiadaan Future Research Agenda**: SLR tanpa kerangka/arah penelitian masa depan dianggap kurang berbobot oleh reviewer jurnal bertaraf internasional/bereputasi.
