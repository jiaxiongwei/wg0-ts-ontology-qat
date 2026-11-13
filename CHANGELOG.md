# Changelog

All notable changes to the TS.ontology-qat source are recorded here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Dates are ISO 8601 (YYYY-MM-DD).

## [Unreleased]

### Added

- Full reStructuredText source for Technical Specification TS.ontology-qat,
  converted from the ITU-T-format Word contribution
  `FGTIDA-TS.ontology-qat.docx` (background, gap analysis, A.1 justification,
  and a draft text of 8 clauses, 3 appendices and a bibliography; no tracked
  changes or comments).

### Changed

- **Structure.** The contribution's three parts were redistributed: the
  **Background** (1.1–1.5) moved into `index.rst` as front matter with its
  numbers dropped, the **Gap analysis** became the final chapter, the
  **Suggestion** section (one sentence proposing the work item) was dropped, and
  the "Annex B: Proposed initial text" wrapper was dropped with its Summary and
  Keywords promoted into `index.rst`.
- **Clause numbering preserved.** The draft text already numbered its clauses
  1–8 with Conventions as clause 5, so no clause was renumbered and the in-text
  references (`clause 7`, `7.2`, `8`, `8.8`) stay valid as written.
- **Two chapters split** into `index.rst` plus one `_fragment.rst` per section:
  clause 8 (386 md-lines) into 9 fragments, Appendix III (345 md-lines) into 10.
  Appendix II stays a single file at 206 lines.
- **Front matter** carries the title, Abstract, Background, Summary, History,
  Authors, Keywords, Foreword and Note. The History table is left empty pending
  approval records.
- **Numbering.** `numfig = False`; captions keep their document-wide numbers
  (`Figure 1`, `Table 1–2`) because the prose cites them by number.
- **Abbreviations** rendered as a two-column table (25 entries) from the
  source's paragraph pairs.
- **Definitions** in 3.1 rendered as a definition list (9 terms), each keeping
  its source citation and note; 3.2 reads `None.` as in the source.
- **Bibliography** rendered as a definition list (24 entries). Entries that wrap
  onto a following line are grouped back into one entry.
- **Appendix III code** rendered as `.. code-block:: turtle` / `sparql`.
- **Annex A** taken from the author's updated form (WG0, Base text `XXX`, the
  stray `TBD` removed) and rendered as a `Field | Content` table after the
  Bibliography. Its "Reference and title" row still named *the sibling
  document's* subject — "Security requirements for trusted environment
  measurement and attestation of AI agents" — and was corrected to this
  specification's own title.
- **Template example content removed**: the demonstration chapters and the
  OpenAPI sample with its `html_extra_path` entry. Archived under
  `local/archive/`, which is not tracked.
- **PDF cover** reads "Technical Specification" rather than "Recommendation".

### Fixed

- **Figure 1 was missing.** pandoc drops the `w:drawing` that carries the
  diagram, so the converted text had the caption and no image. The picture is
  extracted directly from `word/media/image2.png` in the .docx and placed at the
  caption in 8.1.
- **Multi-line bibliography entries** produced "Unexpected indentation" errors;
  continuation lines are now folded into the entry they belong to.
- **Emphasis delimiters glued to URLs** (`*… Reference. *Https://…`) emitted
  "Inline emphasis start-string without end-string"; the closing delimiter now
  gets the space it needs.
- **`###` label lines** inside the Turtle samples are not lexable Turtle, which
  made Pygments retry in relaxed mode and warn; those blocks are no longer
  labelled as Turtle.
- **Word highlight spans** (`<span class="mark">`) stripped from body
  paragraphs, headings and the Editor's Note in clause 5.
- `exclude_patterns` extended to `**/_*.rst` so fragments are not built as
  standalone pages.
