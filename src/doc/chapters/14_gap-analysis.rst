Gap analysis
============

A review of existing standards and frameworks reveals that no current instrument provides a comprehensive requirements specification and quality assessment framework specifically for AI security and trustworthiness ontologies. The following existing instruments address related but distinct aspects.

ITU-T F.DCHE-Reqs — Requirements for construction of ontology knowledge base of home environment for robot interaction; focuses on the ontology knowledge base for home service robots. Relationship: This study is for ontology-based knowledge base (e.g., knowledge graph) for home service robots, not for AI security and trustworthiness ontology. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=21023

ITU-T F.DCOR-reqs — Requirements for construction of ontologies knowledge base for household service robots; provides the requirements for definition and automatically constructing a standardized knowledge base model for household service robots based on ontology technology. Relationship: similar to that for F.DCHE-Reqs. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=21015

ITU-T F.DCHU — Requirements for construction of home user profile ontology knowledge base for robot interaction in intelligent space; proposes the requirements for building an ontology knowledge base of home user. Relationship: similar to that for F.DCHE-Reqs. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=22132

ITU-T L.1401 (2026) — Guidelines for Data Annotation for GHG emissions Verification Knowledge Graph; provides guidelines for data annotation for GHG emissions verification knowledge graphs, and specifies requirements, principles, and methods for data collection, ontology modelling, data annotation and data quality management to support the construction, maintenance, and application of GHG emissions verification knowledge graphs. Relationship: This Recommendation mentions using ontology to verify knowledge graphs, but not for AI security and trustworthiness ontology. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=21904

ITU-T Y.4484 (2022) — Framework to support Web of Objects ontology based semantic data interoperability of eHealth services; specifies the framework to support Web of Objects (WoO) ontology based semantic data interoperability of eHealth services. Relationship: This Recommendation is not about AI security and trustworthiness ontologies, but about WoO ontology to be used for semantic data interoperability of eHealth services. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=17908

ITU-T Y.4500.12 (2018) — oneM2M base ontology; specifies the oneM2M base ontology, and an instantiation of the base ontology in oneM2M resources that is required for generic interworking. Relationship: This Recommendation is not about AI security and trustworthiness ontologies, but about oneM2M. Access: https://www.itu.int/ITU-T/workprog/wp_item.aspx?isn=14326

W3C OWL 2 (2012) — Web Ontology Language. Scope: Standard ontology language for the Semantic Web; defines syntax, semantics, and reasoning for ontology encoding. Relationship: This study adopts OWL 2 as the formal encoding language for AI security and trustworthiness ontologies (requirement R-SF-04), but OWL 2 provides no domain-specific requirements or quality metrics. Access: https://www.w3.org/TR/owl2-syntax/

**W3C RDF 1.1** (2014) — Resource Description Framework. Scope: Standard framework for representing information about resources on the web, forming the foundation for ontology data models. Relationship: Foundational technology for ontology representation and knowledge graph construction. Access: https://www.w3.org/TR/rdf11-concepts/

**W3C SKOS** (2009) — Simple Knowledge Organization System. Scope: Standard for representing thesauri, classification schemes, and term mapping systems. Relationship: Relevant to terminological variant handling (R-TV-01 to R-TV-06) and cross-ontology term alignment. Access: https://www.w3.org/TR/skos-reference/

**W3C SPARQL 1.1** (2013) — SPARQL Query Language for RDF. Scope: Standard query language for querying and manipulating RDF data. Relationship: Adopted as the standard query interface for ontology-based knowledge graphs (R-IR-04). Access: https://www.w3.org/TR/sparql11-query/

ETSI TS 104 050 V1.1.1 (2025) — Securing Artificial Intelligence (SAI); AI Threat Ontology and definitions. Scope: Defines an ontology for AI threats, including a classification of attack types against AI systems. Relationship: The closest existing standard; covers AI threat classification specifically. This study is complementary — it defines requirements and quality assessment for the entire AI security and trustworthiness ontology lifecycle, of which threat classification is one component. Access: https://www.etsi.org/deliver/etsi_ts/104000_104099/104050/01.01.01_60/ts_104050v010101p.pdf

**NIST AI RMF 1.0** (2023) — AI Risk Management Framework. Scope: Provides a framework for managing risks associated with AI systems, including risk identification, assessment, and mitigation. Relationship: Provides the risk governance conceptual framework; this study’s ontology maps AI security concepts to risk dimensions for traceable risk analysis (R-IR-01). Access: https://www.nist.gov/itl/ai-risk-management-framework

**NIST CSF 2.0** (2024) — Cybersecurity Framework. Scope: Framework for improving cybersecurity risk management across critical infrastructure sectors. Relationship: Provides cybersecurity governance concepts that can inform the ontology’s control and mitigation taxonomies. Access: https://www.nist.gov/cyberframework

**ISO/IEC 27090** (2024) — Cybersecurity — Artificial Intelligence — Security threats and controls. Scope: Specifies security threats and controls for AI systems. Relationship: Source domain knowledge for AI security concepts modelled in the ontology (R-AS-02, R-AS-03). Access: https://www.iso.org/standard/87157.html

**ISO/IEC 42001** (2023) — AI management systems. Scope: Specifies requirements for establishing, implementing, and improving AI management systems. Relationship: Provides AI governance context that the ontology’s management-layer concepts align with. Access: https://www.iso.org/standard/81230.html

**OASIS STIX 2.1** (2021) — Structured Threat Information Expression. Scope: Standard for representing cyber threat intelligence, including observables, indicators, and incidents. Relationship: Reference for structured threat information modelling; this study’s ontology can map AI security concepts to STIX patterns for incident representation (use case I.1). Access: https://docs.oasis-open.org/cti/stix/v2.1/stix-v2.1.html

MITRE ATT&CK — MITRE ATT&CK® Framework. Scope: Comprehensive knowledge base of adversary tactics, techniques, and procedures. Relationship: Reference for attack taxonomy modelling; its AI-specific counterpart, MITRE ATLAS [b-MITRE-ATLAS], provides the attack classification patterns used for AI security threat modelling. Access: https://attack.mitre.org/

AIO (Artificial Intelligence Ontology) (2023) — EMBL-EBI / NCI. Scope: Comprehensive ontology for the AI domain covering machine learning tasks, models, layers, training strategies, and bias concepts. Relationship: Primary reference ontology for AI concept mapping (R-CA-01); this study requires AI security and trustworthiness ontologies to maintain concept-level mappability with AIO. Access: https://bioportal.bioontology.org/ontologies/AIO

Summary of gap: No existing standard specifies the quality requirements an AI security and trustworthiness ontology meets or how to assess its quality across structural, semantic, and domain-specific dimensions. This study fills that gap by providing a systematic quality requirements taxonomy, an operational quality assessment framework with measurable metrics, and a quality classification model tailored to the AI security and trustworthiness domain.
