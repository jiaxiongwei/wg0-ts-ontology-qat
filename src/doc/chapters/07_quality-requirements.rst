Quality requirements for AI security and trustworthiness ontologies
===================================================================

The requirements in this clause are quality requirements. They state what makes the ontology fit for use as a shared reference for AI security and trustworthiness standardization, and they are the requirements against which the quality assessment framework of clause 8 evaluates the ontology.

As an infrastructure item for ITU-T SG17 standardization, the requirements for an AI security and trustworthiness ontology can be grouped into the following eight categories. Compared to general ontologies or general security ontologies, the distinctiveness of an AI security and trustworthiness ontology lies in:

- The need to simultaneously model both the “AI system itself” (as the object of security protection) and “AI security knowledge” (as domain-specific security knowledge);

- The need to maintain compatibility and alignment with existing AI domain ontologies;

- The need to have the capability to handle rapidly evolving terminological variants in the AI field.

AI concept coverage
-------------------

This category of requirements addresses the distinctive scope of an AI security and trustworthiness ontology, which encompasses both security concepts and the AI systems they protect, including system components, task types, system categories, capability dimensions, lifecycle stages, and ethical aspects.

R-AC-01: The ontology is required to cover the core constituent elements of AI systems, including Data, Model, Algorithm, Training Strategy, Network Architecture, Layer, Preprocessing, and other key elements.

R-AC-02: The ontology is required to cover the main types of machine learning tasks, such as classification, regression, clustering, reinforcement learning, generation, etc.

R-AC-03: The ontology is required to cover different types of AI systems, including Discriminative AI, Generative AI, Large Language Models (LLMs), AI Agents, Multi-Agent Systems, and others.

R-AC-04: The ontology is required to cover AI capability dimensions, including Perception, Reasoning, Decision-Making, Planning, Autonomous Action, etc.

R-AC-05: The ontology is required to cover all stages of the AI lifecycle, from data collection and preparation, model training and validation, deployment and operation, maintenance and monitoring, and to retirement.

R-AC-06: The ontology is required to cover the ethical and governance dimensions of AI systems, including Bias, Fairness, Explainability, Transparency, etc.

AI security and trustworthiness domain coverage
-----------------------------------------------

The requirements in this clause are quality requirements: they state what makes the ontology fit for use as a shared reference for AI security and trustworthiness standardization, and they are the requirements against which the quality assessment framework of clause 8 evaluates the ontology. This category of requirements addresses the security-specific scope of an AI security and trustworthiness ontology, which complements AI concept coverage with comprehensive coverage of the AI security domain, including threats, vulnerabilities, risks, controls, roles, incidents, and others.

R-AS-01: The ontology is required to simultaneously cover both “Security for AI” (protection of AI systems themselves) and “Security by AI” (enhancing security capabilities using AI technologies).

R-AS-02: The ontology is required to cover the core types of threats to AI security, including but not limited to: Adversarial Attacks, Data Poisoning, Model Stealing, Inference-time Attacks, Prompt Injection, etc.

R-AS-03: The ontology is required to cover the conceptual systems of AI security Vulnerabilities, Risks, and Controls.

R-AS-04: The ontology is required to model the three roles of AI as System, Attacker, and Defender.

R-AS-05: The ontology is required to cover both endogenous risks (e.g., model bias, data quality) and derived risks (e.g., disinformation, public safety impact) faced by AI systems.

R-AS-06: The ontology is required to support modelling of AI security incidents, including the kill chain, scope of impact, and mitigation measures.

R-AT-01: The ontology is required to cover the trustworthiness characteristics of AI systems, including reliability, availability, resilience, safety, robustness, privacy, transparency, explainability, fairness and accountability.

R-AT-02: The ontology is required to relate each trustworthiness characteristic to the security concepts it depends on, so that a security control is traceable to the trustworthiness characteristic that it supports.

R-AT-03: The ontology is required to cover the life-cycle stages at which each trustworthiness characteristic is established and assessed, from data preparation and model development through deployment, operation and decommissioning.

R-AT-04: The ontology is required to represent the assurance evidence that demonstrates each trustworthiness characteristic, including evaluation results, certificates, audit records and incident reports.

R-AT-05: The ontology is required to model the stakeholders to which each trustworthiness characteristic is owed, and the accountability relation that holds when the characteristic is not met.

R-AT-06: The ontology is required to distinguish the trustworthiness characteristics that are properties of the AI system from those that are properties of the process that produced it.

Compatibility and alignment with existing AI ontologies
-------------------------------------------------------

This category of requirements addresses the alignment of the AI security and trustworthiness ontology with existing AI domain ontologies, ensuring conceptual compatibility and mappability while avoiding duplication of effort.

R-CA-01: The definitions of AI core concepts in the ontology are recommended to maintain conceptual-level mappability with mainstream existing AI ontologies.

R-CA-02: The ontology is recommended to explicitly declare which external AI ontologies it has established mappings to, and describe the mapping method (e.g., equivalence class, subclass, property mapping, etc.).

R-CA-03: When referencing external AI ontologies, the ontology is recommended to comply with the version management and namespace conventions of the referenced ontologies.

R-CA-04: When external AI ontologies are updated, the AI security and trustworthiness ontology is recommended to have a corresponding synchronization mechanism to maintain alignment.

Terminological variant inclusivity
----------------------------------

This category of requirements addresses the handling of terminological variants in the AI security domain, ensuring that the ontology recognizes and manages different expressions referring to the same concept, including synonyms, abbreviations, word-order variants, and cross-system terminology.

R-TV-01: The ontology is required to provide a canonical term for each core concept, while allowing one or more synonym variants to be associated.

R-TV-02: The ontology is required to support the recognition of word-order variants.

R-TV-03: The ontology is required to support mapping between abbreviations and full forms, e.g., “LLM” and “Large Language Model”, “ML” and “Machine Learning”.

R-TV-04: The ontology is recommended to support mapping between different terminological systems, e.g., the correspondence between ETSI terminology, ITU-T terminology, and ISO/IEC terminology.

R-TV-05: The ontology is recommended to support the handling of cross-lingual terminological variants, with support for English and Chinese term correspondence.

R-TV-06: The ontology is required to provide a mechanism for the discovery and update of terminological variants, enabling the continuous incorporation of new variants as the AI field evolves.

Structural and formal aspects
-----------------------------

This category of requirements addresses the structural and formal aspects of the ontology, covering class hierarchy, object and data properties, logical axioms and constraints, reasoning support, and alignment with ITU-T SG17 standards.

R-SF-01: The ontology is required to adopt a clear class hierarchy (taxonomy) following is-a inheritance relations, with a recommended maximum depth of 5 levels and an average of 2–12 subclasses per class.

R-SF-02: The ontology is recommended to define rich object properties and data properties to express diverse relationships between concepts.

R-SF-03: The ontology is required to support logical axioms and constraint definitions, including disjointness declarations, cardinality constraints, value constraints, etc.

R-SF-04: The ontology is recommended to have sufficient logical expressiveness to support reasoning and to adopt a subset of OWL 2 description logic.

R-SF-05: The top-level structure of the ontology is required to maintain conceptual alignment with the existing ITU-T security standard systems (e.g., the X-series security standards).

Terminological standardization
------------------------------

This category of requirements addresses the terminological standardization of the ontology, covering naming conventions, class definitions, alignment with published ITU-T standards, and multilingual label support.

R-TS-01: The naming of all classes, properties, and relations in the ontology is required to follow a unified naming convention (e.g., URI naming rules).

R-TS-02: Each class in the ontology is required to be accompanied by a clear definition in natural language describing its intension.

R-TS-03: Core terms in the ontology are required to be consistent with the term definitions in published ITU-T standards.

R-TS-04: The ontology is recommended to provide multilingual label support to accommodate the international nature of ITU-T.

Extensibility and maintainability
---------------------------------

This category of requirements addresses the extensibility and maintainability of the ontology, covering modular design, version management, adaptability to emerging threats, and governance mechanisms.

R-EM-01: The ontology is required to support modular design, allowing new concepts and relations to be extended without affecting the core structure.

R-EM-02: The ontology is required to have a version management mechanism supporting change tracking and version rollback.

R-EM-03: The ontology is required to be capable of adapting to the continuous emergence of new AI security threats, attack methods, and defence technologies.

R-EM-04: The ontology is required to provide clear maintenance procedures and governance mechanisms, specifying the responsible party for updates and the approval process.

Interoperability and reusability
--------------------------------

This category of requirements addresses the interoperability and reusability of the ontology, covering mappability with external ontologies, such as encoding in OWL 2, integration with downstream applications, and SPARQL [b-W3C-SPARQL] query support.

R-IR-01: The ontology is recommended to maintain mappability with external related ontologies, including the ETSI AI Threat Ontology [b-ETSI-AITONT], NIST AI RMF-related concepts [b-NIST-AIRMF], the [b-ISO/IEC 27090] security threat framework, etc.

R-IR-02: The ontology is recommended to be encoded using a standardized ontology language (OWL 2) to ensure machine readability.

R-IR-03: The ontology is recommended to support integration with downstream applications such as knowledge graphs and RAG systems.

R-IR-04: The ontology is recommended to support access and querying through standard SPARQL query interfaces.

Usability
---------

This category of requirements addresses the usability of the ontology, covering documentation, competency questions, serialization formats, and example instances.

R-UB-01: The ontology is required to be accompanied by clear documentation, including class hierarchy diagrams, property descriptions, usage guides, etc.

R-UB-02: The ontology is recommended to be accompanied by sample competency questions demonstrating the typical questions the ontology can answer.

R-UB-03: The ontology is recommended to provide multiple serialization formats (e.g., RDF/XML, Turtle [b-W3C-RDF1.1], JSON-LD [b-W3C-JSON-LD]) for use by different tools.

R-UB-04: The ontology is recommended to be accompanied by sample knowledge graphs or instance population examples to help users understand how to use the ontology.
