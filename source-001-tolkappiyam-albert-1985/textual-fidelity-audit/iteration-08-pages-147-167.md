# Textual-Fidelity Audit — Iteration 08

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **147–167**  
Unit: **Part I Chapter 9 — குற்றியலுகரப் புணரியல் / A Chapter on the Changes in Usage with the Shorter | u |**

## Result

**PASS WITH CORRECTIONS**

Every physical page in Chapter 9 was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **21**
- Pages requiring corrections: **16**
- Pages exact as already transcribed: **5**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **148, 154, 156, 166 and 167**.

### Corrected pages

| PDF page | Correction made | Commit |
|---:|---|---|
| 147 | Restored scan-faithful Tamil joins, separations and edition-specific forms in verses 407–413. | `08811d33c35f345ad154d7e9c4445c97ae56060c` |
| 149 | Restored Tamil word divisions, joins and the printed multiline structure in verses 414–422. | `fbbe43e361515a07b2fa7daee71b8ed3babf02c2` |
| 150 | Restored the standalone dash heading before verse 417 and the printed form `hardconsonantal`. | `c5f83ad567acbc27645739fac12350ed402009d8` |
| 151 | Restored scan-faithful Tamil wording and joins throughout verses 423–431. | `dceb52fccf433f5c9a21d34adc9eb61624f24228` |
| 152 | Restored the printed heading `=exists` before verse 431. | `b38b531657bca9a30d49f80b4114bf3f6e96a0d5` |
| 153 | Restored Tamil joins, word divisions and edition-specific forms in verses 432–439. | `52ea2c33edaf1f8e3ccdc0682ae9c76d58bfd5fc` |
| 155 | Restored scan-faithful Tamil text throughout verses 440–448. | `3606ebff7eac48fbf47352f3234f9ba644774603` |
| 157 | Restored Tamil joins and source punctuation, including the printed comma after verse 453. | `aa46b2f415f5754bf008cbeb87942279f088d8d6` |
| 158 | Restored the printed comma ending verse 449 instead of a period. | `c0ac5408188d6e70421955bb74c036f2b7c2be79` |
| 159 | Restored Tamil joins, spacing and edition-specific wording in verses 458–467. | `4904c07d6f4972a18469d76858232a4dc9b54417` |
| 160 | Restored standalone continuation-dash headings before verses 465–467. | `0dc764d229f3045295509d03294f6a2f9c195b37` |
| 161 | Restored scan-faithful Tamil forms throughout verses 468–475. | `18af601b2a03883ed2954d156b5e00361bf71c01` |
| 162 | Restored standalone continuation-dash headings before verses 468–470. | `a376fea5ae87f51f36cda5334ca7d5d818f3b3eb` |
| 163 | Restored Tamil characters, joins and printed word divisions throughout verses 476–482. | `05a5063c57c4cdd17a7053bdfb9e066d1f242531` |
| 164 | Restored the source’s printed spelling `apinion` rather than silently regularising it. | `8e36ea3c59e9f5e9a0030de335ee03fd1e0afdbd` |
| 165 | Restored the printed Tamil division `நாட்டத் தென்மனார்` in verse 483. | `d7f832800a9ee0ea9193f42dbb7cc0a69b30e881` |

## Correction categories

- Tamil characters, joins, separations and edition-specific orthography
- English source spelling and unregularised wording
- Standalone dash and symbol headings
- Printed line structure
- Verse-final punctuation

## Method

All 21 source pages were rendered directly from the attached PDF and compared visually with their repository records. Tamil verse text, English translation, headings, transliteration, punctuation, notes and page structure were checked at enlarged resolution. The scan remained the controlling source, and apparent spelling or grammatical irregularities were preserved rather than silently corrected.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–167**
- Cumulative pages audited: **167 of 316 (52.85%)**
- Cumulative corrected or expanded page records: **131**
- Cumulative audited pages requiring no change: **36**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **149 pages**
- Next self-contained unit: **Part I Research Topics, Part I Index, blank archival page and Part II title page, PDF pages 168–176**
