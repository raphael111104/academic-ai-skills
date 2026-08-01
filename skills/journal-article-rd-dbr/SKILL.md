---
name: journal-article-rd-dbr
description: Comprehensive guidelines, evaluation frameworks, and prompt recipes for writing, editing, and reviewing journal articles using Research & Development (R&D), Design and Development Research (DDR), Design Science Research (DSR), and Design-Based Research (DBR) methodologies. Use when working on development or design science paper drafts for Sinta and Scopus journals.
---

# Journal Article Writing: R&D, DDR, DSR, and DBR Methodologies

Provides comprehensive guidelines, evaluation frameworks, validation formulas, and prompt recipes for structuring, writing, editing, and reviewing research articles targeting accredited national (Sinta 1–4) and international (Scopus/WoS) journals using development and design methodologies: **Research & Development (R&D)**, **Design and Development Research (DDR)**, **Design Science Research (DSR)**, and **Design-Based Research (DBR)**.

## When to Use

Use this skill when the user:
- Requests guidelines, templates, or structure for paper drafts based on R&D, DDR, DSR, or DBR.
- Needs evaluation metrics (Aiken's V, Gregory's Agreement, N-Gain, SUS, Cohen's d), instrument validation formulas, or phrasing examples.
- Wants guidance choosing between R&D, DDR, DSR, and DBR for a specific research problem.
- Requires review, critique, or revision of a development or design science paper draft.

---

## Deep Methodology Comparison Matrix

| Parameter | Research & Development (R&D) | Design and Development Research (DDR) | Design Science Research (DSR) | Design-Based Research (DBR) |
| --- | --- | --- | --- | --- |
| **Primary Focus** | Developing & testing the effectiveness of educational products/media | Systematic study of designing, developing, & evaluating products or design models | Developing innovative artifacts to solve technical or Information System problems | Iteratively improving real-world learning practices in authentic classroom/learning settings |
| **Foundational References** | Borg & Gall (1983), Thiagarajan (4D, 1974), ADDIE (Branch, 2009) | Richey & Klein (2007), Ellis & Levy (2010) | Hevner et al. (2004), Peffers et al. DSRM (2007) | McKenney & Reeves (2012/2019), DBR Collective (2003) |
| **Core Output** | Valid, practical, & effective product | Product/tool (Type 1) or validated design model (Type 2) | Artifact (software, algorithm, architecture) + Knowledge Base contribution | Practical intervention + Design Principles (CERA framework) |
| **Evaluation Metrics**| Aiken's V, Gregory Index, SUS, N-Gain Score, Cohen's d | Usability testing, Expert review, Formative & Summative evaluation | Demonstration, Empirical evaluation, Utility & Performance tests | Formative evaluation, Field observation, Iterative cycle reflections |

---

## Key Formulas & Quantitative Evaluation Metrics

### 1. Aiken's V Content Validity Index
Evaluates expert agreement on instrument/product items:
$$V = \frac{\sum s}{n(c - 1)}$$
- Where $s = r - l_o$ ($r$ = expert rating score, $l_o$ = lowest possible rating score).
- $n$ = number of experts/validators.
- $c$ = number of rating scale categories (e.g., 5 for a 1–5 Likert scale).
- **Threshold**: Item is valid if $V \ge 0.80$ (for 3–5 experts).

### 2. Normalized Gain ($N\text{-Gain}$) Score
Measures effectiveness pre- and post-implementation:
$$N\text{-Gain} = \frac{S_{\text{post}} - S_{\text{pre}}}{S_{\text{max}} - S_{\text{pre}}}$$
- **Interpretation Benchmarks**:
  - $N\text{-Gain} > 0.70$: High Effectiveness.
  - $0.30 \le N\text{-Gain} \le 0.70$: Medium Effectiveness.
  - $N\text{-Gain} < 0.30$: Low Effectiveness.

### 3. System Usability Scale (SUS)
Evaluates product practicality/usability (10 items, 5-point scale):
- **Scoring**: For odd items, subtract 1 from score ($r - 1$). For even items, subtract score from 5 ($5 - r$). Sum all scores and multiply by 2.5.
- **Benchmark**: SUS score $> 68$ is considered above average (acceptable usability).

---

## Methodology-Specific Structural Patterns

### 1. Research & Development (R&D) - 4D / ADDIE
- **Define**: Front-end analysis, learner analysis, task analysis, concept analysis, specifying objectives.
- **Design**: Criterion-test construction, media selection, format selection, initial prototype design.
- **Develop**: Expert validation (Aiken's V), developmental testing, revisions, main field testing ($N\text{-Gain}$).
- **Disseminate**: Final packaging, adoption, and dissemination.

### 2. Design Science Research (DSR) - Peffers DSRM
- **6 Steps**: Problem Identification -> Objectives of Solution -> Design & Development -> Demonstration -> Evaluation -> Communication.
- **3-Cycle Model (Hevner)**:
  - *Relevance Cycle*: Environmental context, business needs, acceptance criteria.
  - *Rigor Cycle*: Grounding in kernel theories, scientific foundations, contribution to knowledge base.
  - *Design Cycle*: Iterative building and testing of instantiations.

### 3. Design-Based Research (DBR) - McKenney & Reeves
- **Structure**: Analysis & Exploration -> Design & Construction -> Evaluation & Reflection.
- **Design Principles Extraction (CERA Framework)**:
  *“To design [Artifact X] for [Goal Y] in [Context Z], you should [Action A], because [Theoretical Reason B].”*

---

## Interactive Prompt Templates

### Template 1: Drafting Methodology with Aiken's V & N-Gain
> *"Help me draft the Methodology section for a Scopus Q2 journal using the 4D R&D model. The product is [Specify Product]. Include expert validation procedures using Aiken's V (4 validators) and field testing using Normalized Gain (N-Gain) with pre-post test design."*

### Template 2: Extracting Design Principles (DBR)
> *"Based on the attached iterative evaluation results of my educational intervention across 2 cycles, help me extract 3 formal Design Principles using the CERA framework (Context, Action, Result, Reason)."*

---

## Pre-Submission Quality Audit Checklist

- [ ] Development model is explicitly cited with foundational references (e.g., Thiagarajan, Peffers, McKenney).
- [ ] Quantitative expert validation data (Aiken's V $\ge$ 0.80) reported with exact validator profiles.
- [ ] Field trial effectiveness reported with exact statistical metrics ($N\text{-Gain}$, Effect Size, $t$-test).
- [ ] Visual evidence of artifact iterations, screenshots, or system architecture included.
- [ ] Discussion section integrates findings with theoretical kernel frameworks and compares results with at least 10 recent (last 5 years) peer-reviewed articles.
