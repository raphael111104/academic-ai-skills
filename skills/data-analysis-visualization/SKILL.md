---
name: data-analysis-visualization
description: Statistical test selection decision trees, statistical assumption workflows, effect size benchmarks, research data processing (Python/R/Excel), and publication-ready data visualization guidelines (300 DPI, vector formats, APA 7th three-line tables). Use when the user requests help selecting statistical tests, creating scientific charts, or formatting data tables.
---

# Data Analysis & Visualization for Academic Research

Provides comprehensive statistical decision trees, assumption testing workflows, effect size benchmarks, publication-grade data visualization standards (300 DPI, colorblind-friendly, APA/IEEE formats), and code generation templates (Python, R, Excel).

## When to Use

Use this skill when the user:
- Requests recommendations for appropriate statistical tests based on research hypotheses and data types.
- Needs assumption testing workflows (normality, homogeneity of variance, multicollinearity, sphericity).
- Requires Python (`matplotlib`, `seaborn`, `scipy.stats`, `statsmodels`) or R (`ggplot2`, `tidyverse`, `rstatix`) code for data processing and plotting.
- Wants to create publication-grade charts, plots, or diagrams for international and national journals.
- Requires formatting of scientific tables according to journal conventions (e.g., APA 7th Three-Line Table, IEEE format).

---

## Comprehensive Statistical Decision Tree

| Analysis Goal | Data Type / Variables | Parametric Test (Normal Data) | Non-Parametric Test (Non-Normal) | Effect Size Metric & Benchmarks |
| --- | --- | --- | --- | --- |
| **Compare 2 Independent Groups** | Continuous DV, 2 Independent Groups | *Independent Samples t-test* | *Mann-Whitney U test* | Cohen's *d* (0.2 Small, 0.5 Med, 0.8 Large) |
| **Compare 2 Paired Groups** | Continuous DV, Pre-Post / Paired | *Paired Samples t-test* | *Wilcoxon Signed-Rank test* | Matched Pairs *r* (0.1 Small, 0.3 Med, 0.5 Large) |
| **Compare > 2 Independent Groups**| Continuous DV, > 2 Independent Groups | *One-Way ANOVA* | *Kruskal-Wallis H test* | Eta-squared $\eta^2$ (0.01 Small, 0.06 Med, 0.14 Large) |
| **Compare > 2 Repeated Groups** | Continuous DV, Repeated Measures | *Repeated Measures ANOVA* | *Friedman test* | Kendall's *W* (0.1 Small, 0.3 Med, 0.5 Large) |
| **Correlation / Association** | 2 Continuous Variables | *Pearson Correlation (r)* | *Spearman Rank Correlation ($\rho$)* | $R^2$ Coefficient of Determination |
| **Categorical Association** | 2 Categorical Variables | *Chi-Square Test ($\chi^2$)* | *Fisher's Exact Test* (n < 5 per cell) | Cramér's *V* (0.1 Small, 0.3 Med, 0.5 Large) |
| **Prediction / Regression** | Continuous DV, Continuous/Cat IVs | *Multiple Linear Regression* | *Ordinal / Logistic Regression* | Adjusted $R^2$ / Odds Ratio (OR) |

---

## Statistical Assumption Testing Protocols

Prior to executing parametric tests, verify required assumptions:

1. **Normality**:
   - *Test*: Shapiro-Wilk test (n < 50) or Kolmogorov-Smirnov test (n $\ge$ 50).
   - *Rule*: If *p* > .05, normality is met. If *p* < .05, use non-parametric alternative or log transformation.
2. **Homogeneity of Variance**:
   - *Test*: Levene's Test or Bartlett's Test.
   - *Rule*: If *p* > .05, equal variances assumed. If *p* < .05, use Welch's *t*-test or Welch's ANOVA.
3. **Multicollinearity (Regression)**:
   - *Test*: Variance Inflation Factor (VIF).
   - *Rule*: VIF < 5 is acceptable; VIF > 10 indicates severe multicollinearity requiring variable removal/PCA.

---

## Publication Visualization Standards

### 1. Image Specifications
- **Resolution**: Minimum **300 DPI** for raster (`.png`, `.tiff`); vector format preferred (`.pdf`, `.svg`, `.eps`).
- **Dimensions**: Single-column (8.0–8.5 cm) or Double-column (16.0–17.5 cm).
- **Typography**: Sans-serif fonts (Arial, Helvetica, DejaVu Sans). Font size: 8–10 pt.

### 2. Color Palettes & Accessibility
- **Colorblind-Friendly**: Use *Viridis*, *Plasma*, *Cividis*, or *ColorBrewer* palettes (`Set2`, `Dark2`).
- **Grayscale Compatibility**: Ensure distinct line styles (solid, dashed, dotted) and marker shapes (circle, square, triangle) so charts remain legible in black-and-white print.

---

## APA 7th Three-Line Table Standard

Scientific tables **MUST NOT** include vertical lines. Use three horizontal lines: Top, Header, and Bottom.

```text
Table 1
ANOVA Results and Effect Sizes for Learning Outcomes Across Experimental Groups

----------------------------------------------------------------------------------
Group             n       Mean     SD       F (2, 147)    p-value    Eta-sq (η²)
----------------------------------------------------------------------------------
Control           50      72.40    6.15     14.82         < .001***  0.168
Treatment A       50      79.85    5.40
Treatment B       50      84.10    4.95
----------------------------------------------------------------------------------
Note. N = 150. SD = Standard Deviation. η² = Eta-squared (Large effect).
* p < .05. ** p < .01. *** p < .001.
```

---

## Publication Code Snippets (Python & R)

### Python (`matplotlib` + `seaborn` 300 DPI Vector)

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Set publication style
plt.style.use('seaborn-v0_8-paper')
plt.rcParams.update({
    'font.family': 'sans-serif',
    'font.sans-serif': ['Arial', 'DejaVu Sans'],
    'font.size': 9,
    'axes.labelsize': 10,
    'xtick.labelsize': 8,
    'ytick.labelsize': 8,
    'legend.fontsize': 8
})

fig, ax = plt.subplots(figsize=(3.3, 2.8), dpi=300)
sns.barplot(data=df, x='Group', y='Score', palette='viridis', capsize=0.1, ax=ax)

ax.set_xlabel('Experimental Group')
ax.set_ylabel('Mean Score (points)')
sns.despine(top=True, right=True)

plt.tight_layout()
plt.savefig('figure1.png', dpi=300, bbox_inches='tight')
plt.savefig('figure1.pdf', format='pdf', bbox_inches='tight') # Vector
plt.show()
```

---

## Interactive Prompt Templates

### Template 1: Assumption Check & Test Selection
> *"I have experimental data comparing 3 groups (n = 25 per group) on a continuous dependent variable. Provide a Python script to test normality (Shapiro-Wilk) and homogeneity of variance (Levene's test), and automatically run either ANOVA or Kruskal-Wallis with effect size calculation."*

### Template 2: Publication Plot Generation
> *"Provide a complete Python script to generate a 300 DPI vector plot (PDF and PNG) comparing 2 conditions across 4 time points. Use colorblind-friendly colors (Viridis), error bars (SEM), dashed vs solid lines, and APA 7th formatting."*

---

## Critical Gotchas

- **Truncated Y-Axis on Bar Charts**: Y-axis on bar charts MUST start at 0 to avoid visual distortion.
- **Omitting Effect Sizes**: Reporting *p-values* without effect sizes ($\eta^2$, Cohen's *d*) fails to convey practical significance.
