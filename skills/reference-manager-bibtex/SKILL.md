---
name: reference-manager-bibtex
description: Comprehensive guidelines and prompt recipes for managing references, citations, and BibTeX/RIS files for academic manuscripts. Use when formatting citations, checking DOI metadata, cleaning BibTeX entries, converting citation styles (APA 7th, IEEE, Vancouver, Harvard), or detecting orphan citations and outdated references.
---

# Reference Manager & BibTeX Specialist

Provides guidelines, BibTeX/RIS syntax standards, reference metadata verification rules (DOIs, volume, issue, page numbers), citation style conversion frameworks (APA 7th, IEEE, Vancouver, Harvard), and citation consistency audits for academic manuscripts.

## When to Use

Use this skill when the user:
- Requests generation, cleaning, or syntax validation of BibTeX (`.bib`) or RIS (`.ris`) files.
- Needs citation style conversion between standards (e.g., APA 7th to IEEE or Vancouver).
- Asks for metadata verification of references (DOIs, journal names, volume/issue numbers, page ranges).
- Wants to audit consistency between in-text citations and the reference list (detecting orphan citations).
- Requires evaluation of literature currency (percentage of references from the last 5–10 years).

---

## BibTeX Entry Standards

### 1. Journal Article (`@article`)
```bibtex
@article{Arrasyid2026AI,
  author    = {Arrasyid, Rafli and Pratama, Budi},
  title     = {Implementation of {AI} Agents in Academic Publishing: A Systematic Review},
  journal   = {Journal of Educational Technology and Innovation},
  year      = {2026},
  volume    = {14},
  number    = {2},
  pages     = {105--120},
  doi       = {10.1016/j.jeti.2026.01.005}
}
```

### 2. Conference Proceedings (`@inproceedings`)
```bibtex
@inproceedings{Arrasyid2025Design,
  author    = {Arrasyid, Rafli},
  title     = {Designing Gamified Learning Platforms Using {Design-Based Research}},
  booktitle = {Proceedings of the 2025 International Conference on Learning Sciences},
  year      = {2025},
  pages     = {45--52},
  publisher = {IEEE},
  doi       = {10.1109/ICLS54321.2025.101234}
}
```

### 3. Book & Book Chapter (`@book` & `@incollection`)
```bibtex
@book{Branch2009Instructional,
  author    = {Branch, Robert Maribe},
  title     = {Instructional Design: The {ADDIE} Approach},
  publisher = {Springer},
  address   = {New York, NY},
  year      = {2009},
  doi       = {10.1007/978-0-387-09506-6}
}
```

---

## Core BibTeX Formatting Rules

1. **Capital Preservation**: Use curly braces `{}` around acronyms, proper nouns, or brand names to prevent LaTeX compilers from converting them to lowercase (e.g., `{AI}`, `{Indonesia}`, `{Sinta}`).
2. **Special Character Escaping**: Always escape LaTeX special characters:
   - `&` -> `\&`
   - `%` -> `\%`
   - `_` -> `\_`
   - `$` -> `\$`
3. **Author Name Formatting**: Use `Lastname, Firstname` or separate multiple authors with `and`:
   - ✅ `author = {Smith, John and Doe, Jane}`
   - ❌ `author = {John Smith, Jane Doe}`
4. **Page Ranges**: Use double hyphens (`--`) for page ranges (e.g., `105--120`).

---

## Citation Style Matrix

| Parameter | APA 7th Edition | IEEE Style | Vancouver Style | Harvard Style |
| --- | --- | --- | --- | --- |
| **In-Text Format** | Author-Date: `(Arrasyid & Pratama, 2026)` | Bracketed Number: `[1]` | Parenthetical / Superscript: `(1)` or `¹` | Author-Date: `(Arrasyid and Pratama 2026)` |
| **List Ordering** | Alphabetical by primary author | Order of appearance in text | Order of appearance in text | Alphabetical by primary author |
| **Author Name Format** | Lastname, Initial. (`Arrasyid, R.`) | Initial. Lastname (`R. Arrasyid`) | Lastname Initial (`Arrasyid R`) | Lastname, Initial. (`Arrasyid, R.`) |
| **Article Title** | Sentence case | Title Case in quotes `"Implementation..."` | Sentence case | Single quotes sentence case |
| **Journal Name** | Italic Title Case (*Journal of Educational...*) | Italic Abbreviated (*J. Educ. Technol.*) | Abbreviated no periods (*J Educ Technol*) | Italic Title Case |
| **DOI Format** | Full URL (`https://doi.org/...`) | DOI Prefix (`doi: 10.1109/...`) | URL or DOI identifier | Full URL |

---

## Citation Consistency Audit

1. **Orphan Citation Detection**:
   - Verify every in-text citation has a corresponding entry in the Reference List.
   - Verify every Reference List entry is cited at least once in the text.
2. **Currency Ratio Check**:
   - For rapidly evolving fields (AI, Computer Science, Technology), **at least 80%** of references should be published within the **last 5–10 years**.
3. **DOI Verification**:
   - Ensure all journal articles include valid, clickable DOI links.

---

## Interactive Prompt Templates

### Template 1: BibTeX Cleaning & Validation
> *"Here is my BibTeX file. Please clean the syntax, ensure acronyms and proper nouns are protected with curly braces, format author names correctly, and check for missing fields (DOI, volume, issue, page ranges)."*

### Template 2: Citation Style Conversion
> *"Convert the following reference list from APA 7th to IEEE format. Provide: (1) Ordered bracketed in-text citations [1], [2], and (2) Corresponding IEEE reference list."*

---

## Pre-Submission Quality Audit Checklist

- [ ] BibTeX syntax is free of missing braces `{}` or missing commas `,`.
- [ ] Acronyms and proper nouns in titles are enclosed in `{}`.
- [ ] Author names are consistently formatted as `Lastname, Firstname` separated by `and`.
- [ ] Special characters (`&`, `%`, `_`) are properly escaped.
- [ ] No orphan citations exist between text and references.
- [ ] Over 80% of references are primary journal articles from the last 5–10 years.
