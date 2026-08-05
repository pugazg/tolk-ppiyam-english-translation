# Textual-Fidelity Audit — Iteration 04

Audit date: **2026-08-05**  
Source: `TVA_BOK_0013548_Tolkāppiyam.pdf`  
Audited physical PDF range: **51–84**  
Units:

- **Part I Chapter 3 — பிறப்பியல் / A Chapter on the Production of Sounds**
- **Part I Chapter 4 — புணரியல் / A Chapter on the Grammar of Morphophonemic Change**
- **Part I Chapter 5 — தொகை மரபு / Conventions of Morphophonemic Grammar and Usage**

## Result

**PASS WITH CORRECTIONS**

Every page in the combined three-chapter range was freshly raster-rendered and visually compared against its corresponding Markdown file.

- Pages audited: **34**
- Pages requiring corrections: **28**
- Pages exact as already transcribed: **6**
- Missing page files: **0**
- Empty page files: **0**
- New unresolved source readings: **0**

## Page disposition

### Exact — no repository change required

PDF pages **59, 60, 81, 82, 83 and 84**.

### Chapter 3 corrections — PDF pages 51–58

| PDF page | Correction made | Commit |
|---:|---|---|
| 51 | Restored printed Tamil forms and joins, including `பன்னீ ருயிரும்` and `ஐயென`. | `b448af4c0c424049de6d5dbdcbcf7fb8ce0ad567` |
| 52 | Restored the source punctuation in the rounded-vowels list: no comma after `| o |` and a comma before `and`. | `664d580e2515c2d66cb7e22a6a7c9ef27db60f8c` |
| 53 | Restored `டகார ணகாரப்`, the printed separations `நுனி நா` and `நா நுனி`, and retained the edition’s line forms. | `57915528504cb2ea9db908fa0abdff218d3be494`, `f2d3723b38d8dc6d04e8b125db87e0dcc6ef3784` |
| 54 | Restored the semicolon in the heading `Consonants; | k | and | ṅ |`. | `c90113342dd3a469291a65bf39b5bc00f7585191` |
| 55 | Removed the period not printed after verse 103. | `9e46bab81a19148e3a9e6bb1d15cd179a2cc5010` |
| 56 | Restored the initial dash before verse 98 and replaced two inaccurate paraphrases with the exact printed wording in verses 101 and 103. | `2ac942c3296566ed27a39e624ee963872e148c7f` |
| 57 | Restored the diacritic in the first occurrence of `Ṣankaran`, the printed forms `todgue` and `nos e`, and retained the source’s irregular spelling. | `f337dbbedfd1ced821e42a630f22c2ef423bb3a4`, `f4726819222a926a7a6efa4d2a4206d9713009cf` |
| 58 | Restored the printed join `Notes10.` | `2f2473dcf6bda3da4a2e6a6a9c05567a5a6413a9` |

### Chapter 4 corrections — PDF pages 61–70

| PDF page | Correction made | Commit |
|---:|---|---|
| 61 | Restored `முதலெழுத்து இயையப்`, `நிறுத்த சொல்லும்`, `மெய்பிறிதாகுதல்`, and the printed phrase `புணர்நிலைக்கு உரிய`. | `3e7b9fc8263f779d786c7b06ba7b2e35e44f9b80`, `bd8bba6ffe01a8557ef3590a3fac3a90eff5d629` |
| 62 | Restored source errors `Additior` and `morphonoemic`. | `e18eab2a04933c6e19e325015b98de6b610d9a66` |
| 63 | Restored multiple printed Tamil forms and spacing in verses 121–126, including `இன்னி னிகர மாவின்`, `சுட்டுமுத லைம்முன்`, `ஆனி னகரமும்`, `நாண்முன்` and `யில்லை`. | `37c395d39205a1e7d38ba6d8201e8549be09d055`, `d71c863188cf2c858f04fe5b6d9234245683cdc8` |
| 64 | Restored the printed transliteration distinctions `iṉ`, `oṉ`, `āṉ`, `aṉ` and `ṟ` throughout verses 120–125. | `6690c266777bc35200f5f378f57d884b3e5fc385` |
| 65 | Restored printed forms across verses 127, 130, 132 and 133, including `இக்கி னிகரம்`, `ஙஞந வாகும்`, `இன்னென`, `வேற்றுமை உறுபிற்கு`, `பெயரும்` and `இயலுஞ்`. | `4c3fa18f8ba37473f9f9f358c42bac412d3c79f3` |
| 66 | Restored the standalone dash heading before verse 128, the printed `iṉ` diacritics in verse 132, and removed an unprinted final period. | `9931ac6bc9c4a2861b931c0b1edfb747fd55f9f4`, `68dd5b30a885fcb78f0f53c2500645de6bd25822` |
| 67 | Restored `அவற்றிமுன்`, `மெய் யொடுஞ்`, `உயிர் வரு`, `குற்றெழுத்து உடைய` and `உருபுகொள்ளல்`. | `e0227b28754d5747199d56d7837d60b811d8f514`, `6d5c8720cd428c7b3a620c8eac501e9f42acb1df` |
| 68 | Restored the period in `Three more empty morphs.`, two standalone dash headings and the printed typo `cansonant`. | `273e6c4ca7bc504d10f2ace186793373eb3cfc7a` |
| 69 | Restored the printed Tamil spacing `நிலை இய` and `அவை தாம்`. | `058fd5a334fe1e8eca507e3ae1ec5e9998925856` |
| 70 | Restored the standalone dash heading before verse 143. | `f6dbd20c9f078e962ff7529e1cd016077b06ebac` |

### Chapter 5 corrections — PDF pages 71–80

| PDF page | Correction made | Commit |
|---:|---|---|
| 71 | Restored printed Tamil forms and spacing, including `ஞ நம யவவெனும்` and `தொடர் மொழி யிறுதியான`. | `74fee404174ec035c9512010e2589e29f379fa82` |
| 72 | Restored source errors `thos` and `changee`, and the standalone dash heading before verse 149. | `40b134fffb861c1238ad7c3052e7a171c63a6fab` |
| 73 | Restored numerous edition-specific Tamil forms, including `த ந`, `குநவு மென்று`, `ஞ நம வ`, and the visibly printed `உயிர் றாகிய உயர்திணைப் பெயரும்`. | `15fedf2f4dee333297bd8d91e0b0bbf012e459fc`, `3b7e359c621e353b2a909b3afc8bacdb46ecdf58` |
| 74 | Restored standalone dash headings before verses 151 and 153. | `30d8c0e5ec7f7924a5cb6ddf7c8c564677a8a526` |
| 75 | Restored substantive Tamil readings in verses 157–158, including `தொழிற் சொல் முன்வரின்`, `உரியவை`, `ஒழியாது`, `இயற்கை யாதலும்` and `பிறவுந்`. | `23df29fcc13c0a7b58f9e6c0dd8f62cbe5e57b78` |
| 76 | Preserved the first printed `personal class nouns`, the second printed `personal clas nouns`, and the leading apostrophe before `Similar occurrences`. | `1bae4660080c650ad48c82ff3606b07573d9c096`, `a5acc6417afc0bd34b6191d09a776a4e911ff3f6` |
| 77 | Restored `இஐ` and the printed `வில்லை`. | `712cc7f310a72507eb5c44849555ead8a0489c4d` |
| 78 | Restored source errors `reiations`, `Loug` and `copsonant`. | `4cb7d379c4dd00b4c881fa1508936b1a5fb42b3c` |
| 79 | Restored `வேற்றுமை யியற்கை`, `அளவுங்` and the printed spacing `கச தப`. | `86aa976c9b466a8228e21fa85a5d3178eab94234` |
| 80 | Restored three standalone dash headings and the printed transliteration `Pannai`. | `cbe85394a7d2a6f7b7920eb776c3c9c544b76943` |

## Correction categories

- Tamil characters, word boundaries and edition-specific joins
- Substantive omissions or paraphrases in English translation text
- Transliteration letters and diacritics
- Source spelling and typographical irregularities
- Standalone continuation headings represented by a dash
- Heading, list and sentence punctuation
- Verse-final punctuation and physical lineation

## Method

All 34 source pages were rendered from the PDF and compared directly with their repository records. Ambiguous Tamil forms, transliteration marks and small source errors were checked using higher-resolution rerenders and local crops. The edition’s printed wording—including apparent errors—was preserved rather than silently normalized.

## Progress after this iteration

- Cumulative audited range: **PDF pages 1–84**
- Cumulative pages audited: **84 of 316 (26.58%)**
- Cumulative corrected or expanded page records: **61**
- Cumulative audited pages requiring no change: **23**
- Cumulative unresolved source locations: **2**
- Remaining for textual-fidelity audit: **232 pages**
- Next self-contained unit: **Part I Chapter 6 — A Chapter on the Changes in Usage with Case-markers, PDF pages 85–94**
