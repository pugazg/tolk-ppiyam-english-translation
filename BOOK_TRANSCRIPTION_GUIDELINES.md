# PDF Book → GitHub Markdown Archival Guidelines

## Purpose

This document defines the standard operating procedure for converting scanned or born-digital PDF books into structured, searchable, page-level Markdown repositories.

The primary goal is **archival fidelity**. The repository should preserve what is visibly printed in the source before it is used for search, websites, datasets, translation, annotation, linguistic analysis, retrieval-augmented generation, or other derived work.

> The repository is an archival transcription first, a research corpus second, and an application source third.

---

## 1. Core principles

1. **The source scan controls.** OCR, extracted text, existing editions, dictionaries and general knowledge are aids only.
2. **One physical PDF page equals one Markdown page record.** Never merge, omit or silently reorder physical pages.
3. **Preserve the printed text as printed.** Retain spelling errors, punctuation, spacing, transliteration, numbering anomalies and historical usage.
4. **Do not silently correct the source.** Corrections, modernisations and interpretations belong in a separate derived layer.
5. **Blank pages are records.** Preserve blank pages, image-only pages, advertisements, errata, covers and publication lists.
6. **Uncertainty must be explicit.** Never guess an unreadable character or word.
7. **Structural completeness and textual fidelity are separate quality gates.** A book is not finished merely because every page has a file.
8. **Copyright status and transcription accuracy are separate questions.** A completed audit does not by itself authorise public redistribution.

---

## 2. Project models

### 2.1 One book or one edition

Use one source folder:

```text
source-001-short-title-year/
```

Example:

```text
source-001-tolkappiyam-albert-1985/
```

### 2.2 Multiple editions or source PDFs

Create one folder for each distinct source:

```text
source-001-first-edition/
source-002-revised-edition/
source-003-commentary-edition/
```

Never mix page records from different editions in the same source folder.

### 2.3 Multi-volume works

Use a stable volume hierarchy:

```text
volumes/
├── volume-01/
├── volume-02/
└── volume-49/
```

Each volume must have its own metadata, manifest, contents register, progress tracker and audit reports.

---

## 3. Recommended repository structure

```text
repository-root/
├── README.md
├── BOOK_TRANSCRIPTION_GUIDELINES.md
├── RIGHTS.md
├── SOURCES.md
│
├── source-001-short-title-year/
│   ├── README.md
│   ├── metadata.md
│   ├── manifest.md
│   ├── FINAL-AUDIT.md
│   ├── TEXTUAL-FIDELITY-AUDIT.md
│   │
│   ├── contents-index-chapters/
│   │   ├── contents.md
│   │   ├── chapter-register.md
│   │   └── page-map.md
│   │
│   ├── front-matter/
│   ├── part-01-or-main-text/
│   │   ├── chapter-01-short-title/
│   │   ├── chapter-02-short-title/
│   │   └── ...
│   ├── back-matter/
│   │
│   └── textual-fidelity-audit/
│       ├── iteration-01-pages-001-030.md
│       ├── iteration-02-pages-031-060.md
│       └── ...
│
└── derived/
    ├── README.md
    ├── normalized-text/
    ├── datasets/
    ├── annotations/
    └── search-index/
```

The exact chapter folders may vary by book, but the following separation must remain clear:

- source-faithful page transcription
- structural navigation
- audit records
- derived or normalised outputs

---

## 4. Source intake and provenance

Before transcribing, create a source record containing all available information.

### 4.1 Required metadata

```text
Title:
Original title:
Author:
Editor:
Translator:
Commentator:
Publisher:
Place of publication:
Publication year:
Edition or impression:
Volume number:
ISBN or catalogue number:
Language or languages:
Source PDF filename:
Source website or institution:
Source record URL:
Date accessed:
Physical PDF page count:
Printed page range:
PDF file size:
SHA-256 hash:
Rights or licence status:
```

Do not invent missing bibliographic details. Use `not stated` or `not yet verified`.

### 4.2 Source identity

The original filename and file hash should be retained so that future contributors can confirm that they are working from the same scan.

If the source PDF changes, treat it as a new source version unless byte-level and visual equivalence have been established.

### 4.3 Rights record

Every repository should contain `RIGHTS.md` documenting:

- where the PDF was obtained
- whether the source page states a licence
- whether the work is public domain, openly licensed, permission-based or unresolved
- whether full-text public redistribution is authorised
- attribution requirements
- restrictions on commercial or derivative use
- correspondence or permission received from rights-holders

Never assume that any of the following means open reuse:

- the PDF is downloadable
- the website is a government or library website
- the original work is ancient
- the scan is freely accessible
- no copyright notice appears inside the PDF

A translation, commentary, introduction, index, notes and modern editorial arrangement may carry independent rights even when the underlying ancient work is public domain.

---

## 5. Mandatory startup audit

Before writing page files:

1. Confirm the PDF opens correctly.
2. Record the total physical page count.
3. Inspect the first pages, contents, chapter openings, last pages and any irregular scans.
4. Identify:
   - covers and title pages
   - Roman-numbered front matter
   - contents and indexes
   - chapters or letters
   - Tamil and English alternating pages
   - notes and footnotes
   - blank pages
   - foldouts, illustrations and tables
   - errata and advertisements
5. Create an initial page map and folder plan.
6. Create a manifest with every physical page marked `not-started`.

Do not begin mass transcription before the page structure is understood.

---

## 6. Physical-page rule

### 6.1 File naming

Use zero-padded physical page numbers:

```text
page-001.md
page-002.md
page-099.md
page-100.md
page-316.md
```

The filename always follows the **physical PDF page number**, not the number printed on the page.

### 6.2 One-to-one correspondence

For a 316-page PDF, there must ultimately be exactly 316 page records, including:

- cover pages
- blank pages
- image-only pages
- contents pages
- chapter title pages
- errata
- publication lists

### 6.3 Printed page number

Record the printed page label separately in metadata. It may be:

- Roman numeral
- Arabic numeral
- absent
- duplicated
- incorrect in the source

Do not rename the physical page file to match the printed number.

---

## 7. Page-record metadata

Use YAML front matter. Required fields:

```yaml
---
source_id: source-001-short-title-year
pdf_page: 1
printed_page: null
language: Tamil
status: transcribed
---
```

Recommended optional fields:

```yaml
volume: 1
part: Part I
section_number: 2
section_title: Introduction
chapter_number: 1
chapter_tamil: நூல் மரபு
chapter_english: Conventions of Grammar
page_type: text
verses: 1-8
letters: 3764
notes: 1-3
translation_of: page-029
continuation_of: page-030
continues_on: page-032
blank_reason: no printed text; faint reverse-side show-through
chapter_status: complete
volume_status: complete
rights_status: unresolved
```

Use only fields supported by the source. Do not fill metadata by assumption.

### 7.1 Status values

Recommended controlled statuses:

```text
not-started
transcribed
structurally-verified
textually-audited
unresolved
```

A page should be marked `textually-audited` only after visual comparison with the scan.

---

## 8. Transcription policy

### 8.1 Preserve source wording

Retain exactly what is printed, including apparent errors.

Source:

```text
seccnd person
```

Archival transcription:

```text
seccnd person
```

Do not replace it with `second person` in the archival page record.

### 8.2 Preserve punctuation and spacing where meaningful

Check carefully:

- commas and full stops
- colons and semicolons
- quotation marks
- apostrophes
- em dashes and decorative rules
- punctuation attached to headings
- spaces before punctuation where visibly printed
- joined and separated Tamil forms

Minor Markdown formatting may be used to represent the page, but it must not alter the textual content.

### 8.3 Tamil-script fidelity

Pay special attention to:

```text
ண / ன
ர / ற
ல / ள / ழ
ந / ன
ெ /ே
ொ /ோ
புள்ளி and vowel signs
```

Do not modernise sandhi, word division or orthography.

### 8.4 Transliteration fidelity

Preserve:

- diacritics
- vertical bars or brackets
- capitalisation
- apostrophes
- unusual spellings
- inconsistent transliteration across pages

Do not silently convert the book to a preferred transliteration standard.

### 8.5 Line breaks

Preserve lineation when it carries structural meaning, especially for:

- poems and verses
- numbered rules
- quotations
- lists
- tables
- title pages

For ordinary prose, visual line wrapping caused only by page width may be joined into paragraphs.

### 8.6 Hyphenation

- A word visibly broken at the end of a line within the same paragraph may be joined only when the continuation is certain.
- A word broken across physical pages should remain explicitly traceable through `continues_on` and `continuation_of` metadata.
- Preserve intentional hyphens.
- When uncertain whether a mark is a hyphen or dash, inspect at higher resolution.

### 8.7 Headings

Represent printed headings with Markdown headings.

Do not invent topical headings that do not appear in the scan. Explanatory labels created by the transcriber belong in metadata or derived documentation, not in the source body.

### 8.8 Footnotes and endnotes

Preserve:

- note markers
- note numbering
- note text
- page continuations
- source punctuation

Do not renumber notes for convenience.

### 8.9 Tables

Use Markdown tables when they preserve the reading order and content accurately.

Use a fenced text block when:

- spacing is semantically important
- columns are irregular
- Markdown would force a misleading structure

For complex tables, include a clear archival transcription and optionally add a separate derived CSV.

### 8.10 Images, diagrams and illustrations

For an image-only page:

- create the physical page record
- record that it contains an image
- transcribe any visible caption or labels
- do not invent a visual description as if it were printed text

A separate editorial description may be added under a clearly labelled field such as `editorial_description`.

### 8.11 Blank pages

Never omit a blank page.

Example:

```markdown
# Blank page

No printed text is visible on this physical PDF page. Faint reverse-side show-through appears in the scan.
```

State only what is visibly supportable.

### 8.12 Errata

Transcribe both:

- the original erroneous text on its original page
- the errata entry exactly as printed

Do not silently apply the errata correction to the archival page transcription. A derived corrected edition may apply it separately with a documented link to the errata.

---

## 9. OCR policy

OCR may be used to accelerate drafting, but it is never the authority.

Priority order:

```text
source scan
  > enlarged visual inspection
  > verified transcription
  > OCR output
  > external editions or web copies
  > assumption
```

Rules:

1. Never commit raw OCR as verified text.
2. Tamil OCR requires manual character-level review.
3. OCR confidence scores do not replace visual verification.
4. Repeated OCR failure must not lead to guessing.
5. When a location remains unreadable after reasonable inspection, mark it explicitly.

Recommended uncertainty forms:

```text
[unclear in scan]
[one character unclear]
[reading uncertain: …]
```

Use square brackets only for editorial intervention, never to conceal uncertainty.

---

## 10. Contents, chapter and item registers

Maintain the book's original navigation and a repository-level navigation layer.

### 10.1 `contents.md`

Preserve the original contents page exactly and optionally add a clearly separate repository navigation table.

### 10.2 `chapter-register.md`

Recommended fields:

| Field | Description |
|---|---|
| Chapter or item number | As printed |
| Tamil title | As printed |
| English title | As printed |
| Date | For letters, speeches or documents |
| PDF start page | Physical page |
| PDF end page | Physical page |
| Printed start page | As printed |
| Status | Not started, transcribed or audited |

For letter collections, preserve letter numbers, dates, titles and printed-page starts.

### 10.3 `page-map.md`

Map every physical page to its section:

```text
PDF 001–004  Cover and title pages
PDF 005–012  Foreword
PDF 013–020  Contents
PDF 021–045  Chapter 1
```

---

## 11. Manifest requirements

The manifest is the authoritative page inventory.

Recommended columns or fields:

```text
pdf_page
printed_page
path
page_type
part
chapter
language
status
has_text
is_blank
continuation_of
continues_on
unresolved_count
last_audited_commit
```

Required checks:

- all physical pages appear exactly once
- paths are unique
- no page file lies outside the manifest
- no manifest page lacks a file after structural completion
- page ranges are continuous

---

## 12. Work phases

### Phase 0 — Rights and source intake

Deliverables:

- source metadata
- source URL and access date
- file hash
- rights status
- initial page count

### Phase 1 — Structural inventory

Deliverables:

- folder structure
- complete manifest with `not-started` status
- contents and chapter register
- page map

### Phase 2 — Initial transcription

Deliverables:

- one Markdown file per physical page
- front matter, main text and back matter preserved
- blank and image-only pages represented
- progress tracker updated

Initial transcription may be committed in manageable batches, such as 10–30 pages, provided every file remains page-addressable.

### Phase 3 — Structural completion audit

Verify:

- total files equal total PDF pages
- no missing or duplicated page numbers
- chapter boundaries match the source
- contents and indexes are represented
- blank pages and closing matter are included

Create `FINAL-AUDIT.md` or an equivalent structural-completion report.

### Phase 4 — Textual-fidelity audit

Render each source page and compare it visually against the Markdown record.

Check:

- Tamil characters
- English spelling
- transliteration
- punctuation
- verse and item numbering
- headings
- notes
- line continuation
- tables
- footers
- blank-page descriptions

For maximum traceability, use one correction commit per corrected page during the fidelity audit. If corrections are grouped, the report must still identify every changed page and its commit.

### Phase 5 — Final closure

Deliverables:

- final audit iteration report
- cumulative tracker at 100%
- README updated
- zero remaining pages
- unresolved readings explicitly listed
- source folder marked complete

### Phase 6 — Derived outputs

Only after archival completion, create:

```text
derived/
├── normalized-text/
├── verses.json
├── chapters.json
├── glossary.json
├── search-index.json
├── parallel-text.json
└── annotations/
```

Derived files must clearly state that they are not the archival transcription.

---

## 13. Textual-fidelity audit reports

Store reports under:

```text
textual-fidelity-audit/
```

Naming:

```text
iteration-01-pages-001-030.md
iteration-02-pages-031-060.md
```

Each report must include:

```text
Audit date
Source filename
Audited physical page range
Section or chapter
Pages audited
Pages corrected
Pages already exact
Missing files
Empty files
New unresolved locations
Corrected-page list
Correction description per page
Commit SHA per corrected page
Cumulative progress
Next audit unit
```

Recommended result labels:

```text
PASS — NO CORRECTIONS
PASS WITH CORRECTIONS
BLOCKED — SOURCE PAGE UNAVAILABLE
```

---

## 14. Cumulative audit tracker

Maintain `TEXTUAL-FIDELITY-AUDIT.md` with:

```text
Total physical pages
Audited page range
Audited count
Progress percentage
Remaining pages
Corrected or expanded page records
Exact pages requiring no change
Explicitly unresolved locations
Iteration history
Next unit
Completion statement
```

Completion counts must reconcile:

```text
corrected pages + exact pages = audited pages
```

Any exception must be explained.

---

## 15. Git and commit discipline

### 15.1 Suggested commit messages

Initial extraction:

```text
Transcribe PDF pages 001-020
Add Chapter 1 contents and page records
Preserve front matter pages 001-012
```

Fidelity corrections:

```text
Audit PDF page 147 against scan
Restore printed Tamil text on PDF page 203
Preserve source punctuation on PDF page 285
```

Audit documents:

```text
Add textual-fidelity audit iteration 04
Update audit tracker through PDF page 120
Mark source textual-fidelity audit complete
```

### 15.2 Write safety

- Fetch the current file and blob SHA before updating.
- Do not run concurrent updates to the same file.
- Verify important reports and trackers after committing.
- Record commit SHAs in audit reports.
- Never rewrite audit history to make earlier errors disappear.

### 15.3 Branching

For small controlled projects, direct commits to the default branch may be acceptable.

For collaborative or public projects, use:

```text
transcription/pages-001-030
fidelity-audit/pages-031-060
```

and merge through reviewed pull requests.

---

## 16. Quality-control checklist

### Source and rights

- [ ] Original filename recorded
- [ ] Source URL and access date recorded
- [ ] PDF page count confirmed
- [ ] File hash recorded
- [ ] Rights or licence status documented

### Structural transcription

- [ ] One Markdown file exists for every physical page
- [ ] No duplicate physical page numbers
- [ ] Blank pages retained
- [ ] Cover, front matter and back matter retained
- [ ] Contents and chapter boundaries preserved
- [ ] Printed page labels recorded separately
- [ ] Manifest reconciles with the file tree

### Textual fidelity

- [ ] Every page visually compared with the scan
- [ ] Tamil characters checked
- [ ] English spelling and punctuation checked
- [ ] Transliteration checked
- [ ] Notes and footnote markers checked
- [ ] Tables and lists checked
- [ ] Page continuations checked
- [ ] Source errors preserved rather than silently corrected
- [ ] Unreadable locations documented without guessing

### Final closure

- [ ] Audit tracker shows 100%
- [ ] Corrected and exact counts reconcile
- [ ] Remaining page count is zero
- [ ] Structural audit is complete
- [ ] Textual-fidelity audit is complete
- [ ] README reflects final status
- [ ] Rights status is still accurately stated

---

## 17. Definition of done

A source volume is complete only when all of the following are true:

```text
Physical page records: complete
Structural audit: passed
Textual-fidelity audit: passed
Missing pages: 0
Remaining unaudited pages: 0
Unresolved readings: explicitly documented
Rights status: documented without unsupported assumptions
```

Suggested completion statement:

```markdown
## Final source status

- Physical PDF pages: **316**
- Page-level Markdown records: **316**
- Structural completion: **PASS**
- Textual-fidelity audit: **PASS**
- Missing page records: **0**
- Remaining unaudited pages: **0**
- Explicitly unresolved source locations: **2**
```

---

## 18. Archival layer versus derived layer

### Archival layer

Must remain source-faithful:

- page-level Markdown
- original spelling
- original punctuation
- original numbering
- original lineation where meaningful
- source mistakes
- page metadata

### Derived layer

May contain documented transformations:

- corrected text using the printed errata
- modernised Tamil spelling
- word-separated Tamil
- transliteration
- translation alignment
- summaries and explanations
- semantic tags
- searchable databases
- JSON, CSV and APIs

Never replace the archival layer with a derived version.

---

## 19. Standard prompt for future transcription projects

Use the following starting prompt for a new book:

```text
Start a page-by-page archival transcription of the attached PDF in this GitHub repository.

Requirements:

1. Inspect the complete PDF structure before transcribing.
2. Record source metadata, original filename, physical page count and file hash.
3. Check and document the source website's licence or rights status without assuming that download access permits redistribution.
4. Maintain one Markdown file for every physical PDF page, including covers, blank pages, images, contents, indexes, errata and advertisements.
5. Use zero-padded physical page filenames such as page-001.md.
6. Preserve printed wording, Tamil spelling, punctuation, transliteration, numbering anomalies and visible typographical errors exactly as printed.
7. Do not silently correct, modernise, translate or explain the source inside the archival transcription.
8. Mark genuinely unreadable locations explicitly and never guess.
9. Preserve the original contents, chapter hierarchy and page sequence. Maintain a manifest, page map and chapter register.
10. Commit the initial transcription in manageable page batches and keep a progress tracker.
11. After structural completion, perform a second visual textual-fidelity audit of every page against the scan.
12. Record every corrected page, correction category and commit SHA in iteration reports.
13. Update the cumulative tracker until all physical pages are audited and the remaining count is zero.
14. Keep derived data, normalised text, annotations and application outputs separate from the archival page records.

Do not declare the work complete until both structural completeness and the page-by-page textual-fidelity audit have passed.
```

For a multi-volume collection, add:

```text
Maintain a separate folder, metadata record, manifest, contents register, progress tracker and audit history for each volume. Do not mix page records across volumes.
```

---

## 20. Governing rule

Whenever convenience conflicts with fidelity, choose fidelity.

Whenever OCR conflicts with the scan, choose the scan.

Whenever a reading is uncertain, document uncertainty rather than guessing.

Whenever a derived improvement is useful, add it separately without altering the archival record.
