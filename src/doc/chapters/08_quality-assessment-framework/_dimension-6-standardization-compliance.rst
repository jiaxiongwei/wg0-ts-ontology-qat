Dimension 6: Standardization compliance
---------------------------------------

Objective: To evaluate the compliance and alignment of the ontology with the ITU-T security standards systems. The alignment covers the security standards and the trustworthiness provisions of the standards cited by the ontology alike.

Evaluation metrics
~~~~~~~~~~~~~~~~~~

1)  **Term Alignment** — Consistency of ontology terms with terms in published ITU-T standards.

> Assessment method: Term mapping analysis + expert review.

2)  **Naming Convention Compliance** — Whether ontology naming follows ITU-T naming conventions.

> Assessment method: Automated checking + expert review.

3)  **External Ontology Mapping** — Whether the ontology can establish mappings with external ontologies such as ETSI and NIST.

> Assessment method: Ontology alignment analysis.

4)  **Standard Reference Coverage** — Whether the ontology’s references to ITU-T standards are comprehensive and accurate.

> Assessment method: Literature analysis.

Evaluation methods
~~~~~~~~~~~~~~~~~~

1)  Term alignment analysis:

- Extract a core term list from published ITU-T standards (e.g., X.2211, X.sr-ai, etc.);

- Compare the ontology’s terms against the standard term list and calculate the alignment rate;

- Use an LLM to assist in term matching and discrepancy analysis.

2)  Ontology alignment analysis:

- Map the ontology’s classes against classes from external ontologies such as the ETSI AI Threat Ontology;

- Calculate the mapping coverage rate to evaluate interoperability.

3)  Standard compliance checking:

- Check whether the ontology follows ITU-T recommended practices (e.g., A.5 justification requirements).
