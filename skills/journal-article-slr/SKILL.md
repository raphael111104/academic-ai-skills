---
name: journal-article-slr
description: Comprehensive guidelines and protocols for writing Systematic Literature Review (SLR) journal articles following PRISMA 2020 standards and the Kitchenham framework. Use when the user requests help structuring SLR articles, formulating research questions (PICOC), constructing Boolean search queries, creating PRISMA flowcharts, or synthesizing literature.
---

# Journal Article Writing: Systematic Literature Review (SLR)

Provides comprehensive guidelines for structuring, writing, evaluating, and revising Systematic Literature Review (SLR) journal articles adhering to PRISMA 2020 standards (*Preferred Reporting Items for Systematic Reviews and Meta-Analyses*) and the Kitchenham (2007) protocol for high-impact journals (Sinta 1–3, Scopus, WoS).

## When to Use

Use this skill when the user:
- Requests guidelines or templates for writing a Systematic Literature Review (SLR) paper.
- Needs formulation of Research Questions (RQs) using PICOC/PICOS frameworks.
- Requires construction of Boolean search queries across major databases (Scopus, WoS, IEEE Xplore, ScienceDirect).
- Asks for PRISMA 2020 flowchart generation, inclusion/exclusion criteria tables, or Quality Assessment (QA) scoring.
- Wants to synthesize primary studies using thematic analysis, taxonomy mapping, or bibliometric co-occurrence analysis.

---

## Foundational Protocols

### 1. Kitchenham Protocol (2007)
Consists of 3 core phases:
1. **Planning the Review**: Identifying review necessity, registering protocol (OSF/PROSPERO), formulating RQs, establishing criteria.
2. **Conducting the Review**: Search query execution, study screening, Quality Assessment (QA) / Risk of Bias, data extraction, thematic synthesis.
3. **Reporting the Review**: Manuscript drafting, compiling PRISMA 2020 checklist, dissemination.

### 2. PRISMA 2020 Flowchart Workflow
Mandates transparent reporting across 4 main stages:
1. **Identification**: Records identified from academic databases (Scopus, IEEE Xplore, ScienceDirect, WoS) and deduplication.
2. **Screening**: Title and abstract screening against initial eligibility criteria.
3. **Eligibility**: Full-text assessment against specific inclusion/exclusion criteria with documented exclusion reasons for every excluded paper.
4. **Included**: Final number of primary studies included in the systematic synthesis ($n = X$).

---

## Research Question Formulation (PICOC / PICOS)

Use the PICOC framework to structure RQs:

- **P (Population / Problem)**: Target domain or subject group (e.g., K-12 students, software engineers, SMEs).
- **I (Intervention / Topic)**: Technology, method, or approach evaluated (e.g., AI tutoring, gamification, Agile methods).
- **C (Comparison / Control)**: Baseline alternative if applicable (e.g., traditional instruction, non-AI systems).
- **O (Outcome)**: Measured impacts (e.g., cognitive learning gains, operational efficiency, user satisfaction).
- **C/S (Context / Study Design)**: Research environment, industry sector, or study design considered.

### Standard RQ Structure
- **RQ1 (Trends & Bibliometrics)**: What are the publication trends, geographical distributions, and key venues from year Y to Z?
- **RQ2 (Methodologies & Techniques)**: What methodologies, algorithms, or frameworks are predominantly deployed in primary studies?
- **RQ3 (Findings & Empirical Impacts)**: What are the key empirical findings and impacts of intervention X on outcome O?
- **RQ4 (Challenges & Future Agenda)**: What are the primary challenges, limitations, and research gaps for future research?

---

## Boolean Search String Construction

Construct search strings using field tags (`TITLE-ABS-KEY`), exact phrase quotes `""`, wildcards `*`, and Boolean operators `AND` / `OR`:

```text
( TITLE-ABS-KEY ( "artificial intelligence" OR "AI" OR "machine learning" ) )
AND
( TITLE-ABS-KEY ( "educational technology" OR "higher education" OR "K-12" ) )
AND
( TITLE-ABS-KEY ( "systematic literature review" OR "SLR" OR "systematic review" ) )
```

---

## Quality Assessment (QA) Protocol

Evaluate selected primary studies using a 5-point Quality Assessment scale (Scoring: Yes = 1.0, Partial = 0.5, No = 0.0):

- **QA1**: Are the research objectives clearly stated?
- **QA2**: Is the methodology adequately described and replicable?
- **QA3**: Are the data collection instruments validated?
- **QA4**: Are the statistical analyses appropriate for the research questions?
- **QA5**: Do the conclusions logically follow from the empirical findings?
- **Threshold**: Include primary studies achieving a total QA score $\ge 3.5 / 5.0$.

---

## Interactive Prompt Templates

### Template 1: Boolean Search & PICOC Formulation
> *"Help me formulate PICOC parameters and a Boolean search query for Scopus and IEEE Xplore on [Topic]. Include wildcards, exact quotes, and field tags. Timeframe: 2020–2025."*

### Template 2: Synthesis & Research Gap Mapping
> *"Act as an SLR expert. Synthesize the findings of the attached 20 primary studies into a taxonomy table answering RQ2 (Predominant Methodologies) and RQ3 (Empirical Outcomes). Identify 3 explicit research gaps for the Discussion section."*

---

## Pre-Submission Quality Audit Checklist

- [ ] Title explicitly contains "Systematic Literature Review" or "SLR".
- [ ] Research Questions (3–4 RQs) formulated using PICOC/PICOS.
- [ ] Major databases (Scopus, WoS, IEEE, ScienceDirect) searched with replicable Boolean queries.
- [ ] PRISMA 2020 Flowchart included with explicit full-text exclusion reasons.
- [ ] Quality Assessment (QA) criteria applied with explicit threshold cutoff.
- [ ] Primary studies synthesized thematically rather than summarized abstract-by-abstract.
