Appendix II Methodology for constructing an AI security and trustworthiness ontology
====================================================================================

(This appendix does not form an integral part of this Recommendation.)

This appendix provides a systematic, operational methodology for constructing an AI security and trustworthiness ontology. The methodology takes ITU-T’s published and under-development relevant standards as its primary knowledge source and draws on mature practices in ontology engineering, with the aim of guiding the entire process of requirements analysis, design, implementation, evaluation, and maintenance of the ontology.

Overview
--------

Positioning of the methodology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The construction of an AI security and trustworthiness ontology is a complex knowledge engineering task. The AI security domain is characterized by interdisciplinarity (involving computer science, mathematics, cognitive science, law, ethics, etc.), rapid evolution (new model architectures, threat types, and defence measures constantly emerging), and terminological diversity (the same concept has multiple expressions). Therefore, the construction methodology balances systematicity (following a standardized engineering process), flexibility (adapting to rapid changes in the domain), and authoritativeness (using international standards as knowledge sources).

This methodology takes relevant ITU-T SG17 standards documents as its primary knowledge source, references external achievements such as the ETSI AI Threat Ontology, and draws on mature approaches in ontology engineering (e.g., METHONTOLOGY, NeOn), forming a dedicated construction methodology suitable for the domain of AI security standards.

Core principles of the methodology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This methodology follows these core principles:

- **Standards-driven**: using published and under-development ITU-T AI security-related standards as the core knowledge source, ensuring consistency between the ontology and the security standards systems;

- **Requirements-oriented**: driving the design and evaluation of the ontology with clearly defined competency questions and application requirements;

- **Expert participation**: ITU-T domain experts participate throughout the entire process of ontology review and validation;

- **Iterative evolution**: ontology construction is an incremental process, with continuous optimization through multiple iterations;

- **Modular design**: the ontology adopts a modular architecture to support independent extension and maintenance;

- **Reusability**: maximizing the reuse of existing standard terminology and external ontology achievements.

Inputs and outputs of the methodology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- **Inputs**: published and under-development ITU-T AI security-related standards documents, such as X.sr-ai, X.sgGenAI, etc., as well as external reference ontologies such as the ETSI AI Threat Ontology.

- Outputs: an AI security and trustworthiness ontology that conforms to all requirements defined in Part 1 of this Recommendation and has passed quality assessment.

Construction process
--------------------

This methodology divides the construction of an AI security and trustworthiness ontology into six phases, each containing a number of specific activities. Iteration and feedback between phases are supported.

Phase 1: Requirements analysis and scope definition
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To clarify the construction objectives, application scenarios, coverage scope, and core competency questions of the ontology.

**Main activities**:

1.  Identify stakeholders and objectives: identify the primary users of the ontology (ITU-T experts, standards developers, AI security practitioners, etc.) and their core requirements.

2.  Define competency questions: list the typical questions the ontology is expected to answer. For example:

- “What known mitigation measures exist for prompt injection attacks against large language models?”
- “What security threats does a generative AI application service face during the data collection phase?”
- “Which security requirements apply to an AI agent system?”
- “What security dimensions (data, model, environment) need to be assessed when deploying AI technology in ICT?”

3.  Define scope and boundaries: clarify the coverage scope of the AI security domain, including both “Security for AI” (security of AI systems themselves) and “Security by AI” (enhancing security using AI), as well as all stages of the AI lifecycle.

4.  Identify reusable resources: survey existing ontologies and terminological resources that can be reused, including the ETSI AI Threat Ontology, term definitions in existing ITU-T standards, and external ontologies such as AIO (Artificial Intelligence Ontology).

**Outputs**: Requirements specification document, including a list of competency questions, scope definition document, and a list of reusable resources.

Phase 2: Knowledge acquisition and term extraction
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To systematically extract core terms, concepts, and relations from ITU-T standards documents and other knowledge sources.

**Main activities**:

1.  Knowledge source collection and preprocessing:
- Collect published and under-development ITU-T SG17 AI security-related standards documents;
- Collect external reference documents such as the ETSI AI Threat Ontology;
- Convert documents into processable text format, perform cleaning, sentence splitting, tokenization, and other preprocessing steps.
2.  Automated term extraction:
- Employ statistical methods such as TF-IDF and TextRank to automatically extract candidate terms from text;
- Employ topic models (e.g., LDA) to discover core topics and their associated terms in the document set;
- Use large language models (LLMs) with prompt engineering to extract candidate terms and concepts from standards documents.
3.  Term filtering and normalization:
- Invite ITU-T domain experts to filter and confirm the automatically extracted candidate terms;
- Cross-reference and unify confirmed terms with term definitions in existing ITU-T standards;
- Establish mapping relationships between canonical terms and their synonym variants.
4.  Relation identification:
- Based on co-occurrence patterns of terms in documents, identify potential associations between concepts;
- Use LLMs to infer semantic relations between terms (e.g., is-a, hasThreat, mitigates, etc.);
- Domain experts validate and supplement the automatically identified relations.

**Outputs**: Term list (including canonical terms and synonym variants) and draft relations between concepts.

Phase 3: Ontology design and formalization
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To design the ontology’s conceptual systems, property systems, and logical constraints based on the extracted terms and relations, and to encode them formally using a standard ontology language.

**Main activities**:

1.  Class hierarchy (taxonomy) design:
- Organize confirmed terms into classes and establish is-a inheritance systems;
- Use the classification framework of the ETSI AI Threat Ontology as a reference for top-level design;
- Ensure reasonable depth and breadth of the class hierarchy (recommended depth ≤ 5 levels, average 2–12 subclasses per class);
- Adopt modular design, dividing the ontology into independently reusable modules.
2.  Property and relation definition:
- Define object properties to express semantic relations between concepts;
- Define data properties to express numerical or textual attributes of concepts;
- Reference relation definition patterns from existing ontologies such as ITU-T X.641.
3.  Logical axiom and constraint definition:
- Define disjointness declarations, cardinality constraints, value constraints, and other logical axioms;
- Ensure the ontology has sufficient logical expressiveness to support reasoning.
4.  Alignment with external ontologies:
- Establish mapping relations between the ontology’s classes and external ontologies such as the ETSI AI Threat Ontology;
- Ensure that concepts related to AI systems in the ontology maintain mappability with AI domain ontologies such as AIO.
5.  Formal encoding:
- Use OWL 2 as the ontology encoding language;
- Provide multiple serialization formats (RDF/XML, Turtle, JSON-LD);
- Follow a unified naming convention (e.g., CamelCase, URI naming rules, etc.).

**Outputs**: OWL 2 ontology file and accompanying documentation.

Phase 4: Instance population
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To populate the ontology with individuals derived from specific provisions, security requirements, and threat instances in ITU-T standards documents.

**Main activities**:

1.  Instance identification and extraction:
- Identify specific entities from standards documents that can serve as instances of classes (e.g., specific attack types, specific AI system types, explicit security control measures, etc.);
- Use LLMs or rule engines to automatically extract instances and their properties from text.
2.  Instance validation and population:
- Domain experts validate the accuracy of automatically extracted instances;
- Populate validated instances into the ontology, establishing class membership relations and instance-to-instance relations.
3.  Instance-to-standard provision traceability:
- Record the source standard document and specific provision for each instance to ensure traceability.

**Outputs**: Complete ontology with populated individuals (including instance layer).

Phase 5: Quality assessment
~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To conduct a systematic quality assessment of the constructed ontology according to the evaluation framework defined in Part 2 of this Recommendation.

**Main activities**:

1.  Structural assessment:
- Use Pellet, HermiT, and other reasoners for syntax checking and logical consistency verification;
- Use OntoMetrics and other tools to calculate structural metrics (class hierarchy depth, average number of subclasses, property richness, etc.).
2.  AI concept coverage assessment:
- Assess the ontology’s AI concept coverage against reference ontologies such as AIO;
- Evaluate coverage of core AI concepts such as AI lifecycle, AI types, and AI capability dimensions.
3.  Semantic assessment:
- Use LLMs to review the accuracy, completeness, and clarity of each class definition;
- Use embedding models to calculate semantic similarity between class names and definitions;
- Domain experts review the reasonableness of relation definitions.
4.  Terminological variant inclusivity assessment:
- Use test sets of synonyms, word-order variants, and abbreviations to verify the ontology’s variant recognition capability;
- Evaluate cross-standard and cross-lingual term alignment.
5.  Pragmatic assessment:
- Verify whether the ontology can correctly answer the competency questions defined in Phase 1;
- Evaluate the ontology’s usability in typical scenarios through case studies.
6.  Standardization compliance assessment:
- Check the alignment rate between ontology terms and terms in published ITU-T standards;
- Check the mapping coverage between the ontology and external ontologies such as the ETSI AI Threat Ontology.

**Outputs**: Quality assessment report, including scores for each dimension, quality level, and improvement recommendations.

Phase 6: Maintenance and evolution
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Objective**: To establish a continuous maintenance mechanism for the ontology, ensuring that it evolves in step with the development of the AI security domain and the ITU-T standards framework.

**Main activities**:

1.  Version management:
- Establish a version management mechanism for the ontology, recording the content, reason, and date of each change;
- Support version rollback and change tracking.
2.  Regular update mechanism:
- Establish a mechanism for regular (e.g., semi-annual) mining of newly published standards documents using unsupervised learning techniques;
- When new ITU-T AI security standards are published or existing standards are updated, promptly incorporate new knowledge into the ontology.
3.  Continuous discovery of terminological variants:
- Use LLMs to continuously discover new terminological variants from newly published literature and standards;
- Regularly update the terminological variant mapping table.
4.  Community feedback mechanism:
- Establish an ITU-T expert community feedback channel to collect issues and improvement suggestions from ontology use;
- Regularly organize expert review meetings to discuss ontology update requirements.

**Outputs**: Updated ontology version and change log.

Knowledge sources
-----------------

Primary knowledge sources: ITU-T AI security-related standards
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The ontology is constructed using published and under-development ITU-T SG17 AI security-related standards as its primary knowledge source.

Supplementary knowledge sources
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In addition to ITU-T standards, the following external resources may serve as supplementary knowledge sources for the ontology:

- ETSI AI Threat Ontology: an AI threat ontology developed by the ETSI SAI ISG, serving as an important reference for AI threat classification;
- NIST AI RMF: the NIST AI Risk Management Framework, providing a conceptual framework for AI risk governance;
- AIO (Artificial Intelligence Ontology): a comprehensive AI domain ontology covering the core concepts of AI;
- W3C ML-Schema: a W3C machine learning schema providing standard descriptions of ML concepts;
- MITRE ATT&CK and MITRE ATLAS: knowledge bases of cyberattack tactics and techniques; ATLAS provides the AI-specific techniques referenced for AI security threat modelling.

Quality criteria
----------------

A completed AI security and trustworthiness ontology satisfies all requirements defined in Part 1 of this Recommendation and passes validation through the evaluation framework defined in Part 2. Minimum quality requirements include:

- Passing reasoner consistency checking (no logical contradictions);
- AI concept coverage rate of no less than 80% of the core concepts of reference ontologies (e.g., AIO);
- Core term alignment rate with published ITU-T standards of no less than 90%;
- Ability to correctly answer no less than 80% of predefined competency questions;
- Comprehensive quality score of no less than the Acceptable level (≥ 60 points).
