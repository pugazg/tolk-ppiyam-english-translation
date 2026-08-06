# Tolkāppiyam — English Translation

A page-by-page archival transcription of **Dr. D. Albert's _Tolkāppiyam: Phonology & Morphology (An English Translation)_**, published by the International Institute of Tamil Studies in July 1985.

## Reusable workflow

The completed process from this repository has been documented as a reusable standard for future PDF-book projects:

- [`BOOK_TRANSCRIPTION_GUIDELINES.md`](BOOK_TRANSCRIPTION_GUIDELINES.md) — source intake, rights documentation, page-level Markdown structure, transcription rules, manifests, Git discipline, structural audits, visual fidelity audits and final completion criteria.

## Source

- Source PDF: `TVA_BOK_0013548_Tolkāppiyam.pdf`
- Physical/PDF pages: 316
- Languages: Tamil and English
- Scope: one Markdown file per physical PDF page, preserving front matter, contents, chapter order, Tamil source pages, English translation pages, notes, references, errata, closing matter and printed page numbering.

## Repository structure

```text
source-001-tolkappiyam-albert-1985/
├── README.md
├── manifest.md
├── FINAL-AUDIT.md
├── TEXTUAL-FIDELITY-AUDIT.md
├── textual-fidelity-audit/
├── contents-index-chapters/
├── front-matter/
├── part-01-phonology/
│   ├── chapters 1–9/
│   ├── research-topics/
│   └── index/
├── part-02-morphology/
│   ├── page-176.md
│   ├── chapters 1–9/
│   ├── research-topics/
│   ├── index/
│   └── reference-to-terms/
└── back-matter/
    ├── page-315.md
    └── page-316.md
```

Each page file records the physical PDF page, printed page label where present, language, section and transcription status. Doubtful readings are explicitly marked rather than silently corrected.

## Structural completion

All **316 physical PDF pages** have corresponding Markdown records.

- **Part I — Phonology is complete**, including its nine chapters, Research Topics and Index.
- **Part II — Morphology is complete**, including its nine chapters, Research Topics, Index and Reference to Terms.
- **Back matter is complete**, including Errata and the final institute-publications page.
- All **18 chapters** are represented.
- Missing physical page records: **0**.

## Textual-fidelity audit

The second-pass visual comparison of every Markdown page against the scan is complete.

- Audited: **PDF pages 1–316**
- Progress: **316 of 316 pages (100.00%)**
- Corrected or expanded across Iterations 1–14: **242 page records**
- Audited pages requiring no change: **74**
- Explicitly unresolved source locations: **2**
- Remaining for second-pass audit: **0 pages**

See the [`textual-fidelity audit tracker`](source-001-tolkappiyam-albert-1985/TEXTUAL-FIDELITY-AUDIT.md), the [`structural extraction audit`](source-001-tolkappiyam-albert-1985/FINAL-AUDIT.md), the [`manifest`](source-001-tolkappiyam-albert-1985/manifest.md) and the [`maintained navigation`](source-001-tolkappiyam-albert-1985/contents-index-chapters/).
