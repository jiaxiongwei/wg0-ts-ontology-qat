# TS.ontology-qat

**Quality requirements and assessment framework for ontology on security and
trustworthiness in AI systems**

Proposed new Technical Specification of the Focus Group on Trust and Identity
for humans and agentic AI (FG-TIDA), Working Group 0 (WG0). Status: **draft (V1)**.

📄 **Web page:** https://jiaxiongwei.github.io/wg0-ts-ontology-qat/
📥 **PDF:** https://jiaxiongwei.github.io/wg0-ts-ontology-qat/specification.pdf

## What this document is

AI security standards describe the same concepts with different terms,
different granularities and different structures, so their content cannot be
combined, compared or queried across bodies. An ontology gives that content a
shared formal representation — but an ontology is only useful if it is itself
of adequate quality, and today there is no agreed way to judge that.

This Technical Specification specifies the quality requirements an AI security
and trustworthiness ontology has to meet, and an assessment framework for
measuring it. The requirements cover AI concept coverage, domain coverage,
compatibility with existing ontologies, terminological variant inclusivity,
structural and formal aspects, terminological standardization, extensibility,
interoperability and usability. The framework turns those requirements into six
quality dimensions with metrics and evaluation methods, a comprehensive scoring
model with quality-level classification, and an evaluation process. Appendix II
gives the construction methodology and Appendix III a worked ontology example
in OWL/Turtle with SPARQL competency questions.

## Contents

| | |
|---|---|
| 1–5 | Scope, References, Definitions, Abbreviations, Conventions |
| 6 | Overview of ontology and its role for AI security and trustworthiness |
| 7 | Quality requirements (7.1–7.9) |
| 8 | Quality assessment framework (8.1–8.9: six dimensions, scoring model, process) |
| Appendix I | Use cases |
| Appendix II | Methodology for constructing an AI security and trustworthiness ontology |
| Appendix III | Example ontology — OWL/Turtle, taxonomies, axioms, SPARQL |
| Bibliography, Annex A | References and the A.1 justification |
| Gap analysis | The gaps this work item addresses |

## Working on the document

The document is authored in reStructuredText and built with Sphinx into a web
page and a print PDF.

```shell
pip install -r requirements.txt
sphinx-build -b html src/doc target/html                            # web
sphinx-build -b latex src/doc target/latex && make -C target/latex  # PDF
```

`target/` is a **local build directory only** — it is git-ignored and never
published. The public site and PDF are built by GitHub Actions on every push to
`main` and deployed to the addresses above.

- `src/doc/index.rst` — title, abstract, background, summary, history, authors,
  keywords, foreword, note.
- `src/doc/chapters/` — one file per clause, `01`–`08`, then Appendix I–III, the
  bibliography, the Annex A justification and the gap analysis. Two of them are
  directories with an `index.rst` plus one `_fragment.rst` per section, pulled in
  with `.. include::`: `08_quality-assessment-framework/` (9 fragments) and
  `11_appendix-iii_example-ontology/` (10 fragments).
- `src/doc/images/` — figures.
- `src/doc/conf.py` — project metadata and the `cover_*` values used on the PDF cover.

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for how to propose a change, and
**[WG-ONBOARDING.md](WG-ONBOARDING.md)** for the TIDA authoring workflow.

## Editor

Xiongwei Jia, China Unicom — jiaxw9@chinaunicom.cn

## Licence

MIT, per [LICENSE](LICENSE). See [CHANGELOG.md](CHANGELOG.md) for document history.
