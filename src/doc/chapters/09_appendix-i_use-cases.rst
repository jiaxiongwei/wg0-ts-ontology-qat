Appendix I Use cases for AI security and trustworthiness ontology
=================================================================

(This appendix does not form an integral part of this Recommendation.)

To help readers gain a more intuitive understanding of the practical value of an AI security and trustworthiness ontology, this appendix presents two typical use cases. The first use case focuses on semantic interoperability, demonstrating how the ontology establishes a unified “translation layer” among different standards, systems, and organizations. The second use case focuses on knowledge graph generation, demonstrating how the ontology serves as a “schema layer” to guide the construction of structured AI security knowledge graphs from unstructured documents.

Enabling semantic interoperability of AI security information
-------------------------------------------------------------

The field of AI security involves multiple standards development organizations (ITU-T, ETSI, ISO/IEC, NIST, etc.), multiple information-sharing standards (STIX, MITRE ATT&CK, MITRE ATLAS, CAPEC, CVE, etc.), and numerous security tools and platforms. These systems and organizations each use their own terminologies and data models, resulting in a serious "semantic gap" when AI security information is transmitted across systems, organizations, and standards — the same concept has different names in different standards, and the same term refers to different concepts in different contexts.

Ontologies have been proven to “enable knowledge integration between heterogeneous knowledge bases, support shared understanding across different systems and stakeholders, and provide automated reasoning support for collaborative defence and integrated knowledge management”.

Use case scenario
~~~~~~~~~~~~~~~~~

When experts are developing new standards on security requirements for large language models (LLMs), during the drafting process they could reference:

- The classification of “Prompt Injection” threats as defined in the ETSI AI Threat Ontology;

- The tactic IDs and descriptions of relevant attack techniques in the MITRE ATLAS framework (the AI-specific extension of MITRE ATT&CK);

- Key concepts related to AI risk management in the NIST AI RMF;

- The format specifications for structured threat information expression in the STIX 2.1 standard.

However, the above sources may use different terminologies and classification systems for the same concept, making manual comparison both time-consuming and error-prone for experts.

Role and method of the ontology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In this scenario, the AI security and trustworthiness ontology serves as a Semantic Interoperability Layer, with the following specific steps:

Step 1: Establish a standard term mapping table. The AI security and trustworthiness ontology defines a canonical term for each core concept and establishes mapping relationships with external standard terms. Table 1 gives an example:

.. list-table:: Table 1 – Mapping of canonical ontology terms to corresponding terms in external frameworks
    :header-rows: 1
    :widths: 21 21 29 30

    * - Ontology Canonical Term
      - ETSI Corresponding Term
      - MITRE ATLAS Corresponding Entry
      - NIST AI RMF Corresponding Concept
    * - PromptInjection
      - prompt_injection
      - AML.T0051 (LLM Prompt Injection)
      - Adversarial threat
    * - DataPoisoning
      - data_poisoning
      - AML.T0020 (Poison Training Data)
      - Data integrity threat
    * - ModelExtraction
      - model_extraction
      - AML.T0024.002 (Extract AI Model)
      - Model leakage

NOTE – The corresponding entries in Table 1 are taken from ETSI TS 104 050 [b-ETSI-AITONT], MITRE ATLAS [b-MITRE-ATLAS] and the NIST AI Risk Management Framework [b-NIST-AIRMF]. MITRE ATLAS is the AI-focused knowledge base that complements MITRE ATT&CK® [b-MITRE-ATT&CK], which does not itself define AI-specific techniques for these threats.

**Step 2: Enable cross-standard querying and reasoning.** Based on the ontology’s unified conceptual framework, experts can use standard query languages such as SPARQL to retrieve relevant information from different standard sources in a single pass. For example, when querying “all security control requirements related to LLM prompt injection”, the system automatically maps the query to the corresponding terms from ETSI, MITRE, NIST, and other sources, returning integrated results.

**Step 3: Support automated impact analysis.** When a standard is updated, the ontology can automatically identify affected related standards and concepts. For example, when ETSI updates the classification definition of “prompt injection”, the ontology can automatically flag all provisions in ITU-T standards that reference this concept, alerting experts to conduct a consistency review.

**Step 4: Enable cross-organizational information sharing.** In AI security incident reporting or threat intelligence sharing scenarios, different organizations can describe the same event using their preferred terminological systems, while the ontology, as a shared semantic foundation, ensures that the receiving party can accurately understand the nature of the described security event, rather than merely matching keywords.

Outcomes
~~~~~~~~

- Improved standards development efficiency: experts no longer need to manually compare terminological differences across multiple sources;

- Cross-standard consistency assurance: ontology constraints ensure that definitions of the same concept remain consistent across different standards;

- Enhanced knowledge reuse: existing external standards achievements can be efficiently referenced and integrated into ITU-T standards;

- Foundation for automated tools: the ontology enables machines to automatically perform cross-standard semantic mapping and reasoning.

Generating knowledge graphs from AI security standards documents
----------------------------------------------------------------

The number of published and under-development AI security-related standards documents in ITU-T SG17 continues to grow. These documents exist in the form of natural language text and contain rich domain knowledge — threat definitions, security requirements, controls, best practices, etc. However, this knowledge is sealed within documents in unstructured text form, making it difficult for machines to directly process, retrieve, and reason with.

Research has shown that extracting actionable structured knowledge from unstructured text is a challenging task, because text “is typically unstructured, syntactically heterogeneous, and often ambiguous in meaning, complicating automated analysis”. Traditional manual knowledge extraction methods cannot keep pace with the speed of standards updates.

Use case scenario
~~~~~~~~~~~~~~~~~

Suppose an expert wishes to build an AI security knowledge graph that integrates knowledge scattered across various standards documents (e.g., “what mitigation measures exist for poisoning attacks against AI training data”, “what dimensions need to be checked in LLM security assessment”) into a structured, queryable, and inferable knowledge base to support intelligent retrieval, compliance checking, and decision support applications.

Role and method of the ontology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In this scenario, the AI security and trustworthiness ontology serves as the "schema layer" of the knowledge graph — it defines what types of entities (classes) are included in the knowledge graph, what types of relationships (properties) are allowed between entities, and what logical constraints (axioms) these entities and relationships follow. The specific steps are as follows:

Step 1: Define the schema of the knowledge graph. Based on the classes (e.g., “AI System”, “Threat”, “Vulnerability”, “Control”, “Mitigation”, etc.) and relations (e.g., “hasThreat”, “mitigates”, “exploits”, etc.) defined in the AI security and trustworthiness ontology, determine the node types and edge types of the knowledge graph. Each class in the ontology corresponds to a type of node in the knowledge graph, and each relation corresponds to a type of edge.

**Step 2: Extract entities and relations from standards documents.** Using natural language processing (NLP) techniques or large language models (LLMs), automatically identify and extract entities and entity-relations that conform to the ontology’s definitions from the text of ITU-T standards documents. For example, extract “Large Language Model” as an instance of the “AI System” class from the X.sgGenAI standard, extract “Prompt Injection” as an instance of the “Threat” class from the same document, and establish a “hasThreat” relation.

Step 3: Perform knowledge validation and disambiguation based on the ontology. The logical axioms and constraints defined in the ontology (e.g., "a 'Mitigation' corresponds to at least one 'Threat'", "'AI System' and 'Non-AI System' are disjoint", etc.) can serve as quality checking rules to automatically verify whether the extracted triples conform to the ontology's semantic constraints. Extracted results that do not satisfy the constraints are flagged for manual review, thereby ensuring the quality of the knowledge graph.

**Step 4: Construct a queryable knowledge graph.** Store the validated entities and relations in a graph database (e.g., Neo4j) or triple store, forming a knowledge graph accessible via standard query languages such as SPARQL. Researchers have demonstrated that integrating ontologies with knowledge graphs can “provide reliable and verifiable methods” and “improve context retention by 63%”.

**Step 5: Support intelligent applications.** Based on this knowledge graph, the following applications can be realized:

- Semantic search: retrieval based on concept semantics rather than keyword matching;

- Intelligent question-answering: using Retrieval-Augmented Generation (RAG) techniques to enable LLMs to answer specialized questions based on structured knowledge in the knowledge graph;

- Automated reasoning: discovering implicit knowledge through reasoners. For example, if the ontology defines that “Poisoning Attack” is a subclass of “Data Layer Attack” and “Data Layer Attack” affects “Training Data Integrity”, then the reasoner can automatically infer that “Poisoning Attack” affects “Training Data Integrity”;

- Continuous updating: when new draft standards are published, using automated extraction tools to incrementally populate new knowledge into the knowledge graph.

Outcomes
~~~~~~~~

- Standards knowledge is transformed from “static text” into a “dynamic knowledge base” that can be understood and processed by machines;

- Knowledge retrieval efficiency is greatly improved, from flipping through individual documents to precise semantic queries;

- Automated logical reasoning is supported, discovering implicit knowledge associations that are present in the text but not explicitly stated;

- Verifiable structured knowledge sources are provided for AI applications such as LLMs, reducing “hallucination”;

- Continuous evolution of the knowledge graph is achieved, keeping pace with updates to the security standards systems.

The two use cases above illustrate two different levels of value provided by an AI security and trustworthiness ontology:

- Use case 1 (Interoperability) demonstrates the value of the ontology as a “horizontal integration layer” — building semantic bridges between different standards, systems, and organizations to solve the “Tower of Babel” problem;

- Use case 2 (Knowledge Graph Generation) demonstrates the value of the ontology as a “vertical modelling layer” — establishing a structured knowledge representation framework within a single knowledge domain, transforming unstructured text into computable knowledge.

The two are mutually reinforcing: the knowledge graph generated in Use Case 2 can be cross-domain linked and fused with external knowledge graphs based on the interoperability framework established in Use Case 1; and the interoperability capability of Use Case 1 depends on the structured knowledge constructed in Use Case 2 as exchangeable content. Together, they constitute the complete value chain of an AI security and trustworthiness ontology in supporting standardization work.
