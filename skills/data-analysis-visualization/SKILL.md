---
name: data-analysis-visualization
description: Panduan dan resep analisis data statistik, pemrosesan data ilmiah (Python/R/Excel), serta pembuatan visualisasi grafik/tabel berstandar publikasi jurnal bereputasi (Sinta / Scopus / IEEE / Elsevier / Springer). Gunakan saat pengguna meminta bantuan menganalisis data, memilih uji statistik, membuat grafik/diagram ilmiah, atau menyajikan tabel hasil riset.
---

# Data Analysis & Visualization for Academic Research

Skill ini memberikan panduan komprehensif, pohon keputusan statistik, standar visualisasi publikasi ilmiah (300 DPI, *colorblind-friendly*, format APA/IEEE), serta templat kode (Python/R/Excel) untuk mengolah dan menyajikan data riset secara konsisten.

## When to Use

Gunakan skill ini saat pengguna:

- Meminta rekomendasi pemilihan uji statistik yang tepat berdasarkan hipotesis dan jenis data.
- Meminta kode Python (`matplotlib`, `seaborn`, `scipy`) atau R (`ggplot2`, `tidyverse`) untuk pengolahan data dan visualisasi.
- Ingin membuat grafik, diagram, atau plot berstandar publikasi jurnal internasional/nasional bereputasi.
- Membutuhkan penataan tabel ilmiah sesuai konvensi publikasi (misal: *APA 7th Three-Line Table* atau format IEEE).
- Membutuhkan penafsiran naratif atas hasil analisis statistik (uji hipotesis, *p-value*, *effect size*, *confidence interval*).

---

## Pohon Keputusan Uji Statistik (*Statistical Decision Tree*)

Gunakan matriks ini untuk merekomendasikan uji statistik yang tepat:

| Tujuan Analisis | Jenis Data / Variabel | Uji Parametrik (Normal) | Uji Non-Parametrik (Bebas Asumsi) | Ukuran Efek (*Effect Size*) |
| --- | --- | --- | --- | --- |
| **Beda 2 Kelompok Independen** | Kontinu (2 sampel terpisah) | *Independent Samples t-test* | *Mann-Whitney U test* | Cohen's *d* |
| **Beda 2 Kelompok Berpasangan** | Kontinu (Pre-Post / Berpasangan) | *Paired Samples t-test* | *Wilcoxon Signed-Rank test* | Cohen's *d* / Matched pairs $r$ |
| **Beda > 2 Kelompok Independen** | Kontinu (> 2 sampel terpisah) | *One-Way ANOVA* | *Kruskal-Wallis H test* | Eta-squared ($\eta^2$) / $\omega^2$ |
| **Beda > 2 Kelompok Berulang** | Kontinu (Pengukuran berulang) | *Repeated Measures ANOVA* | *Friedman test* | Partial Eta-squared ($\eta_p^2$) |
| **Hubungan / Korelasi** | 2 Variabel Kontinu | *Pearson Correlation ($r$)* | *Spearman Rank Correlation ($ho$)* | Coefficient of Determination ($R^2$) |
| **Asosiasi / Hubungan Kategorikal**| 2 Variabel Kategorikal | *Chi-Square Test of Independence* | *Fisher's Exact Test* (sampel kecil) | Cramér's $V$ / Odds Ratio |
| **Prediksi / Pemodelan** | Variabel Bebas -> Terikat | *Linear / Multiple Regression* | *Logistic Regression* (Dependent = Binomial) | Adjusted $R^2$ / Odds Ratio |

---

## Standar Visualisasi Publikasi Ilmiah (*Publication Standards*)

### 1. Spesifikasi Teknis Gambar
- **Resolusi**: Minimal **300 DPI** untuk gambar berwarna/grayscale, **600–1200 DPI** untuk *line art*.
- **Format File**: Vektor disukai (`.pdf`, `.svg`, `.eps`) atau raster tanpa kompresi rugi (`.png`, `.tiff`).
- **Dimensi**:
  - *Single column*: Lebar 8–8.5 cm (3.1–3.3 inci).
  - *Double column*: Lebar 16–17.5 cm (6.3–6.9 inci).
- **Tipografi**: Gunakan font *sans-serif* standar (Arial, Helvetica, atau DejaVu Sans). Ukuran font teks pada grafik wajib seimbang dengan teks tubuh naskah (8–10 pt).

### 2. Skema Warna & Aksesibilitas
- **Colorblind-Friendly**: Gunakan palet ramah buta warna seperti *Viridis*, *Plasma*, *Cividis*, atau palet kategorikal *ColorBrewer* (*Set2*, *Dark2*).
- **Pengujian Cetak Grayscale**: Pastikan grafik tetap dapat dibaca dan dibedakan saat dicetak hitam-putih.
- **Hindari**: Jangan gunakan palet *Rainbow / Jet* karena menciptakan distorsi persepsi nilai data.

### 3. Elemen Kelengkapan Grafik
- **Label Sumbu**: Wajib menyertakan nama variabel dan satuan dalam kurung, misal: `Temperature (°C)`, `Time (s)`, `Accuracy (%)`.
- **Batas Kesalahan (*Error Bars*)**: Wajib jelaskan di *caption* apakah *error bar* mewakili *Standard Deviation (SD)*, *Standard Error of the Mean (SEM)*, atau *95% Confidence Interval (CI)*.
- **Legenda**: Letakkan di dalam area plot (bila ada ruang kosong) atau di bagian atas/bawah untuk menghemat ruang kolom.

---

## Konvensi Tabel Ilmiah (*APA 7th Three-Line Table*)

Tabel ilmiah bereputasi **TIDAK BOLEH** menggunakan garis vertikal. Gunakan prinsip *Three-Line Table*:

1. **Garis Top**: Pembatas paling atas tabel.
2. **Garis Header**: Pembatas di bawah baris judul kolom.
3. **Garis Bottom**: Pembatas paling bawah sebelum catatan kaki tabel (*Table Note*).

### Contoh Struktur Tabel APA 7th:

```text
Table 1
Comparison of Model Performance Metrics Across Datasets

-------------------------------------------------------------------------
Dataset        Model A (Mean ± SD)    Model B (Mean ± SD)    p-value
-------------------------------------------------------------------------
Dataset 1      88.45 ± 2.15           93.20 ± 1.80           < .001***
Dataset 2      82.10 ± 3.40           87.55 ± 2.90             .012*
Dataset 3      79.30 ± 4.12           84.15 ± 3.85             .028*
-------------------------------------------------------------------------
Note. N = 150 per dataset. SD = Standard Deviation.
* p < .05. ** p < .01. *** p < .001.
```

---

## Snippet Kode Standar (Python & R)

### Python (`matplotlib` + `seaborn` Publikasi 300 DPI)

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Konfigurasi gaya publikasi
plt.style.use('seaborn-v0_8-paper')
plt.rcParams.update({
    'font.family': 'sans-serif',
    'font.sans-serif': ['Arial', 'DejaVu Sans'],
    'font.size': 9,
    'axes.labelsize': 10,
    'axes.titlesize': 10,
    'xtick.labelsize': 8,
    'ytick.labelsize': 8,
    'legend.fontsize': 8,
    'figure.titlesize': 11
})

# Plotting
fig, ax = plt.subplots(figsize=(3.3, 2.8), dpi=300) # Single column format
sns.barplot(data=df, x='Group', y='Score', palette='viridis', capsize=0.1, err_kws={'linewidth': 1.2}, ax=ax)

ax.set_xlabel('Experimental Group')
ax.set_ylabel('Mean Score (points)')
sns.despine(top=True, right=True) # Hapus bingkai atas & kanan

plt.tight_layout()
plt.savefig('figure1.png', dpi=300, bbox_inches='tight')
plt.savefig('figure1.pdf', format='pdf', bbox_inches='tight') # Format Vektor
plt.show()
```

### R (`ggplot2` Standar Publikasi)

```r
library(ggplot2)
library(viridis)

ggplot(df, aes(x = Group, y = Score, fill = Group)) +
  geom_bar(stat = "summary", fun = "mean", width = 0.6) +
  geom_errorbar(stat = "summary", fun.data = "mean_se", width = 0.2) +
  scale_fill_viridis_d(option = "C") +
  labs(x = "Experimental Group", y = "Mean Score (points)") +
  theme_classic(base_size = 9, base_family = "Arial") +
  theme(
    legend.position = "none",
    axis.text = element_text(color = "black")
  )

ggsave("figure1.pdf", width = 8.5, height = 7, units = "cm", dpi = 300)
```

---

## Resep Prompt Siap Pakai (*Interactive Prompt Templates*)

### Templat 1: Rekomendasi Uji Statistik
> *"Saya memiliki data eksperimen dengan variabel bebas [Nama Variabel] (3 kelompok) dan variabel terikat [Nama Variabel] (skala rasio). Jumlah sampel n = 45. Bantu saya memilih uji statistik yang tepat, uji asumsi yang wajib dilakukan, serta buatkan skrip Python untuk analisisnya."*

### Templat 2: Pembuatan Skrip Visualisasi Python/R 300 DPI
> *"Bantu saya membuat skrip Python (Seaborn/Matplotlib) untuk membuat [Jenis Plot, misal: Grouped Barplot / Scatterplot] berstandar jurnal Scopus. Gunakan palet ramah buta warna (Viridis), sertakan error bars (SD), hilangkan bingkai atas/kanan, dan atur output ke 300 DPI serta format PDF vektor."*

---

## Quality Audit Checklist Sebelum Submit

- [ ] Uji asumsi (normalitas, homogenitas varians) telah dilakukan sebelum memilih uji parametrik.
- [ ] *p-value* dilaporkan secara tepat (misal: *p* = .023 atau *p* < .001) beserta nilai *effect size* (Cohen's *d*, $\eta^2$).
- [ ] Grafik memiliki resolusi minimal 300 DPI atau berformat vektor (`.pdf`/`.svg`).
- [ ] Label sumbu menyertakan nama variabel dan satuan yang eksplisit.
- [ ] Palet warna dapat dibedakan oleh penderita buta warna dan tetap jelas jika dicetak hitam-putih.
- [ ] Tabel menggunakan format *Three-Line Table* tanpa garis vertikal.

---

## Gotchas & Perangkap Kritis

- **Memotong Sumbu Y secara Menyesatkan (*Truncated Y-Axis*)**: Pada grafik batang (*bar chart*), sumbu Y **wajib** dimulai dari angka 0 untuk mencegah distorsi visual skala perbedaan.
- **Hanya Melaporkan p-value Tanpa Effect Size**: Nilai *p-value* hanya menunjukkan signifikansi statistik, bukan besarnya dampak praktis. Selalu sertakan *effect size*.
- **Visualisasi 3D yang Unnecessary**: Grafik 3D (seperti *3D pie chart* atau *3D bar chart*) menyulitkan pembacaan data secara presisi dan dilarang pada mayoritas jurnal bereputasi.
