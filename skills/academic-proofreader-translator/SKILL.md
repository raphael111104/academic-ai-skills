---
name: academic-proofreader-translator
description: Panduan dan resep penyuntingan (proofreading), perbaikan tata bahasa Inggris/Indonesia akademis, penerjemahan artikel ilmiah, serta pemeliharaan alur kohesi dan register bahasa jurnal bereputasi (Sinta / Scopus / IEEE / Elsevier / Springer). Gunakan saat pengguna meminta bantuan menerjemahkan, mengedit tata bahasa, menyelaraskan gaya akademis, atau memoles (polishing) naskah karya ilmiah.
---

# Academic Proofreader & Translator

Skill ini memberikan panduan komprehensif, aturan register bahasa akademis, strategi penerjemahan presisi, dan teknik penyuntingan naskah ilmiah (*academic proofreading & polishing*) untuk publikasi di jurnal bereputasi internasional (Scopus, WoS, IEEE, Elsevier, Springer) dan nasional terakreditasi (Sinta 1–4).

## When to Use

Gunakan skill ini saat pengguna:

- Meminta penerjemahan draf naskah ilmiah dari Bahasa Indonesia ke Bahasa Inggris Akademis (*Academic English*) atau sebaliknya.
- Meminta *proofreading*, perbaikan *grammar*, *polishing*, atau peningkatan keterbacaan (*readability*) draf artikel jurnal.
- Ingin mengeliminasi frasa informal, kata-kata redundan (*wordiness*), atau kesalahan terjemahan literal (*machine translation errors*).
- Membutuhkan penyesuaian register bahasa akademis (*hedging*, nada obyektif, *academic vocabulary*, kohesi paragraf).

---

## Prinsip Utama Register Bahasa Akademis (*Academic Register*)

1. **Formalitas & Obyektivitas**: Gunakan kosa kata tingkat akademis (*Academic Word List / AWL*). Hindari frasa percakapan, kontraksi (*don't*, *can't* -> *do not*, *cannot*), idiom, dan klise.
2. **Keterukuran & Hedging**: Gunakan bahasa berhati-hati (*hedging*) untuk klaim ilmiah. Bedakan antara fakta teruji (*the results demonstrate*) dan hipotesis/interpretasi (*the findings suggest*, *the data indicate*).
3. **Konsistensi Varian Bahasa**: Patuhi satu varian bahasa secara konsisten dalam seluruh artikel:
   - *American English (US)*: *behavior, analyze, program, organize*.
   - *British English (UK)*: *behaviour, analyse, programme, organise*.
4. **Kohesi & Struktur Antarkalimat**: Gunakan penanda transisi akademis (*academic transition words*) yang tepat (*furthermore*, *consequently*, *conversely*, *nevertheless*) untuk menjaga alur logika (*coherence & cohesion*).

---

## Alur Kerja Utama

### Modus 1: Penerjemahan Akademis Presisi (*Academic Translation*)

Penerjemahan teks ilmiah wajib menghindari terjemahan harfiah (*word-for-word*) yang sering dihasilkan mesin penerjemah.

#### Aturan & Perangkap Umum Penerjemahan ID <-> EN

| Frasa Indonesia | Perangkap Terjemahan Literal (❌ Salah) | Terjemahan Akademis yang Tepat (✅ Benar) |
| --- | --- | --- |
| *Berdasarkan hasil penelitian...* | *Based on the result of the research...* | *The empirical findings indicate that...* / *As shown by the experimental results,...* |
| *Penelitian ini bertujuan untuk...* | *This research aims to...* | *This study aims to...* / *The objective of this investigation is to...* |
| *Peneliti melakukan wawancara...* | *Researcher conducted interviews...* | *Interviews were conducted to...* / *We conducted semi-structured interviews to...* |
| *Hal ini menunjukkan bahwa...* | *This thing shows that...* | *These findings suggest that...* / *This outcome demonstrates that...* |
| *Dapat disimpulkan bahwa...* | *Can be concluded that...* | *It can be concluded that...* / *In conclusion, the data confirm that...* |
| *Semakin tinggi A, maka semakin B...* | *More high A, then more B...* | *A higher level of A corresponds to an increase in B...* / *As A increases, B exhibits a corresponding rise...* |

#### Panduan Penggunaan Kata Kerja (*Tense Usage in Academic Papers*)

- **Abstract & Introduction**: *Present Simple* untuk fakta umum (*AI impacts productivity*); *Present Perfect* untuk tinjauan literatur umum (*Studies have investigated...*).
- **Methods & Results**: *Past Simple* untuk tindakan spesifik yang telah dilakukan (*Data were collected...*, *The algorithm achieved 92% accuracy*).
- **Discussion & Conclusion**: *Present Simple* untuk interpretasi temuan (*This implies that...*) dan rekomendasi.

---

### Modus 2: Penyuntingan & Pemolesan (*Proofreading & Polishing*)

Proses penyuntingan dilakukan secara berlapis mencakup 4 tingkat perbaikan:

1. **Grammar & Mechanics Check**: Perbaikan *subject-verb agreement*, penggunaan artikel (*a/an/the*), bentuk kata kerja (*tenses*), dan tanda baca.
2. **Conciseness & Paraphrasing**: Mengeliminasi kata berlebihan (*wordiness*) dan menyederhanakan frasa rumit tanpa mengurangi makna ilmiah.
   - ❌ *Due to the fact that* -> ✅ *Because* / *Since*
   - ❌ *At the present time* -> ✅ *Currently* / *Presently*
   - ❌ *In order to achieve the purpose of* -> ✅ *To achieve*
   - ❌ *A total of 150 respondents participated in* -> ✅ *A total of 150 respondents completed*
3. **Academic Hedging Calibration**:
   - Klaim Terlalu Kuat (❌): *This model proves that feature X is the best solution.*
   - Terkalibrasi (✅): *The empirical results suggest that feature X provides a significant performance enhancement.*
4. **Active vs Passive Voice Optimization**:
   - Gunakan *passive voice* pada bagian *Methods* untuk fokus pada prosedur (*Data were collected using...*).
   - Gunakan *active voice* / *first-person plural* (*we*) bila jurnal mengizinkan untuk menyoroti kontribusi peneliti (*We propose a novel framework...*).

---

## Tabel Perbandingan Gaya Penerbit (*Publisher Style Conventions*)

| Penerbit / Jurnal | Gaya Sitasi | Varian Bahasa | Penggunaan "I" / "We" | Format Gambar/Tabel |
| --- | --- | --- | --- | --- |
| **IEEE** | Angka siku `[1]`, `[2]` | US English | Diizinkan (*We propose...*) | Figure (Fig. 1), Table I (Romawi) |
| **Elsevier** | APA / Harvard / Numbered | US atau UK (Konsisten) | Diizinkan terbatas | Figure 1, Table 1 |
| **Springer / Nature** | Numbered / Author-Date | UK / US English | Diizinkan | Figure 1, Table 1 |
| **Sinta (Nasional)** | APA 7th / IEEE | Bahasa Indonesia / Inggris | Sesuai *Author Guidelines* | Gambar 1, Tabel 1 |

---

## Resep Prompt Siap Pakai (*Interactive Prompt Templates*)

### Templat 1: Penerjemahan Draf Abstrak / Paragraf ke Bahasa Inggris Akademis

> *"Terjemahkan paragraf berikut dari Bahasa Indonesia ke Bahasa Inggris Akademis (Academic English) berstandar Scopus Q1/Q2. Pastikan pilihan kata sesuai dengan Academic Word List (AWL), tenses tepat (Past Tense untuk metode/hasil, Present Tense untuk diskusi), dan alur antarkalimat kohesif."*

### Templat 2: Proofreading & Polishing Artikel Jurnal

> *"Bertindaklah sebagai Senior Academic Editor jurnal internasional. Sunting draf teks berikut untuk meningkatkan keterbacaan (readability), eliminasi wordiness/redundansi, perbaiki grammar, dan kalibrasi hedging. Berikan output dalam format: (1) Teks Hasil Polishing, dan (2) Daftar Ringkas Perubahan Utama (Key Edits Summary)."*

### Templat 3: Peningkatan Register Bahasa & Eliminasi Informalisme

> *"Tinjau draf berikut dan ubah frasa informal/percakapan menjadi register bahasa akademis yang baku dan profesional. Sertakan alasan perubahan pada kata-kata kunci."*

---

## Quality Audit Checklist Sebelum Submit

- [ ] Bebas dari kesalahan terjemahan literal ID <-> EN (*false friends* dan struktur kaku).
- [ ] Penggunaan tenses konsisten di tiap bagian (*Methods* = Past Tense, *Discussion* = Present Tense).
- [ ] Varian bahasa (*US vs UK English*) konsisten 100% di seluruh naskah.
- [ ] Tidak ada penggunaan frasa percakapan, idiom, atau kontraksi (*don't*, *can't*, *it's*).
- [ ] Penggunaan *hedging* terkalibrasi secara ilmiah (tidak membuat klaim berlebihan tanpa data mutlak).
- [ ] Penanda transisi (*academic transition markers*) digunakan secara natural antarkalimat dan antarparagraf.
- [ ] Penggunaan *articles* (*a*, *an*, *the*) dan *plural/singular agreements* telah diverifikasi secara akurat.

---

## Gotchas & Perangkap Kritis

- **Terjemahan Literal Istilah Spesifik**: Jangan menerjemahkan istilah teknis/domain-specific secara harfiah. Contoh: *Pengujian Praktikalitas* -> *Practicality Testing*, bukan *Practical Testing*.
- **Over-hedging vs Under-hedging**: Terlalu banyak *hedging* (*It might possibly seem to suggest...*) membuat tulisan ragu-ragu; terlalu sedikit *hedging* (*This proves 100% that...*) membuat klaim mudah disanggah reviewer.
- **Transisi Berlebihan (*Overusing Transitions*)**: Memulai setiap kalimat dengan *Furthermore*, *Moreover*, *Therefore* membuat paragraf terasa kaku dan repetitif.
