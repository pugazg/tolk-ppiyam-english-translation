# Textual-Fidelity Audit — Iteration 02

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **29–38**  
Unit: **Part I Chapter 1 — நூன் மரபு / Conventions of Grammar**

## Result

**PASS WITH CORRECTIONS**

Every page in the range was raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **10**
- Pages requiring corrections: **9**
- Pages exact as already transcribed: **1**
- Missing page files: **0**
- Empty page files: **0**
- Unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF page **33**.

### Corrected

| PDF page | Correction made | Commit |
|---:|---|---|
| 29 | Restored the edition’s printed Tamil forms `னகரவிறுவாய்`, `முப்பஃ தென்ப`, `ஒள`, and `அப்பா லேழும்` instead of normalized readings. | `5299399fc8e692e3c2208ac12b9009f73840d9ac` |
| 30 | Restored the printed colon in the heading `—: three measure.` | `fe484546ab031090883d9411afca2e68ea371cb9` |
| 31 | Restored `ஒளகார விறுவாய்ப்`, `பன்னீ ரெழுத்தும்`, and `னகார விறுவாய்ப்`. | `b020a36c14d3cd935dee103d007f0573a2ed2630` |
| 32 | Restored the three printed colon headings before verses 11–13. | `5eb481d945a1cbd847ccde5542a0a04423e8c343` |
| 34 | Restored the printed typo `Medial Consonauts` and corrected the transliteration symbols in verses 23–24 to `ṟ`, `l`, and `ḷ` as printed. | `411bb6ee5ee834c0bf677800e21be5c4d63c5d96` |
| 35 | Restored the period after the first line of verse 30. | `95533ccff7b7b4acd8d328bc38ce37408e6fac23` |
| 36 | Corrected the final consonant in verse 29 from `a` to printed `ṅ`; removed periods not present after verses 28 and 29. | `267ba647ff80289c8457d1bbc0026a2532652b48` |
| 37 | Restored `Similiar`, removed the unprinted period in note 1, and restored punctuation in note 8 (`measure, It` and `vowel-consonant, | pi |`). | `3e1611aac8e4465488cc9262a4831f626b8fa327` |
| 38 | Removed the period not printed after the final transliteration expression in note 9. | `2bade95c5007773074b0a8d3a39e272b92991964` |

## Correction categories

- Tamil source forms and sandhi-like printed spellings
- Tamil word spacing retained from the edition
- Transliteration diacritics and consonant identities
- Source typographical irregularities
- Heading punctuation
- Sentence and verse-final punctuation

## Method

Each page was inspected directly from a fresh raster rendering of the source PDF. Tamil source pages, English translation pages, headings, sūtra numbering, transliteration symbols, notes and punctuation were compared visually. The edition’s wording and errors were preserved rather than silently regularized.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–38**
- Cumulative pages audited: **38 of 316 (12.03%)**
- Cumulative corrected or expanded page records: **26**
- Cumulative audited pages requiring no change: **12**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **278 pages**
- Next self-contained unit: **Part I Chapter 2 — Conventions of Usage, PDF pages 39–50**
