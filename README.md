# 🚀 Gemini AI Custom Skills Collection

Repositori ini berisi kumpulan **custom skills** terstruktur yang siap digunakan oleh AI Agent (seperti Gemini Spark) untuk meningkatkan kapabilitas dalam analisis ilmiah, evaluasi kritis, dan penulisan karya tulis akademik bereputasi.

---

## 📂 Struktur Repositori

```text
gemini-skills-repository/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
└── skills/
    ├── critical-thinking-advisor/
    │   └── SKILL.md
    ├── journal-article-rd-dbr/
    │   └── SKILL.md
    ├── journal-article-slr/
    │   └── SKILL.md
    └── journal-reviewer-sinta/
        └── SKILL.md
```

---

## 🛠️ Ringkasan Skill

Berikut adalah daftar skill yang terdapat dalam repositori ini:

### 1. 🧠 `critical-thinking-advisor`
* **Deskripsi**: Kerangka berpikir kritis analitis, anti-sycophancy (tanpa pujian kosong), Socratic questioning, serta evaluasi multi-perspektif.
* **Penggunaan**: Cocok untuk meninjau ide, analisis *pre-mortem*, pengujian strategi, *red-teaming*, dan validasi logika.

### 2. 📑 `journal-article-rd-dbr`
* **Deskripsi**: Panduan komprehensif, kerangka evaluasi, dan templat prompt penulisan artikel jurnal berbasis **Research & Development (R&D)**, **Design and Development Research (DDR)**, **Design Science Research (DSR)**, dan **Design-Based Research (DBR)**.
* **Penggunaan**: Digunakan saat menyusun, merevisi, atau menganalisis naskah jurnal penelitian pengembangan dan ilmu desain (Sinta 1-3 & Scopus).

### 3. 🔍 `journal-article-slr`
* **Deskripsi**: Panduan dan protokol penulisan artikel jurnal **Systematic Literature Review (SLR)** sesuai standar **PRISMA 2020** dan protokol **Kitchenham (2007)**.
* **Penggunaan**: Membantu perumusan *Research Questions* (PICOC/PICOS), kriteria inklusi/eksklusi, diagram alir PRISMA, *Quality Assessment*, dan ekstraksi *research gaps*.

### 4. 📝 `journal-reviewer-sinta`
* **Deskripsi**: Evaluasi dan *peer-review* kritis, objektif, dan realistis untuk draf naskah jurnal terakreditasi **Sinta 1–4** dan **Scopus**.
* **Penggunaan**: Memberikan masukan dari sudut pandang reviewer profesional untuk menguji kesiapan publikasi naskah.

---

## 📥 Cara Penggunaan & Impor

1. **Clone Repositori**:
   ```bash
   git clone https://github.com/username/gemini-skills-repository.git
   ```
2. **Impor Skill**:
   Setiap folder di dalam `skills/` berisi file `SKILL.md` yang dapat diimpor atau diunggah ke sistem AI Agent sesuai konvensi manajemen skill agent yang digunakan.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Silakan lihat file [LICENSE](LICENSE) untuk informasi lebih lanjut.
