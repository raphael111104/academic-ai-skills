# 🚀 Universal AI Agent Skills Collection

Repositori ini berisi kumpulan **custom skills** terstruktur yang dirancang secara universal untuk meningkatkan kapabilitas **AI Agent** dalam analisis ilmiah, berpikir kritis, pengolahan data, dan penulisan karya tulis akademik bereputasi.

> ℹ️ **Catatan Kompatibilitas**:  
> Seluruh skill dalam repositori ini dirancang secara **universal** sehingga dapat digunakan oleh berbagai sistem dan kerangka kerja AI Agent modern yang mendukung instruksi kustom terstruktur (seperti Claude, ChatGPT Custom Agents/Instructions, AutoGPT, dan framework agentik lainnya). **Secara khusus, seluruh skill dalam repositori ini aktif digunakan dan dioptimalkan oleh penulis pada platform Gemini Spark.**

---

## 📂 Struktur Repositori

```text
academic-ai-skills/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
└── skills/
    ├── academic-proofreader-translator/
    │   └── SKILL.md
    ├── critical-thinking-advisor/
    │   └── SKILL.md
    ├── data-analysis-visualization/
    │   └── SKILL.md
    ├── journal-article-rd-dbr/
    │   └── SKILL.md
    ├── journal-article-slr/
    │   └── SKILL.md
    ├── journal-reviewer-sinta/
    │   └── SKILL.md
    └── reference-manager-bibtex/
        └── SKILL.md
```

---

## 🛠️ Matriks & Ringkasan Ekosistem Skill

Berikut adalah katalog lengkap dari 7 *custom skills* yang terdapat di dalam repositori ini:

| No | Nama Skill | Domain Fokus | Fungsi Utama |
| --- | --- | --- | --- |
| 1 | `academic-proofreader-translator` | Bahasa & Polishing | Penerjemahan presisi ID <-> EN akademis, perbaikan grammar, penyesuaian AWL, dan kalibrasi *hedging*. |
| 2 | `critical-thinking-advisor` | Logika & Evaluasi | Analisis kritis anti-sycophancy, Socratic questioning, *pre-mortem analysis*, dan pengujian asumsi. |
| 3 | `data-analysis-visualization` | Statistik & Visualisasi | Pohon keputusan uji statistik, pembuatan skrip grafik 300 DPI/vektor, dan format *APA 3-Line Table*. |
| 4 | `journal-article-rd-dbr` | Metodologi Riset | Panduan penulisan naskah penelitian pengembangan & ilmu desain (R&D, DDR, DSR, DBR). |
| 5 | `journal-article-slr` | Tinjauan Literatur | Protokol penulisan Systematic Literature Review (SLR) sesuai standar PRISMA 2020 & Kitchenham. |
| 6 | `journal-reviewer-sinta` | Peer Review | Penelaahan naskah ilmiah kritis dan objektif dari sudut pandang reviewer Sinta 1–4 & Scopus. |
| 7 | `reference-manager-bibtex` | Sitasi & Bibliografi | Pemformatan file BibTeX/RIS, konversi gaya sitasi (APA 7th, IEEE, Vancouver), dan deteksi sitasi gantung. |

---

## 📖 Deskripsi Rinci per Skill

### 1. 🌐 `academic-proofreader-translator`
* **Fungsi**: Membantu menyunting tata bahasa (*proofreading*), menerjemahkan draf naskah ilmiah Bahasa Indonesia ke Bahasa Inggris Akademis (*Academic English*), mengeliminasi *wordiness*, serta menyesuaikan *hedging* ilmiah.

### 2. 🧠 `critical-thinking-advisor`
* **Fungsi**: Menyediakan kerangka berpikir kritis analitis tanpa pujian kosong (*anti-sycophancy*), pengujian logika *First Principles*, dan evaluasi strategi secara objektif.

### 3. 📊 `data-analysis-visualization`
* **Fokus**: Merekomendasikan uji statistik yang tepat (parametrik vs non-parametrik), membuat skrip grafik berkualitas publikasi (300 DPI, *colorblind-friendly*, format vektor), serta menyusun tabel tiga garis (*Three-Line Table*).

### 4. 📑 `journal-article-rd-dbr`
* **Fungsi**: Membimbing penyusunan, analisis, dan perbaikan naskah jurnal berbasis metode Research & Development (R&D), Design and Development Research (DDR), Design Science Research (DSR), dan Design-Based Research (DBR).

### 5. 🔍 `journal-article-slr`
* **Fungsi**: Menyediakan protokol komprehensif penulisan artikel Systematic Literature Review (SLR), perumusan *Research Questions* (PICOC), diagram alir PRISMA 2020, dan matriks sintesis literatur.

### 6. 📝 `journal-reviewer-sinta`
* **Fungsi**: Memberikan umpan balik *peer-review* yang ketat, jujur, dan realistis untuk menguji kesiapan publikasi naskah pada jurnal terakreditasi Sinta 1–4 dan Scopus.

### 7. 📚 `reference-manager-bibtex`
* **Fungsi**: Mengelola dan merapikan sintaks file BibTeX/RIS, melakukan konversi gaya sitasi (APA 7th, IEEE, Vancouver, Harvard), memeriksa ketersediaan DOI, serta mendeteksi sitasi gantung (*orphan citations*).

---

## 📥 Cara Penggunaan pada AI Agent

1. **Clone / Download Repositori**:
   ```bash
   git clone https://github.com/username/gemini-skills-repository.git
   ```
2. **Import ke AI Agent**:
   * Setiap direktori di dalam folder `skills/` memuat file `SKILL.md` mandiri.
   * File `SKILL.md` dapat diimpor langsung sebagai *System Prompt*, *Custom Instruction*, atau dimasukkan ke dalam folder skill AI Agent Anda (seperti pada Gemini Spark).

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Silakan lihat file [LICENSE](LICENSE) untuk informasi lebih lanjut.
