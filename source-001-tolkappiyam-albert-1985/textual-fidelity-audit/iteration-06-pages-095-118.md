# Textual-Fidelity Audit — Iteration 06

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **95–118**  
Unit: **Part I Chapter 7 — உயிர் மயங்கியல் / A Chapter on the Changes in Usage with Vowels**

## Result

**PASS WITH CORRECTIONS**

Every physical page in Chapter 7 was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **24**
- Pages requiring corrections: **24**
- Pages exact as already transcribed: **0**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Corrected pages

| PDF page | Correction made | Commit |
|---:|---|---|
| 95 | Restored scan-faithful Tamil wording and joins, including `வேற்றுமை யல்வழிக்`, `தத்தம்`, `எனவென்`, and `வரினே`. | `3755e2c47e94e02cd43cc6936153cca486967714` |
| 96 | Restored the printed dash headings, `inbetween-`, the omitted `| in |`, and the source’s `infinite` wording. | `6a02f901d7185d9618ab2a18b10cf950de18b846` |
| 97 | Restored edition-specific Tamil forms and joins, including `தொழிலிறு`, `இறும் யகரங்`, and `தொடரல்`. | `f110338db4a3bdfb59ec0b593b47d1af19b07dbc` |
| 98 | Restored printed headings and source forms including `infinite`, `verbal phase`, `ama`, `vāliya`, and `la`/`ra`. | `407ae51af4da846badf515d98ecbb4d258554376` |
| 99 | Restored Tamil joins and wording including `அத்தவண்`, `உருபியல்`, and `ஒரு பெயர்த்`. | `71279c6877d5274bcab9f5653145ccdd8eea12f1` |
| 100 | Restored dash headings and the printed grammatical form `hold good`. | `c9d463cb302a7032d907a23c18d5de836307e154` |
| 101 | Restored Tamil wording and preserved the printed verse number `30`, where the sequence indicates 230. | `9e699aee9ffdd6831bc855aa89aa4dfa7525648e` |
| 102 | Restored the printed `| ā |` in verse 227 and the source’s structural headings. | `e7aac3fc59d1c0b21b367048c098e6ea6970b1c3` |
| 103 | Restored Tamil spacing, joins, and source-specific forms throughout verses 236–243. | `92c8d79391491477353974a36d435b10bf30a25c` |
| 104 | Restored printed dash-and-symbol headings, including `——empty morphs` and `— = elements`. | `722c8ee9009e86c594e1f86480532d4067c2c65f` |
| 105 | Restored Tamil forms including `நாண்முன்` and `இடம்வரைக்`. | `9440c7a944855cc0fbe3760d70b7b647af5e2f8d` |
| 106 | Restored source headings, `puli`, lower-case `undoubtedly`, and the printed transliteration `mi`. | `f66029f9189bffc580a0d8724b366ccb8f96a09f` |
| 107 | Restored scan-faithful Tamil joins and wording in verses 252–259. | `f4df3f9abaac0acb6c8eab92c9900d57537e3a58` |
| 108 | Restored dash headings and the printed footer `T—6`. | `745528c781531a2242365452749b5aef6563b023` |
| 109 | Restored Tamil joins and edition-specific wording in verses 260–268. | `f44769a0a3340d02df843dde15448b051b8c2c56` |
| 110 | Restored printed headings, including the distinctive `—after......`. | `6e4c240f9ec26a7b8550c5a525d79c25fa8c64c0` |
| 111 | Restored Tamil forms including `ஆயியல் பின்றே`, `மாறுகோள்`, and multiple printed joins. | `814302359bf808dec49c918123e07099b959ce06` |
| 112 | Restored source headings including `— + | iṉ | +` and `with—`. | `b834c217fa0dfcaad2265669a9f3558b04e8197a` |
| 113 | Restored scan-faithful Tamil wording and joins across verses 279–288. | `b4c6ed39e07d5d7423e63fc13806f4e3a58ee65b` |
| 114 | Restored printed headings and preserved verse number `236`, where the sequence indicates 286. | `52e375b17830b405ba1dcc35ab52a5a0011faf99` |
| 115 | Restored Tamil forms, preserved printed verse number `291` where the sequence indicates 294, and retained the printed final comma. | `8efcdae93b0fab6d86ff6e36244bb707f9f047db` |
| 116 | Restored the page’s printed structural headings and symbols. | `d5352a1b3e4c61eb8b10596655f11b9dc09cebd7` |
| 117 | Repaired the page-boundary continuation by removing an unprinted trailing dash after `the`. | `d56f9f70703107dcf3ebe8bb82591532d00937ec` |
| 118 | Removed the unprinted leading dash before the continued word `structure` and restored `mi` and `e` as printed. | `6c56b56ee6696ed3d39da055cc00d5dd679af4b1` |

## Numbering irregularities preserved

The audit found and documented three visibly printed numbering irregularities rather than silently regularising them:

- PDF page 101 prints **30**, where the sequence indicates **230**.
- PDF page 114 prints **236**, where the sequence indicates **286**.
- PDF page 115 prints **291**, where the sequence indicates **294**.

## Correction categories

- Tamil characters, joins, separations, and edition-specific orthography
- English wording altered or regularised during the first transcription
- Transliteration letters and vowel lengths
- Standalone dash, symbol, and continuation headings
- Printed verse-number irregularities
- Page-boundary continuation handling
- Source punctuation, capitalisation, and footer notation

## Method

All 24 source pages were rendered directly from the attached PDF and visually compared with the repository records. Tamil verse text, English translation, transliteration, headings, punctuation, notes, numbering, and page continuations were checked at enlarged resolution. The edition’s printed forms—including apparent spelling, grammatical, and numbering errors—were preserved rather than silently corrected.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–118**
- Cumulative pages audited: **118 of 316 (37.34%)**
- Cumulative corrected or expanded page records: **89**
- Cumulative audited pages requiring no change: **29**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **198 pages**
- Next self-contained unit: **Part I Chapter 8 — புள்ளி மயங்கியல் / A Chapter on the Changes in Usage with Consonants, PDF pages 119–146**
