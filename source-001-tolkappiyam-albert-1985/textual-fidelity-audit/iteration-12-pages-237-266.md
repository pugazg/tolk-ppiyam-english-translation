# Textual-Fidelity Audit — Iteration 12

Audit date: **2026-08-06**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **237–266**

Units:

- **Part II Chapter 6 — வினையியல் / A Chapter on the Verbs**, PDF pages 237–252
- **Part II Chapter 7 — இடையியல் / A Chapter on the Bound Morphemes**, PDF pages 253–266

## Result

**PASS WITH CORRECTIONS**

Every physical page in the two chapters was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **30**
- Pages requiring corrections: **23**
- Pages exact as already transcribed: **7**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **239, 249, 250, 257, 261, 263 and 266**.

Page 266 is the retained blank archival page with faint reverse-side show-through.

### Corrected pages

| PDF page | Correction made | Commit |
|---:|---|---|
| 237 | Restored `அம்ஆம்` and the printed Tamil form `குற்றிய லுகரமொடு`. | `6f81f30ac37594757a9a3f5ec0f6d517984d0e6f` |
| 238 | Restored printed punctuation and separated the `——singular——` and `ceyku` headings from their verse numbers. | `cbf869fde49fd61341ccbf4500f682afd0a41af7` |
| 240 | Restored standalone symbolic headings and the printed form `Of these-the`. | `e82ee5cdce7b7f1b7e7d62a6b28c53d6e0f33b09` |
| 241 | Restored the printed Tamil join `ஆஆ`. | `a403b970683421b9bdefaddc24e5580fe90360ed` |
| 242 | Restored continuation headings and source transliteration `uṭaia`; corrected continuation metadata. | `5c92b0607d324b03b717392d5b0816082c5dfb8b` |
| 243 | Restored the printed Tamil form `தன்மை யாயீ`. | `c5bf9db24dfbf749727abd76c5f87fe97f27f5df` |
| 244 | Removed a non-printed editorial continuation heading and restored the standalone `Other——` heading. | `c0f6ff42481c66c86aa9583f8ec2fbaf9d7d67e2` |
| 245 | Restored the printed division `முடியா தடுக்குந`. | `ca3b28fecfd71716c8e82fda84c4ad9bb8cd420c` |
| 246 | Restored continuation headings and source spacing `mo rphemes`. | `abfd6509705b5cd18cebbb82e5378d6803db036f` |
| 247 | Restored scan-faithful Tamil divisions and forms including `வினாவிடை` and `இயற்கையுந்`. | `6972cf975a7f44da722437b28ff1338f591f7a56` |
| 248 | Restored the printed space before the comma following `ceytu`. | `60cf5d6d727a7e7863577207ba73c1b23c9feca1` |
| 251 | Removed a non-printed editorial Notes heading and preserved source form `vllar`. | `dbb2a0e2f9a68e5a82685aceed2b1e830063b88d` |
| 252 | Removed a non-printed Notes heading, restored source punctuation and added footer `T—15`. | `7f784d42214443d6ad7f477691d9408aa8b50b84` |
| 253 | Restored scan-faithful Tamil text including `குதவும்`, `வருநவும்` and `கழிவே யாக்கம் மொழியிசைக்`. | `ca4827c385cb186d7c461071f68304333de05288` |
| 254 | Preserved source typos `casee` and `m,rphs` and restored standalone symbolic headings. | `3d39f2227104767fac0518de04dd9f6d53e2758e` |
| 255 | Corrected verse 251 to the printed `ஓகா ரம்மே`. | `4fc81b40dd49834c92687ee6b5e0335d139dfc91` |
| 256 | Preserved source forms `impl'ied` and `si x` and restored standalone headings. | `9599018c327d38c22708d525b4507af545c40455` |
| 258 | Restored the standalone continuation dash before verse 266. | `d4e3fc5c579e818e2f2978fb80df5beea12e09fa` |
| 259 | Restored Tamil forms `ஆங்க வரை யசை`, `ஈரள`, and `வேறு படுதல்`. | `f7f1e2ac48d51ad1bc1f26bf4a9f0277f2365efc` |
| 260 | Preserved the printed incomplete verse number `2 9.`, documented its sequence value, and restored source forms `rightiy` and `emphy`. | `c196aa52a3034cd401f14b94f5362423a332dce0` |
| 262 | Restored standalone `——placement` and `——exclusiveness` headings. | `e489438b9b781f015ddb6884e93b554a85b9d4a8` |
| 264 | Restored symbolic headings and the printed space before the period after `untu`. | `eccd7081161a3b7b28e84cdf42a4e974921f139c` |
| 265 | Removed a non-printed editorial Notes heading. | `721b484fa0f746c9abbd870ba512cd1924b4107f` |

## Correction categories

- Tamil characters, joins, separations and edition-specific orthography
- Printed verse-number irregularities and explanatory metadata
- Standalone dash, symbolic and continuation headings
- Transliteration, punctuation and malformed source notation
- English spelling and spacing irregularities
- Footers and page-level archival structure
- Removal of editorial headings not present on the scan

## Method

All 30 source pages were rendered directly from the attached PDF and compared visually with their repository records. Tamil verses, English translations, headings, transliteration, punctuation, notes, footers and the concluding blank page were checked at enlarged resolution. The scan remained the controlling source; visible errors and irregularities were preserved rather than silently regularised.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–266**
- Cumulative pages audited: **266 of 316 (84.18%)**
- Cumulative corrected or expanded page records: **212**
- Cumulative audited pages requiring no change: **54**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **50 pages**
- Next self-contained unit: **Part II Chapter 8 — உரியியல் / A Chapter on the Free Morphemes, PDF pages 267–288**
