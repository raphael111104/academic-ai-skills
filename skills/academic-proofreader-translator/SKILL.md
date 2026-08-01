---
name: academic-proofreader-translator
description: Comprehensive guidelines and prompt recipes for academic proofreading, English grammar correction, scholarly translation, sentence structure refactoring, and register alignment for high-impact journals (Sinta, Scopus, IEEE, Elsevier, Springer). Use when the user requests help translating, proofreading, refining academic tone, calibrating scientific hedging, or polishing paper manuscripts.
---

# Academic Proofreader & Translator

Provides an advanced, multi-tier editing framework, scholarly translation protocols, academic register principles, and structural refactoring strategies for publishing in high-impact international journals (Scopus, WoS, IEEE, Elsevier, Springer, Nature) and accredited national journals (Sinta 1–4).

## When to Use

Use this skill when the user:
- Requests precision academic translation between Indonesian and Academic English.
- Requires proofreading, grammar correction, style polishing, or readability optimization for research paper drafts.
- Needs to eliminate informal phrasing, conversational filler, wordiness, or literal machine translation artifacts (*false friends*).
- Requires calibration of scientific hedging, objective tone, Academic Word List (AWL) vocabulary, and paragraph cohesion.
- Seeks structural refactoring (converting nominalizations, fixing dangling modifiers, resolving ambiguous pronoun references).

---

## Core Principles of Academic Register

### 1. Formality & Vocabulary Elevation
- Utilize Academic Word List (AWL) terminology.
- Replace informal phrasal verbs with formal single-word equivalents:
  - ❌ *look into* -> ✅ *investigate* / *examine*
  - ❌ *set up* -> ✅ *establish* / *configure*
  - ❌ *find out* -> ✅ *determine* / *ascertain*
  - ❌ *bring about* -> ✅ *induce* / *precipitate*
  - ❌ *get rid of* -> ✅ *eliminate* / *eradicate*
- Eliminate contractions (*don't*, *can't*, *it's* -> *do not*, *cannot*, *it is*), colloquialisms, and rhetorical questions.

### 2. Scientific Hedging Taxonomy
Calibrate claims precisely based on empirical certainty:

| Hedging Category | Function | Preferred Terms | Example Usage |
| --- | --- | --- | --- |
| **Epistemic Verbs** | Expressing interpretation | *suggest, indicate, propose, infer, speculate* | *The data suggest that feature X enhances performance.* |
| **Probability Adverbs** | Calibrating likelihood | *plausibly, potentially, presumably, conceivably* | *This mechanism potentially explains the observed variance.* |
| **Modal Auxiliaries** | Expressing possibility | *may, might, could* | *Higher temperatures may accelerate catalyst degradation.* |
| **Approximators** | Refining measurements | *approximately, roughly, predominantly, virtually* | *The reaction was predominantly completed within 30 minutes.* |

### 3. Sentence Structure Refactoring Rules
- **De-nominalization**: Convert heavy noun phrases back into active verbs to improve sentence momentum:
  - ❌ *We conducted an investigation into the effects of...*
  - ✅ *We investigated how X affects...*
  - ❌ *The occurrence of a decrease in accuracy was observed...*
  - ✅ *Accuracy decreased when...*
- **Fixing Ambiguous Pronouns**: Never use *This* or *These* as standalone subjects. Always append a clarifying head noun:
  - ❌ *This shows that the algorithm fails.*
  - ✅ *This performance degradation indicates that the algorithm fails.*
- **Dangling Modifiers**: Ensure introductory participle phrases logically modify the subject immediately following:
  - ❌ *Using a 5-point Likert scale, the survey was completed by 100 students.*
  - ✅ *Using a 5-point Likert scale, we surveyed 100 students.*

---

## Precision Translation Strategies (ID <-> EN)

### Translation Traps & False Friends

| Indonesian Source Phrase | Literal Translation Trap (❌ Incorrect) | Academic Translation (✅ Correct) |
| --- | --- | --- |
| *Berdasarkan hasil penelitian...* | *Based on the result of the research...* | *The empirical findings indicate that...* / *As demonstrated by the experimental data,...* |
| *Penelitian ini bertujuan untuk...* | *This research aims to...* | *This study aims to...* / *The primary objective of this investigation is to...* |
| *Peneliti melakukan wawancara...* | *Researcher conducted interviews...* | *Semi-structured interviews were conducted to...* / *We conducted interviews to...* |
| *Hal ini menunjukkan bahwa...* | *This thing shows that...* | *These findings suggest that...* / *This outcome demonstrates that...* |
| *Dapat disimpulkan bahwa...* | *Can be concluded that...* | *It can be concluded that...* / *In conclusion, the data confirm that...* |
| *Uji praktikalitas produk...* | *Practical testing of the product...* | *Product practicality evaluation...* / *Usability testing...* |

---

## Section-Specific Verb Tense Rules

- **Abstract**: *Present Simple* for general context; *Past Simple* for methodologies and results; *Present Simple* for main conclusion.
- **Introduction**: *Present Simple* for established domain truths; *Present Perfect* for ongoing research trends (*Recent studies have explored...*); *Past Simple* for specific past experiments.
- **Methods**: *Past Simple* (predominantly passive voice) for procedural actions (*Data were collected...*, *Samples were synthesized...*).
- **Results**: *Past Simple* for reporting observed data (*Model A achieved 94.2% accuracy*, *The difference was statistically significant*).
- **Discussion**: *Present Simple* for interpreting implications (*These results indicate...*); *Modal Past/Present* for recommendations and future directions.

---

## Interactive Prompt Templates

### Template 1: Precision Academic Translation
> *"Act as an expert academic translator. Translate the following text from Indonesian to Academic English suitable for a Scopus Q1 journal in [Field]. Ensure Academic Word List (AWL) vocabulary, correct section-specific tenses, de-nominalization, and elimination of literal translation traps. Provide: (1) Translated Text, and (2) Translation Notes."*

### Template 2: Multi-Tier Proofreading & Refactoring
> *"Act as a Senior Managing Editor for an IEEE/Elsevier journal. Proofread and refactor the attached manuscript section. Focus on fixing grammar, eliminating wordiness, removing dangling modifiers, and calibrating scientific hedging. Provide: (1) Polished Text, and (2) Summary of Key Refactorings."*

---

## Pre-Submission Quality Audit Checklist

- [ ] All standalone subject pronouns (*This*, *These*) have explicit head nouns.
- [ ] No informal phrasal verbs, contractions, or conversational filler remain.
- [ ] Passive voice is used appropriately in Methods, while active voice highlights key contributions in Introduction/Discussion.
- [ ] Verb tenses adhere strictly to section conventions (Past Tense for Methods/Results).
- [ ] Scientific claims are appropriately hedged (no absolute statements like *100% proves* without mathematical proof).
