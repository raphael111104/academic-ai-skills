# Academic & Critical AI Agent Skills Repository

Repositori ini berisi kumpulan *Custom Agent Skills* yang dirancang khusus untuk memandu AI Agent (seperti Gemini, Claude, atau ChatGPT) dalam membantu penulisan ilmiah, penyuntingan naskah akademis, *Systematic Literature Review* (SLR), penelitian pengembangan (R&D/DDR/DSR/DBR), *peer review* jurnal bereputasi (Sinta 1-4 & Scopus), serta analisis berpikir kritis.

---

## 📁 Struktur Repositori

```
academic-ai-skills/
├── README.md                           # Dokumentasi utama repositori
├── CONTRIBUTING.md                     # Panduan kontribusi repositori
├── LICENSE                             # Lisensi terbuka (MIT)
├── .gitignore                          # Daftar file yang diabaikan Git
├── .github/                            # Templat Issue dan Pull Request
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── PULL_REQUEST_TEMPLATE.md
└── skills/                             # Direktori utama AI Skills
    ├── critical-thinking-advisor/      # Skill Penalaran Kritis & Anti-Sycophancy
    ├── journal-article-author-expert/  # Unified Master Skill Penulisan & Review
    ├── journal-article-rd-dbr/         # Skill Artikel R&D, DDR, DSR, dan DBR
    ├── journal-article-slr/            # Skill Artikel SLR (PRISMA 2020 & Kitchenham)
    └── journal-reviewer-sinta/         # Skill Peer Reviewer Standar Sinta 1-4
```

---

## 🛠️ Daftar & Ringkasan Skills

| Nama Skill | Deskripsi & Kegunaan Utama | Target / Standar |
| --- | --- | --- |
| **`journal-article-author-expert`** | **[Unified Master Skill]** Peleburan komprehensif seluruh skill penulisan, SLR, R&D/Desain, *peer review*, dan penalaran kritis. | Sinta 1-4 & Scopus |
| **`critical-thinking-advisor`** | Kerangka kerja penalaran kritis, *constructive pushback*, metode Sokratis, *First Principles*, dan audit 4-aksis. | Evaluasi Umum & Akademis |
| **`journal-article-rd-dbr`** | Panduan penulisan artikel berbasis R&D, DDR, DSR, dan DBR beserta formulasi metrik kuantitatif (V-Aiken, N-Gain, SUS). | Sinta 1-3 & Scopus Q1-Q3 |
| **`journal-article-slr`** | Panduan penyusunan artikel Systematic Literature Review sesuai standar PRISMA 2020 dan protokol Kitchenham. | Sinta 1-3 & Scopus |
| **`journal-reviewer-sinta`** | Panduan *peer review* objektif, jujur, dan ketat untuk naskah jurnal terakreditasi Sinta 1-4. | Akreditasi Sinta 1-4 |

---

## 🚀 Cara Menggunakan di Agent / Workspace

### 1. Mengunggah ke GitHub
1. Unduh file zip repositori ini.
2. Ekstrak dan *push* repositori ini ke akun GitHub Anda:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Academic AI Agent Skills Collection"
   git branch -M main
   git remote add origin https://github.com/USERNAME/academic-ai-skills.git
   git push -u origin main
   ```

### 2. Mengimpor ke AI Environment (Google Gemini / Claude / Custom GPTs)
- **Sistem Agent / Custom Skill Manager**: Salin folder dari direktori `skills/<nama-skill>` ke dalam direktori kerja Agent Anda atau impor melalui *Skills Manager*.
- **Penggunaan Manual**: Buka file `SKILL.md` dari skill yang diinginkan, salin seluruh isinya, dan tempelkan sebagai *System Prompt* atau *Custom Instructions* pada percakapan AI Anda.

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail selengkapnya.
