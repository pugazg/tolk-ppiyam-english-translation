# Textual-Fidelity Audit — Iteration 03

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **39–50**  
Unit: **Part I Chapter 2 — மொழி மரபு / Conventions of Usage**

## Result

**PASS WITH CORRECTIONS**

Every page in the range was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **12**
- Pages requiring corrections: **7**
- Pages exact as already transcribed: **5**
- Missing page files: **0**
- Empty page files: **0**
- Unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **39, 41, 45, 48 and 49**.

### Corrected

| PDF page | Correction made | Commit |
|---:|---|---|
| 40 | Restored the printed wording `if the six occur`, the heading `Final position—`, and the comma ending verse 39. | `ebd370d588ab4894426259cc1ef15b5b3c5c931b` |
| 42 | Restored `additions`, printed `| ou |`, two standalone dash headings, and the source punctuation in the consonant-cluster list. | `3752375f076ae1458bed1328b8cb593f66f41c2d` |
| 43 | Restored the physical three-line layout of verse 53 instead of combining its wrapped middle line. | `d6bfc5aed969acb3c677df4889f14b46aaa8bce7` |
| 44 | Restored the standalone dash headings, `| polum |`, `Phonoemic`, `Dipthong`, and the printed `| ṉ |` symbol after enlarged visual checking. | `cfa4127394d2106bfe0a564ba9677ca5ee4fb5e6`, `6882e80fba97660b1a2283b57116dfbab3447812` |
| 46 | Restored the printed `withall` and the omitted `| a |` in verse 62. | `14a9ece90f88f0d91ca6c3cb298c628d3c2f52a2` |
| 47 | Corrected the Tamil source to printed `என வரும்` and `ஏ ஓ`. | `fe9bb1055ede5eb6458196cbbe05f254653a29bb` |
| 50 | Restored the semicolon in the eleven-consonant list and removed the period not printed after verse 82. | `e87314223b9a4d5986031f6a67c4366c94cc722c` |

## Correction categories

- Printed source errors and irregular spellings that had been silently normalized
- Omitted source content
- Tamil character and word-form fidelity
- Transliteration symbols
- Heading and list punctuation
- Verse-final punctuation
- Physical line layout within a Tamil sūtra

## Method

Each source page was rendered at high resolution and compared directly with the repository record. Ambiguous small symbols were enlarged before adjudication. Tamil source pages, English translation pages, headings, sūtra numbers, transliteration marks, punctuation and lineation were checked. Source irregularities were preserved rather than editorially improved.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–50**
- Cumulative pages audited: **50 of 316 (15.82%)**
- Cumulative corrected or expanded page records: **33**
- Cumulative audited pages requiring no change: **17**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **266 pages**
- Next self-contained unit: **Part I Chapter 3 — A Chapter on the Production of Sounds, PDF pages 51–58**
