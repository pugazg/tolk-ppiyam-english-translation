# Textual-Fidelity Audit — Iteration 01

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **1–28**  
Scope: complete front matter and the Part I — Phonology title page

## Result

**PASS WITH CORRECTIONS**

Every page in the range was visually compared against its corresponding Markdown file.

- Pages audited: **28**
- Pages requiring corrections or fuller archival description: **17**
- Pages exact as already transcribed: **11**
- Missing page files: **0**
- Empty page files: **0**
- Unresolved source readings retained without guessing: **2 locations**

## Page disposition

### Exact — no repository change required

PDF pages **3, 4, 14, 16, 17, 19, 20, 22, 24, 25 and 28**.

### Corrected or expanded

| PDF page | Correction made | Commit |
|---:|---|---|
| 1 | Replaced generic cover annotations with the readable English seal legend; explicitly recorded that the Tamil seal legend and handwritten library markings cannot be transcribed confidently. | `d1a0b6f6bee9ffd823a3315a5b4f5c43cdde73fa` |
| 2 | Restored the printed title punctuation, author qualifications, address lineation, `21 X 14 cms`, page-count punctuation and other bibliographical formatting instead of normalized prose. | `f8e528f95da4cd0423fdd1866628d02dd0a17b98` |
| 5 | Removed an invented continuation hyphen at the start of the page and refined the note on the damaged `Aḵṟiṇai` reading. | `c1e9b39ed0f810a148cc9c6bb5c0e000290f4df6` |
| 6 | Restored the printed form `difererent`. | `e9629c626eb1e0609ff6ac8a9fcb8b0a5235500b` |
| 7 | Restored the printed initials `S.V. Subramanian`. | `43d27f41a4ee54cc542f2d3155a70dd98aafc5f4` |
| 8 | Corrected the printed contents entry for “An Approach to Tolkāppiyam” from `viii` to `vii`; restored spacing in `| u |`. | `abaa57805c42d71cc6363e0fee9d57050a3ce21f` |
| 9 | Restored diacritics in names and the edition’s printed title form `Thoikāppiyam`. | `933b14ebf4d6aa16678b79b577cf138c78a9b095` |
| 10 | Restored bibliographical names, diacritics, the shorter printed title `Compilation of Commentaries`, `Thoikāppiyam` and `Patipukaḷ`. | `a7cc01a6813527a7045a437e74faee896c88202a` |
| 11 | Restored the printed wording `how for the consciousness`. | `e4d16cb14fb804c8abc0c463c9633b7dc2a06b0d` |
| 12 | Restored the printed punctuation `co.relate`. | `3035e5227ce056ebaa6bee975adda509782dbc96` |
| 13 | Restored the printed `ilampūraṇar` and `layou`. | `554c6b34e7c0bc665d0735ee1a134f9f5f284e1a` |
| 15 | Restored the scanned Latin form `utrem`. | `691761faca37bb946518880adbfe404ef6226bb1` |
| 18 | Restored the printed forms `betweet`, `lostly` and `versse`. | `e48dd3c478295269821aa04232f5a76e3b858c64` |
| 21 | Restored the printed form `rhythmt c`. | `66a89c9a11766b8add028eb18099bbd2e717303d` |
| 23 | Restored `syas`, `succint`, `words!`, `so me` and the printed author initials `J.D.O’ Connor`. | `d4481682b8dc4662f991c53ab85a28e2bdbfec6c` |
| 26 | Restored Tamil vowel form `ஒள` and the source wording for the dash-below transliteration. | `0e3effcbc9b8783cb0a2eb343112f66594c6a014` |
| 27 | Restored `the the`, `Transliteratton`, `isf ollowed` and the semicolon in the quoted reference title. | `2c973e3c0f773549682f67099734a65a6d465c41` |

## Correction categories

- Source spelling or typographical irregularities that had previously been normalized
- Bibliographical names and transliteration diacritics
- Punctuation, initials and internal word spacing
- Contents-page numbering
- Tamil transliteration-table characters
- Page-continuation handling
- Archival description of non-body cover text and markings

## Unresolved source readings

1. **PDF page 1:** the Tamil legend around the institutional seal is too small and faint for a confident diplomatic transcription; the handwritten library markings are only partly legible. Both are described but not guessed.
2. **PDF page 5:** the damaged character sequence in `Aḵṟiṇai` remains uncertain and is explicitly documented in the page note.

No other uncertain reading remains in pages 1–28 after this pass.

## Method

Each source page was raster-rendered and visually compared with its Markdown record. The audit checked wording, source typos, punctuation, diacritics, tables, headings, printed page labels, page continuations and non-textual archival annotations. Source irregularities were preserved rather than silently corrected.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–28**
- Cumulative pages audited: **28 of 316 (8.86%)**
- Remaining for textual-fidelity audit: **288 pages**
- Next self-contained unit: **Part I Chapter 1, PDF pages 29–38**
