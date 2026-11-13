Dimension 4: Terminological variant inclusivity quality
-------------------------------------------------------

Objective: To evaluate the ontology's ability to handle terminological diversity in the AI domain. The AI field has a large number of synonyms, expressions with different word orders, abbreviations, and other variants. The ontology has the capability to recognize and accommodate these variants. The dimension applies to the terminology of the security domain and of the trustworthiness domain alike; variants such as “resilience” and “robustness”, or “assurance” and “evidence”, are handled in the same way as the security variants.

Evaluation metrics
~~~~~~~~~~~~~~~~~~

1)  **Synonym Coverage Rate** — Whether the ontology associates sufficient synonym variants for each core concept.

> Assessment method: Construct an AI domain synonym test set and check ontology coverage.

2)  **Word-order Variant Recognition Ability** — Whether the ontology can recognize word-order variants (e.g., “general artificial intelligence” vs. “artificial general intelligence”).

> Assessment method: Construct a word-order variant test set and test the ontology’s recognition capability.

3)  **Abbreviation Mapping Coverage Rate** — Whether the ontology covers mappings between common AI abbreviations and their full forms (e.g., LLM ↔ Large Language Model).

> Assessment method: Construct an abbreviation test set and check coverage.

4)  **Cross-ontology Term Alignment** — Whether the ontology can recognize and map terminological differences between different standards organizations (ITU-T, ETSI, ISO/IEC).

> Assessment method: Term mapping analysis.

5)  **Cross-lingual Term Coverage Rate** — Whether the ontology supports multilingual terminological variants (at minimum Chinese and English).

> Assessment method: Expert review + automated checking.

6)  **Variant Update Mechanism Completeness** — Whether the ontology has mechanisms for the continuous discovery and incorporation of new terminological variants.

> Assessment method: Process review.

Evaluation methods
~~~~~~~~~~~~~~~~~~

1)  Test set verification method:

- Construct an AI domain terminological variant test set, including:
  - Synonym pairs: e.g., “neural network” and “artificial neural network”, “deep learning” and “deep neural network”;
  - Word-order variant pairs;
  - Abbreviation-full form pairs: e.g., “LLM” and “Large Language Model”, “CNN” and “Convolutional Neural Network”, “NLP” and “Natural Language Processing”;
  - Cross-standard term pairs: e.g., “AI threat” as defined by ETSI and the corresponding concept in relevant ITU-T standards.
- Test whether the ontology can correctly recognize these variants as referring to the same concept.

2)  LLM-assisted variant discovery and validation:

- Use an LLM to automatically discover potential terminological variants from AI literature and standards documents;

- Validate whether the ontology’s existing variant mappings are complete and accurate;

- Evaluate whether the ontology has the capability to continuously discover new variants using LLMs and other tools.

3)  Retrieval robustness testing:

- Construct queries using different variant expressions (e.g., expressing the same concept using synonyms, different word orders, abbreviations, etc.);

- Test whether the ontology-based knowledge graph or retrieval system returns consistent results.
