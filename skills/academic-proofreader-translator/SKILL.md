---
name: academic-proofreader-translator
description: Guidelines and prompt recipes for academic proofreading, English grammar correction, scholarly translation, and maintaining cohesion and register for high-impact journals (Sinta, Scopus, IEEE, Elsevier, Springer). Use when the user requests help translating, proofreading, refining academic tone, or polishing paper manuscripts.
---

# Academic Proofreader & Translator

Provides comprehensive guidelines, academic register principles, precision translation strategies, and multi-tier proofreading techniques for publishing in high-impact international journals (Scopus, WoS, IEEE, Elsevier, Springer) and accredited national journals (Sinta 1–4).

## When to Use

Use this skill when the user:
- Requests academic translation of manuscript drafts between Indonesian and Academic English.
- Needs proofreading, grammar correction, style polishing, or readability enhancements for research paper drafts.
- Wants to eliminate informal phrasing, wordiness, or literal machine translation artifacts.
- Requires calibration of academic register (hedging, objective tone, Academic Word List vocabulary, paragraph cohesion).

---

## Core Principles of Academic Register

1. **Formality & Objectivity**: Use Academic Word List (AWL) vocabulary. Avoid conversational language, contractions (*don't*, *can't* -> *do not*, *cannot*), colloquialisms, and idioms.
2. **Precision & Hedging**: Calibrate scientific claims using appropriate hedging terms. Distinguish clearly between empirical facts (*the results demonstrate*) and hypotheses or interpretations (*the findings suggest*, *the data indicate*).
3. **Spelling Consistency**: Maintain 100% consistency in language variants throughout the manuscript:
   - *American English (US)*: *behavior, analyze, program, organize*.
   - *British English (UK)*: *behaviour, analyse, programme, organise*.
4. **Cohesion & Transitions**: Deploy academic transition markers (*furthermore*, *consequently*, *conversely*, *nevertheless*) appropriately to ensure logical paragraph flow.

---

## Core Workflows

### Mode 1: Precision Academic Translation

Academic translation must avoid word-for-word literal translation that results in awkward phrasing.

#### Common Translation Traps (ID <-> EN)

| Indonesian Phrase | Literal Translation Trap (❌ Incorrect) | Academic Translation (✅ Correct) |
| --- | --- | --- |
| *Berdasarkan hasil penelitian...* | *Based on the result of the research...* | *The empirical findings indicate that...* / *As demonstrated by the experimental results,...* |
| *Penelitian ini bertujuan untuk...* | *This research aims to...* | *This study aims to...* / *The objective of this investigation is to...* |
| *Peneliti melakukan wawancara...* | *Researcher conducted interviews...* | *Semi-structured interviews were conducted to...* / *We conducted interviews to...* |
| *Hal ini menunjukkan bahwa...* | *This thing shows that...* | *These findings suggest that...* / *This outcome demonstrates that...* |
| *Dapat disimpulkan bahwa...* | *Can be concluded that...* | *It can be concluded that...* / *In conclusion, the data confirm that...* |
| *Semakin tinggi A, maka semakin B...* | *More high A, then more B...* | *A higher level of A corresponds to an increase in B...* |

#### Verb Tense Conventions Across Sections

- **Abstract & Introduction**: *Present Simple* for established facts (*AI enhances operational efficiency*); *Present Perfect* for general literature background (*Recent studies have investigated...*).
- **Methods & Results**: *Past Simple* for completed research actions (*Data were collected...*, *The model achieved 94.5% accuracy*).
- **Discussion & Conclusion**: *Present Simple* for interpretations (*This implies that...*) and recommendations.

---

### Mode 2: Multi-Tier Proofreading & Polishing

1. **Grammar & Mechanics**: Correct subject-verb agreement, article usage (*a/an/the*), verb tenses, and punctuation.
2. **Conciseness & Paraphrasing**: Eliminate redundancies and simplify convoluted phrasing.
   - ❌ *Due to the fact that* -> ✅ *Because* / *Since*
   - ❌ *At the present time* -> ✅ *Currently* / *Presently*
   - ❌ *In order to achieve the purpose of* -> ✅ *To achieve*
3. **Academic Hedging Calibration**:
   - Overly Strong Claim (❌): *This algorithm proves that feature X is the optimal solution.*
   - Calibrated Claim (✅): *The experimental results suggest that feature X provides a statistically significant performance improvement.*
4. **Active vs. Passive Voice Optimization**:
   - Use *passive voice* in Methods sections to maintain procedural focus (*Data were gathered using...*).
   - Use *active voice* (*We propose...*) when highlighting researcher contributions if target journal guidelines allow.

---

## Publisher Style Matrix

| Publisher / Journal | Citation Format | Language Variant | Use of First Person ("I"/"We") | Figure & Table Captions |
| --- | --- | --- | --- | --- |
| **IEEE** | Bracketed Numbers `[1]`, `[2]` | US English | Allowed (*We propose...*) | Figure (Fig. 1), Table I (Roman) |
| **Elsevier** | APA / Harvard / Numbered | US or UK (Consistent) | Sparingly allowed | Figure 1, Table 1 |
| **Springer / Nature** | Numbered / Author-Date | UK or US English | Allowed | Figure 1, Table 1 |
| **Sinta (National)** | APA 7th / IEEE | Indonesian or English | Per Author Guidelines | Gambar 1, Tabel 1 / Figure 1, Table 1 |

---

## Interactive Prompt Templates

### Template 1: Paragraph Translation to Academic English
> *"Translate the following paragraph into Academic English suitable for a Scopus Q1/Q2 journal. Ensure Academic Word List (AWL) vocabulary, appropriate verb tenses (Past for methods/results, Present for discussion), and smooth cohesion between sentences."*

### Template 2: Comprehensive Proofreading & Polishing
> *"Act as a Senior Academic Editor for an international journal. Edit the following manuscript section to improve readability, eliminate wordiness, correct grammatical errors, and calibrate scientific hedging. Provide: (1) Polished Text, and (2) Summary of Key Edits."*

---

## Pre-Submission Quality Audit Checklist

- [ ] Free of literal translation traps (*false friends* and rigid syntax).
- [ ] Section-specific tenses are consistently applied (*Past Tense* for Methods/Results).
- [ ] Language variant (US vs. UK) is 100% consistent throughout the text.
- [ ] No informal phrasing, contractions (*can't*, *it's*), or slang.
- [ ] Scientific claims are properly calibrated with appropriate hedging.
- [ ] Article usage (*a/an/the*) and singular/plural agreements have been verified.

---

## Critical Gotchas

- **Literal Translation of Technical Terms**: Do not translate domain-specific terms literally (e.g., use *Practicality Evaluation* instead of *Practical Testing*).
- **Over-hedging vs. Under-hedging**: Over-hedging (*It might possibly seem to suggest...*) signals lack of confidence; under-hedging (*This proves 100% that...*) makes claims vulnerable to reviewer rejection.
- **Overusing Transitions**: Avoid starting every sentence with *Furthermore*, *Moreover*, or *Therefore*, which creates rigid and repetitive prose.
