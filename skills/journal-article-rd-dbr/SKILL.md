---
name: journal-article-rd-dbr
description: Guidelines, evaluation frameworks, and prompt recipes for writing, editing, and reviewing journal articles using Research & Development (R&D), Design and Development Research (DDR), Design Science Research (DSR), and Design-Based Research (DBR) methodologies. Use when working on development or design science paper drafts for Sinta and Scopus journals.
---

# Journal Article Writing: R&D, DDR, DSR, and DBR Methodologies

Provides comprehensive guidelines, evaluation frameworks, and prompt recipes for structuring, writing, editing, and reviewing research articles targeting accredited national (Sinta 1–4) and international (Scopus/WoS) journals using development and design methodologies: **Research & Development (R&D)**, **Design and Development Research (DDR)**, **Design Science Research (DSR)**, and **Design-Based Research (DBR)**.

## When to Use

Use this skill when the user:
- Requests guidelines, templates, or structure for paper drafts based on R&D, DDR, DSR, or DBR.
- Asks for review, critique, or improvement of a development or design science paper draft.
- Needs guidance choosing between R&D, DDR, DSR, and DBR for a specific research problem.
- Requires evaluation metrics (Aiken's V, N-Gain, SUS, Cohen's d), instrument validation formulas, or phrasing examples for Sinta/Scopus journals.

---

## Methodology Comparison Matrix

| Parameter | Research & Development (R&D) | Design and Development Research (DDR) | Design Science Research (DSR) | Design-Based Research (DBR) |
| --- | --- | --- | --- | --- |
| **Primary Focus** | Developing & testing the effectiveness of educational products/media | Systematic study of designing, developing, & evaluating products/models | Developing innovative artifacts to solve technical or Information System problems | Iteratively improving real-world learning practices in authentic contexts |
| **Key References** | Borg & Gall (1983), Thiagarajan et al. (4D, 1974), ADDIE (Branch, 2009) | Richey & Klein (2007), Ellis & Levy (2010) | Hevner et al. (2004), Peffers et al. DSRM (2007) | McKenney & Reeves (2012/2019), DBR Collective (2003) |
| **Output** | Valid, practical, & effective product | Product/tool + design principles or model framework | Artifact (software, algorithm, architecture) + knowledge base contribution | Practical intervention + Design Principles |
| **Evaluation Metrics**| Aiken's V, Gregory's Agreement, SUS, N-Gain Score, Effect Size | Usability testing, Expert review, Formative & Summative evaluation | Demonstration, Empirical evaluation, Performance tests | Formative evaluation, Field observation, Iterative reflections |
| **Target Journals** | Educational Journals (Sinta 1–3, Scopus Q2/Q3) | Educational Technology & Instructional Design Journals | IS / Computer Science Journals (IEEE, Elsevier, Scopus Q1/Q2) | Learning Sciences & Educational Technology Journals |

---

## Article Structure & Page Proportions (5,000–8,000 Words)

1. **Title & Abstract (5%)**: Mentions specific artifact/product, target context, methodology, and key quantitative findings.
2. **Introduction (15–20%)**: State-of-the-art, literature gap analysis, needs analysis, and explicit novelty statement.
3. **Methodology (15–20%)**: Adapted development model, validator qualifications, instrument validation, statistical formulas (Aiken's V, N-Gain).
4. **Results & Discussion (45–50%)**:
   - *Results*: Visual evidence of artifact/iterations, validation tables, practicality scores, effectiveness tests.
   - *Discussion*: Theoretical explanation of why features worked, integration with kernel theories/literature, limitations.
5. **Conclusion & Recommendations (5–10%)**: Answers to research questions, theoretical/practical contributions, future research roadmap.

---

## Methodology-Specific Patterns

### 1. Research & Development (R&D)
- **Frameworks**: ADDIE, 4D (Define, Design, Develop, Disseminate), Borg & Gall (simplified to 5–7 steps).
- **Key Metrics**:
  - **Validity**: Aiken's V ($V = \frac{\sum s}{n(c-1)}$) or Gregory's Content Validity index.
  - **Practicality**: User response questionnaires / System Usability Scale (SUS).
  - **Effectiveness**: Normalized Gain ($N\text{-Gain} = \frac{S_{\text{post}} - S_{\text{pre}}}{S_{\text{max}} - S_{\text{pre}}}$) and Cohen's $d$.

### 2. Design Science Research (DSR)
- **Frameworks**: Peffers DSRM 6 Steps (Problem ID, Objectives, Design & Development, Demonstration, Evaluation, Communication) or Hevner's 3-Cycle Model (Relevance, Design, Rigor).
- **Core Elements**:
  - **Relevance Cycle**: Real-world problem & artifact evaluation criteria.
  - **Rigor Cycle**: Theoretical foundation (*kernel theories*) & knowledge base contribution.
  - **Design Cycle**: System architecture, UML/ERD, algorithms, and instantiations.

### 3. Design-Based Research (DBR)
- **Frameworks**: McKenney & Reeves (Analysis & Exploration, Design & Construction, Evaluation & Reflection).
- **Core Elements**: Iterative cycles in authentic learning settings, practitioner collaboration, and extraction of **Design Principles**:
  *“To design [Artifact X] for [Goal Y] in [Context Z], you should [Action A], because [Theoretical Reason B].”*

---

## Interactive Prompt Templates

### Template 1: Drafting the Methodology Section
> *"Help me draft the Methodology section for a Scopus-indexed journal paper using [R&D / DDR / DSR / DBR]. The product is [Specify Product], guided by the [ADDIE / 4D / Peffers / McKenney & Reeves] model. Include validator profiles, instrument details, and statistical formulas (Aiken's V, N-Gain, SUS)."*

### Template 2: Reviewing Development Paper Drafts
> *"Act as a reviewer for a Sinta 2 / Scopus journal. Evaluate the following [R&D / DSR / DBR] paper draft based on: (1) Clarity of development model, (2) Adequacy of quantitative validity/effectiveness evidence, (3) Depth of theoretical discussion, and (4) Novelty."*

---

## Pre-Submission Quality Audit Checklist

- [ ] Development model is explicitly cited with foundational references.
- [ ] Quantitative validation data from at least 2 subject matter experts and 2 media/technical experts.
- [ ] Effectiveness reported using appropriate statistical metrics (Aiken's V, N-Gain, SUS, Effect Size).
- [ ] Visual evidence of product iterations, screenshots, or system architecture included.
- [ ] Discussion section compares findings with at least 10 recent (last 5 years) peer-reviewed journal articles.

---

## Critical Gotchas

- **Confusing R&D with Pure Experimental Research**: R&D focuses on the design-and-evalulative cycle of an artifact, not merely statistical treatment effects.
- **Omitting Revision Matrices**: Reviewers inspect expert feedback matrices and specific artifact modifications between iterations.
- **Reporting Raw Metrics Without Qualitative Explanation**: High validity scores must be accompanied by narrative explanations of which specific features contributed to usability.
