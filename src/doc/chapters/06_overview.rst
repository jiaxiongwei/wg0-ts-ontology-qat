Overview of ontology and its role for AI security and trustworthiness
=====================================================================

Overview of ontology
--------------------

An ontology is a formal, explicit specification of a shared conceptualization — a structured knowledge model that defines the concepts, relationships, and logical constraints within a given domain. It enables machines to understand how entities in a domain are categorized and how they relate to one another, and provides a community with a shared vocabulary for organizing and exchanging knowledge.

A typical ontology comprises the following core building blocks:

- Class: a concept, object type, or kind of thing, e.g., “AI System”, “Threat”, “Vulnerability”;

- Individual: a specific instance of a class, e.g., “GPT-4” is an individual of the class “Large Language Model”;

- Property: a characteristic or parameter of objects (and classes), e.g., “model parameter scale”, “training data source”;

- Relation: the manner in which classes relate to one another and to individuals, e.g., “is-a” (inheritance), “hasAttack” (has a certain attack), “mitigates” (mitigates a certain threat);

- Axiom and Constraint: logical rules and restrictions used to support automated reasoning.

Based on the above definitions and components, ontologies exhibit the following key technical characteristics:

1)  Formality: ontologies are encoded in rigorous logical languages (e.g., OWL 2 [b-W3C-OWL2]) with well-defined syntax and semantics, ensuring machine readability and processability.

2)  Shareability: an ontology represents a consensus within a community, enabling different systems, organizations, and individuals to communicate using a unified set of terms and concepts.

3)  Reasonability: through the definition of logical axioms and constraints, ontologies support automated logical inference by reasoners, enabling the discovery of implicit knowledge.

4)  Extensibility: ontologies support modular design, allowing new concepts and relations to be added without disrupting the core structure.

5)  Hierarchical structure: ontologies construct a hierarchy of concepts (taxonomy) through “is-a” inheritance relations, progressively refining from abstract to concrete.

AI security and trustworthiness ontology
----------------------------------------

An AI security and trustworthiness ontology is the specific product of applying ontological methodology to the domain of AI security. It constitutes a formal, shared description of all relevant concepts, attributes, relations, and logical constraints in the AI security field, with the aim of providing a unified semantic foundation for the standardization, knowledge management, and intelligent analysis of AI security.

Specifically, an AI security and trustworthiness ontology covers two core dimensions at the same time:

- The AI system itself (as the object of security protection): including the constituent elements of AI systems (data, models, algorithms, network architectures, etc.), AI task types (classification, generation, reinforcement learning, etc.), AI types (discriminative AI, generative AI, large language models, AI agents, etc.), and AI capability dimensions (perception, reasoning, decision-making, etc.);

- AI security knowledge (as the specialized knowledge of the security domain): including threats to AI systems (adversarial attacks, data poisoning, model stealing, prompt injection, etc.), vulnerabilities, risks, controls, mitigation strategies, and the two major directions of “Security for AI” (protecting AI systems) and “Security by AI” (enhancing security using AI).

The distinctiveness of an AI security and trustworthiness ontology, as compared to a general ontology or a general security ontology, is reflected in the following aspects:

1)  Dual modelling objects: a general ontology models only a single domain of concepts, and a general security ontology models only security concepts, whereas an AI security and trustworthiness ontology simultaneously models both the "AI system" and "AI security" domains, which are interwoven, and precisely describes the causal relationships between them (e.g., "a certain AI architecture :math:`\rightarrow` has a certain vulnerability :math:`\rightarrow` can be exploited by a certain type of attack").

2)  Rapidly evolving domain characteristics: AI technology itself is in a phase of rapid development, with new model architectures, training methods, and application scenarios continuously emerging, and correspondingly, new security threats and defence measures are also proliferating. An AI security and trustworthiness ontology possesses a stronger capacity for dynamic evolution than traditional domain ontologies.

3)  High terminological diversity: the AI field features a large number of synonyms, varied word-order expressions (e.g., “general artificial intelligence” versus “artificial general intelligence”), and the coexistence of abbreviations and full forms. An AI security and trustworthiness ontology has the capability to handle these terminological variants.

4)  Interdisciplinary integration: AI security involves multiple disciplines, including computer science, mathematics, cognitive science, law, and ethics. An AI security and trustworthiness ontology integrates the conceptual systems of these different disciplines within a single framework.

5)  Compatibility requirements with existing AI ontologies: the description of AI systems in an AI security and trustworthiness ontology maintains conceptual-level mappability with existing AI domain ontologies (such as the W3C ML-Schema [b-W3C-ML-Schema], etc.), thereby avoiding duplication of effort and conceptual conflicts.

Role of the AI security and trustworthiness ontology
----------------------------------------------------

As an infrastructure item for standardization, the AI security and trustworthiness ontology serves the following important functions.

Enabling semantic interoperability
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the field of AI security, different standards organizations, various security tools (STIX [b-OASIS-STIX], MITRE ATT&CK [b-MITRE-ATT&CK], MITRE ATLAS [b-MITRE-ATLAS], etc.), and diverse stakeholders (technical teams, compliance teams, management, etc.) each employ their own terminologies and conceptual frameworks. This inconsistency in terminology and semantic heterogeneity severely impedes the sharing of knowledge and cross-organizational collaboration.

Ontology alignment is a key means of achieving semantic interoperability. By providing a unified, standardized conceptual framework, an AI security and trustworthiness ontology enables:

- Terms from different standards documents to be cross-referenced and mapped to one another;

- Different security systems to exchange and understand structured security information;

- Different stakeholder groups (technical experts and management) to communicate about AI security risks using a common language.

In the cybersecurity domain, ontologies have demonstrated their ability to integrate knowledge from heterogeneous sources, foster shared understanding among diverse systems and stakeholders, and facilitate automated reasoning for collaborative defence and comprehensive knowledge management.

Supporting large language models (LLMs) and improving AI service quality
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The integration of AI security and trustworthiness ontologies with LLMs is emerging as an important trend in the AI security field. The supporting role of ontologies for LLMs is reflected in the following aspects:

1)  Providing structured knowledge anchors for LLMs and reducing “hallucination”:

Ontologies provide precise concept definitions and relation constraints for LLMs. Ontology-based retrieval-augmented generation (RAG) enriches LLM responses by retrieving structured knowledge triples from domain ontologies. Research has shown that knowledge graphs grounded in ontologies can provide LLMs with a reliable and verifiable method for reducing hallucination.

2)  Supporting reasoning and decision-making by AI agents:

With the rise of agentic AI, autonomous reasoning and decision-making in complex environments have become essential for AI agents. Ontologies supply these agents with well-defined entity types and explicit relational constraints, allowing them to formulate precise queries, navigate chains of relationships, and interpret the underlying causes of risky behaviour—rather than simply flagging anomalies. Practical experience shows that reasoning performance improves significantly when entities are unambiguously specified, relations are fixed, constraints are machine-accessible, and contextual information remains coherent across different domains.

3)  Enabling bounded reasoning:

Traditional LLM reasoning is probabilistic and prone to uncertain outputs. By incorporating ontologies into the reasoning process (e.g., querying deterministic facts from an ontology using SQL), AI reasoning can be transformed from probabilistic inference to bounded reasoning, thereby reducing the risk of hallucination, validating AI conclusions, and improving the accuracy and explainability of reasoning.

Promoting harmonization and consistency of AI security standards
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For ITU-T, the most direct value of an AI security and trustworthiness ontology lies in:

1)  Unifying standard terminology:

The ontology provides a controlled, standardized core glossary for the AI security domain, resolving terminological ambiguities that arise when the same concept is defined differently across standards (e.g., ITU-T X.2211, X.2212, etc.), and thus aligning all standards to a common terminological foundation.

2)  Discovering logical relationships between standards:

Through the hierarchical structure and relation definitions of the ontology, inheritance, dependency, complementarity, or conflict relationships between different standard requirements can be clearly displayed, helping experts identify and resolve issues during the standards development stage.

3)  Supporting intelligent application of standards:

Ontology-based knowledge graphs can support intelligent retrieval, automated question-answering, compliance checking, and other application scenarios, transforming static standards documents into dynamic knowledge bases that can be understood and processed by machines.

Enabling quantitative risk assessment and decision-making
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

An AI security and trustworthiness ontology provides a structured framework that connects abstract technical threats to concrete business impacts. By formalising the relationships between threat types, system vulnerabilities, and organizational assets, the ontology enables a systematic translation of technical risk factors into measurable business loss categories. This mapping supports quantitative risk scoring, facilitates cost-benefit analysis of mitigation measures, and allows decision-makers to prioritise investments based on objective financial exposure, rather than relying on subjective qualitative assessments.

Supporting the construction and continuous evolution of knowledge graphs
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

An ontology serves as the “schema layer” of a knowledge graph. It provides the knowledge graph with:

- A structural framework: Defining what types of entities and relations the knowledge graph includes;

- Semantic constraints: Ensuring that data in the knowledge graph conforms to predefined logical rules;

- An evolutionary foundation: When domain knowledge expands, updating the ontology guides the synchronous evolution of the knowledge graph.
