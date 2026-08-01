---
name: data-analysis-visualization
description: Statistical test selection decision trees, research data processing (Python/R/Excel), and publication-ready data visualization guidelines (300 DPI, vector formats, APA 7th three-line tables). Use when the user requests help selecting statistical tests, creating scientific charts, or formatting data tables.
---

# Data Analysis & Visualization for Academic Research

Provides comprehensive statistical decision trees, research data processing workflows, publication-grade data visualization standards (300 DPI, colorblind-friendly, APA/IEEE formats), and code generation templates (Python, R, Excel).

## When to Use

Use this skill when the user:
- Requests recommendations for appropriate statistical tests based on research hypotheses and data types.
- Needs Python (`matplotlib`, `seaborn`, `scipy.stats`) or R (`ggplot2`, `tidyverse`) code for data processing and visualization.
- Wants to create publication-grade charts, plots, or diagrams for international and national journals.
- Requires formatting of scientific tables according to journal conventions (e.g., APA 7th Three-Line Table, IEEE format).
- Needs narrative interpretation of statistical outputs (*p-values*, effect sizes, confidence intervals, test statistics).

---

## Statistical Decision Tree

Use this decision matrix to recommend appropriate statistical tests:

| Analysis Goal | Data Type / Variables | Parametric Test (Normal) | Non-Parametric Test | Effect Size Metric |
| --- | --- | --- | --- | --- |
| **Compare 2 Independent Groups** | Continuous (2 independent samples) | *Independent Samples t-test* | *Mann-Whitney U test* | Cohen's *d* |
| **Compare 2 Paired Groups** | Continuous (Pre-Post / Paired) | *Paired Samples t-test* | *Wilcoxon Signed-Rank test* | Cohen's *d* / Matched pairs $r$ |
| **Compare > 2 Independent Groups**| Continuous (> 2 independent samples) | *One-Way ANOVA* | *Kruskal-Wallis H test* | Eta-squared ($\eta^2$) / $\omega^2$ |
| **Compare > 2 Repeated Groups** | Continuous (Repeated measures) | *Repeated Measures ANOVA* | *Friedman test* | Partial Eta-squared ($\eta_p^2$) |
| **Correlation / Relationship** | 2 Continuous variables | *Pearson Correlation ($r$)* | *Spearman Rank Correlation ($ho$)* | Coefficient of Determination ($R^2$) |
| **Categorical Association** | 2 Categorical variables | *Chi-Square Test of Independence*| *Fisher's Exact Test* (small sample) | Cramér's $V$ / Odds Ratio |
| **Prediction / Modeling** | Independent -> Dependent | *Linear / Multiple Regression* | *Logistic Regression* (Binomial Y) | Adjusted $R^2$ / Odds Ratio |

---

## Publication Visualization Standards

### 1. Technical Image Specifications
- **Resolution**: Minimum **300 DPI** for color/grayscale raster images; **600–1200 DPI** for line art.
- **File Format**: Preferred vector formats (`.pdf`, `.svg`, `.eps`) or uncompressed raster (`.png`, `.tiff`).
- **Dimensions**:
  - *Single column*: Width 8.0–8.5 cm (3.1–3.3 inches).
  - *Double column*: Width 16.0–17.5 cm (6.3–6.9 inches).
- **Typography**: Standard sans-serif fonts (Arial, Helvetica, or DejaVu Sans). Font size in figures must match body text scale (8–10 pt).

### 2. Color Palettes & Accessibility
- **Colorblind-Friendly**: Use accessible palettes such as *Viridis*, *Plasma*, *Cividis*, or *ColorBrewer* categorical palettes (*Set2*, *Dark2*).
- **Grayscale Print Compatibility**: Ensure figures remain legible and distinguishable when printed in black and white.
- **Avoid Distortion**: Do not use *Rainbow / Jet* palettes due to perceptual distortion of data transitions.

### 3. Figure Elements & Error Bars
- **Axis Labels**: Explicitly include variable name and units in parentheses, e.g., `Temperature (°C)`, `Time (s)`, `Accuracy (%)`.
- **Error Bars**: State clearly in figure captions whether error bars represent *Standard Deviation (SD)*, *Standard Error of the Mean (SEM)*, or *95% Confidence Interval (CI)*.

---

## APA 7th Three-Line Table Format

Academic journal tables MUST NOT include vertical gridlines. Use the *Three-Line Table* rule:

1. **Top Border**: Placed above the column header row.
2. **Header Border**: Placed below the column header row.
3. **Bottom Border**: Placed at the bottom of the table data, above table notes.

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

## Publication Code Snippets (Python & R)

### Python (`matplotlib` + `seaborn` 300 DPI)

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Publication style setup
plt.style.use('seaborn-v0_8-paper')
plt.rcParams.update({
    'font.family': 'sans-serif',
    'font.sans-serif': ['Arial', 'DejaVu Sans'],
    'font.size': 9,
    'axes.labelsize': 10,
    'axes.titlesize': 10,
    'xtick.labelsize': 8,
    'ytick.labelsize': 8,
    'legend.fontsize': 8
})

fig, ax = plt.subplots(figsize=(3.3, 2.8), dpi=300) # Single column size
sns.barplot(data=df, x='Group', y='Score', palette='viridis', capsize=0.1, ax=ax)

ax.set_xlabel('Experimental Group')
ax.set_ylabel('Mean Score (points)')
sns.despine(top=True, right=True)

plt.tight_layout()
plt.savefig('figure1.png', dpi=300, bbox_inches='tight')
plt.savefig('figure1.pdf', format='pdf', bbox_inches='tight') # Vector
plt.show()
```

### R (`ggplot2` Publication Standard)

```r
library(ggplot2)
library(viridis)

ggplot(df, aes(x = Group, y = Score, fill = Group)) +
  geom_bar(stat = "summary", fun = "mean", width = 0.6) +
  geom_errorbar(stat = "summary", fun.data = "mean_se", width = 0.2) +
  scale_fill_viridis_d(option = "C") +
  labs(x = "Experimental Group", y = "Mean Score (points)") +
  theme_classic(base_size = 9, base_family = "Arial") +
  theme(legend.position = "none")

ggsave("figure1.pdf", width = 8.5, height = 7, units = "cm", dpi = 300)
```

---

## Interactive Prompt Templates

### Template 1: Statistical Test Recommendation
> *"I have experimental data with 1 independent variable (3 treatment groups) and 1 continuous dependent variable. Sample size n = 45. Recommend the appropriate statistical test, required assumption checks, and provide a Python script for the analysis."*

### Template 2: 300 DPI Publication Plot Generation
> *"Help me create a Python script using Seaborn to generate a publication-ready grouped barplot. Use a colorblind-friendly palette (Viridis), error bars (SD), remove top/right spines, and output a 300 DPI PNG and vector PDF."*

---

## Pre-Submission Quality Audit Checklist

- [ ] Assumption checks (normality, homogeneity of variance) were conducted prior to parametric testing.
- [ ] Exact *p-values* and effect sizes (Cohen's *d*, $\eta^2$) are reported alongside test statistics.
- [ ] Figures meet 300 DPI minimum resolution or are provided in vector format (`.pdf`/`.svg`).
- [ ] Axis labels explicitly state variable names and units.
- [ ] Tables use the Three-Line format without vertical lines.

---

## Critical Gotchas

- **Truncated Y-Axis on Bar Charts**: Sumbu Y on bar charts MUST start at 0 to prevent visual distortion of differences.
- **Reporting p-values Without Effect Sizes**: A *p-value* indicates statistical significance, not practical effect magnitude. Always report effect sizes.
- **Unnecessary 3D Graphics**: 3D pie or bar charts distort data perception and are prohibited by reputable journals.
