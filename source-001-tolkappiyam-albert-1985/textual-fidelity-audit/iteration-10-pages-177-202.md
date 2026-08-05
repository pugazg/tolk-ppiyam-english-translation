# Textual-Fidelity Audit — Iteration 10

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **177–202**  
Units:

- **Part II Chapter 1 — கிளவியாக்கம் / Formation and Distribution of Morphemes**, PDF pages 177–194
- **Part II Chapter 2 — வேற்றுமையியல் / A Chapter on the Cases**, PDF pages 195–202

## Result

**PASS WITH CORRECTIONS**

Every physical page in both chapters was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **26**
- Pages requiring corrections: **19**
- Pages exact as already transcribed: **7**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **180, 184, 192, 194, 196, 198 and 202**.

Page 202 is the retained blank archival page with faint reverse-side show-through.

### Corrected pages

| PDF page | Correction made | Commit |
|---:|---|---|
| 177 | Restored scan-faithful Tamil joins, divisions and wording in verses 1–7. | `a3b2646cfa5075eaa5c63b4d1570d494ccacaee3` |
| 178 | Restored the printed extra bar after `mār` and the superscript note marker in verse 7. | `ee62330aadc4396aa630a56892b241abc0535c0a` |
| 179 | Restored Tamil joins, edition-specific word divisions and deliberately unpunctuated verse endings in verses 8–16. | `5d58384b0987f92d5bdcf78dd7ae5a91611b5192` |
| 181 | Restored scan-faithful Tamil forms throughout verses 17–25. | `f49ed9fbb19d7805c998b86873f2935b9007c5cb` |
| 182 | Restored printed dash headings and heading-final punctuation. | `0b4166fc7bae020a1f1fbfced6fe1e99db73bff0` |
| 183 | Restored Tamil joins, source word divisions and unpunctuated endings in verses 26–33. | `da65cafc49639ca2b6a4cca8b80fb963fcd7cb0a` |
| 185 | Restored scan-faithful Tamil wording and joins in verses 34–41. | `77805869a684ce012c7274c374499d63a909a5ef` |
| 186 | Restored the standalone continuation-dash heading before verse 34. | `80c797b0ac65a416a74313249fd67962d2ccc114` |
| 187 | Restored Tamil joins, wording and printed absence of final punctuation in verses 42–49. | `d24a8a0c0913095a1f1b0e2ad91a93c0f4bad5b2` |
| 188 | Restored four standalone continuation headings before verses 44–47. | `1bec6e5f143c9c22866bf114f05b68d82b52e172` |
| 189 | Restored scan-faithful Tamil forms throughout verses 50–55. | `be2043cec3cde31eda272ac010cc8a3460edbd45` |
| 190 | Restored the source’s continuation-heading structure before verses 53–55. | `dc2ce0ab6e123ca0014dd9fa1e2e4a06fc001be4` |
| 191 | Restored Tamil characters, joins and source-specific divisions throughout verses 56–62. | `ff249da7900b7b8eee64d13f49b8b65bd7bbe1b6` |
| 193 | Restored the source’s spaces around colons in the bibliographic citation. | `2f21f98482810dde75c472611d1e61536d61e7bd` |
| 195 | Restored scan-faithful Tamil joins and wording in verses 63–69. | `7ec8ee2e03b01c7c0c8588f98c809dcadedb717e` |
| 197 | Restored Tamil joins and the printed form `முதலில்` in the case descriptions of verses 70–74. | `c12a7e7fc58e02146fba632ff6adf41d2df6669c` |
| 199 | Restored the page-boundary continuation and scan-faithful Tamil divisions in verses 74–79. | `7bed84205fd27f23d88beff9bed776d565460176` |
| 200 | Restored the printed source spacing error `instrument,association`. | `48c80e3399d5ced55c0f6a666da6363b2d53ee6e` |
| 201 | Restored `Np + Vp`, source forms `bythe` and `market`, malformed quotation punctuation and the irregularly punctuated serial list. | `f3fcd2b5c78901c20e0b88e419e9ea7344784b81` |

## Correction categories

- Tamil characters, joins, separations and edition-specific orthography
- Deliberately absent verse-final punctuation
- English source spelling, spacing and malformed punctuation
- Transliteration notation and superscript note markers
- Standalone dash and continuation headings
- Bibliographic punctuation
- Page-boundary continuation

## Method

All 26 source pages were rendered directly from the attached PDF and compared visually with their repository records. Tamil verse text, English translation, headings, transliteration, punctuation, footnote markers, notes and the concluding blank page were checked at enlarged resolution. The scan remained the controlling source; visible errors and irregularities were preserved rather than silently regularised.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–202**
- Cumulative pages audited: **202 of 316 (63.92%)**
- Cumulative corrected or expanded page records: **156**
- Cumulative audited pages requiring no change: **46**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **114 pages**
- Next self-contained unit: **Part II Chapter 3 — வேற்றுமை மயங்கியல் / A Chapter on the Case-marker Substitution, PDF pages 203–212**
