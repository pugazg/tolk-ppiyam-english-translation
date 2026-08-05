# Textual-Fidelity Audit — Iteration 07

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **119–146**  
Unit: **Part I Chapter 8 — புள்ளி மயங்கியல் / A Chapter on the Changes in Usage with Consonants**

## Result

**PASS WITH CORRECTIONS**

Every physical page in Chapter 8 was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **28**
- Pages requiring corrections: **26**
- Pages exact as already transcribed: **2**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **145 and 146**. Page 145 contains notes 30–36; page 146 is the retained blank archival page with faint reverse-side show-through.

### Corrected pages

| PDF page | Correction made | Commit |
|---:|---|---|
| 119 | Restored scan-faithful Tamil joins, separations and wording in verses 297–304. | `2080685c20fe0a0ed439d21e92a9e624e2db4d3c` |
| 120 | Restored title capitalisation and the printed dash continuation headings. | `4408332bc254b6804aca9bfb6d5382c4130bfacb` |
| 121 | Restored edition-specific Tamil forms throughout verses 305–313. | `0f099dadc4fc73d78965b07ea6a6be50baee7f87` |
| 122 | Restored the page’s symbol headings and the printed plural wording in verse 306. | `525237c3f908a43f7aa16dcd66032d53157c406b` |
| 123 | Restored Tamil joins, word divisions and morphology-specific printed forms in verses 314–321. | `2f539e0ffdbee7cc8cfc370507471aa925190225` |
| 124 | Restored dash headings, source punctuation and the printed `T—7` footer. | `fc28f5e4830419dc88e89f574a59bf4c4bc52dd7` |
| 125 | Restored scan-faithful Tamil text and preserved the printed verse number `328`, where the sequence indicates 322. | `bb3859f68524032b984d2f5fa295b0ee62851f08` |
| 126 | Restored all printed continuation headings, including the doubled-dash gerunds heading. | `1b68b6a8169882fea7da6c7ff8ce1355d4d45d3d` |
| 127 | Restored Tamil joins and edition-specific wording in verses 330–338. | `76c7a8f978ad77856114815e7734f31a8e02fdd9` |
| 128 | Restored source errors and irregular wording including `sholars`, `taeks`, and `of the | e |`, plus the printed headings. | `eabc9c1846a2f700b23cecd6e8e23d95dc963b1f` |
| 129 | Restored Tamil punctuation, joins and verse-final forms in verses 339–347. | `3e8d9360ff322a3d43e53f7010149195f4b8c99c` |
| 130 | Restored the printed headings and removed the unprinted final period from verse 345. | `542c3ced5bcb265c035b6c5e6a41fb529177d323` |
| 131 | Restored Tamil text in verses 348–355 and preserved the printed verse number `34`, where the sequence indicates 349. | `705fe07b75a4033860da736868f1f71b14e4d83a` |
| 132 | Restored the complete set of printed dash headings. | `19cf4c95fa2b3be5f59ca6a8e61025ec16599c1f` |
| 133 | Restored scan-faithful Tamil wording and joins across verses 356–365. | `d0cb650c4a82e23dd3eb7962fc3fd7f5f27b9b83` |
| 134 | Restored printed headings and preserved verse number `353`, where the sequence indicates 358. | `e9526b7aa9333006180ab8a0d6b7c67a41bec99d` |
| 135 | Restored Tamil characters, joins and source-specific divisions throughout verses 366–374. | `b97053f8d9fdb774aff25e1cbecf26d1f412bca4` |
| 136 | Restored the page’s dash-and-symbol heading structure. | `50c2dc161b8b49a8cb1c4a5517b8b0a7e9732ba7` |
| 137 | Restored Tamil joins and preserved places where the source prints no verse-final punctuation. | `ebcc271234bba11d7eeb72f196210d571e23c8fc` |
| 138 | Restored source forms including `nāi`, the malformed `| u—`, `veiyl`, and printed list punctuation. | `531a81c1410389b2ee66ac12a0ce076293b6b1dd` |
| 139 | Restored Tamil wording, joins and unpunctuated verse 388. | `68d10961f8e8bb3b1817fe761e2ef46b39f32a97` |
| 140 | Restored headings, source forms `tamil` and `numbes`, the `T—8` footer, and preserved printed verse number `381` where the sequence indicates 388. | `f017a3e826237c02e101306e8f7c765899f004ef` |
| 141 | Restored scan-faithful Tamil text across verses 393–401. | `8b659c1fc305d9e6ca25780f8de0835d5ad4facd` |
| 142 | Restored headings and source errors including the missing opening bar before `ṇ |` and `occours`. | `43c6b20b9d9f06e5d44b78e33c7a57041af785d7` |
| 143 | Restored Tamil joins and places where the source has no final punctuation. | `4d1064335f5f65c2debcc44cbcd718864f81a7bd` |
| 144 | Restored the printed headings, including `— = | veyil | .`. | `ae6c24f0b762bb806a5971b11150244d76fba2c6` |

## Numbering irregularities preserved

Four visibly printed numbering irregularities were retained and documented rather than silently regularised:

- PDF page 125 prints **328**, where the sequence indicates **322**.
- PDF page 131 prints **34**, where the sequence indicates **349**.
- PDF page 134 prints **353**, where the sequence indicates **358**.
- PDF page 140 prints **381**, where the sequence indicates **388**.

## Correction categories

- Tamil characters, joins, separations and edition-specific orthography
- English source wording, spelling errors and malformed notation
- Transliteration letters and symbols
- Standalone dash, symbol and continuation headings
- Printed verse-number irregularities
- Verse-final punctuation and deliberate absence of punctuation
- Printed page footers and physical page structure

## Method

All 28 source pages were rendered directly from the attached PDF and compared visually with the repository records. Tamil verse text, English translation, transliteration, headings, punctuation, notes, numbering and the concluding blank page were checked at enlarged resolution. The scan remained the controlling source; apparent spelling, grammatical, symbol and numbering errors were preserved rather than silently corrected.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–146**
- Cumulative pages audited: **146 of 316 (46.20%)**
- Cumulative corrected or expanded page records: **115**
- Cumulative audited pages requiring no change: **31**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **170 pages**
- Next self-contained unit: **Part I Chapter 9 — குற்றியலுகரப் புணரியல் / A Chapter on the Changes in Usage with the Shorter u, PDF pages 147–167**
