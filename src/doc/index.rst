.. raw:: latex

    \pagestyle{plain}
    \thispagestyle{plain}
    %% Suppress all TOC entries for the front matter (sections, subsections and
    %% any addcontentsline) — restored just before \sphinxtableofcontents so the
    %% numbered clauses appear in the TOC normally.
    \let\osiaorigaddcontentsline\addcontentsline
    \renewcommand{\addcontentsline}[3]{}

.. _front-matter:

Quality requirements and assessment framework for ontology on security and trustworthiness in AI systems
========================================================================================================

.. only:: html

    **Draft new Technical Specification TS.ontology-qat — Quality requirements and assessment framework for ontology on security and trustworthiness in AI systems**

.. raw:: latex

    \begin{center}\textbf{Draft new Technical Specification TS.ontology-qat — Quality requirements and assessment framework for ontology on security and trustworthiness in AI systems}\end{center}

Abstract
--------

This contribution proposes a new work item of Technical Specification on "Quality requirements and assessment framework for ontology on security and trustworthiness in AI systems".

Background
----------

Context of the study
~~~~~~~~~~~~~~~~~~~~

An ontology is a formal, explicit specification of a shared conceptualization — a structured knowledge model that defines the concepts, relationships, and logical constraints within a given domain. It provides a community with a shared vocabulary for organizing and exchanging knowledge, and enables machines to understand how entities in a domain are categorized and how they relate to one another. An AI security and trustworthiness ontology applies this methodology to the AI security domain, serving as a formal and shared description of concepts such as AI systems, threats, vulnerabilities, controls, mitigations, and incidents, as well as the causal relationships among them (e.g., a specific AI architecture exhibits a vulnerability that can be exploited by a particular type of attack).

The functions of an AI security and trustworthiness ontology are multi-fold. It enables semantic interoperability across different standards, tools, and organizations by providing a unified conceptual framework for mapping disparate terminologies. It supports large language models (LLMs) and AI agents with structured knowledge anchors that reduce hallucination and enable bounded reasoning. It serves as the schema layer for constructing AI security knowledge graphs, transforming unstructured standards text into machine-readable, queryable, and inferable knowledge assets. It also promotes harmonization across standards by revealing logical relationships — such as inheritance, dependency, and complementarity — between requirements defined in different documents.

Within ITU-T, SG17 has been actively advancing AI security standardization through a growing portfolio of work items, including X.sr-ai, X.sgGenAI, X.S-AIA, X.sr-da-gai, etc. The AI security and trustworthiness ontology serves as an important infrastructure for these efforts, providing a common semantic foundation that facilitates cross-standard consistency, knowledge reuse, and intelligent retrieval. In parallel, the rapid advancement of LLMs and agentic AI has created new demands for structured, machine-readable domain knowledge — a need that AI security and trustworthiness ontologies are uniquely positioned to address by providing deterministic entity definitions and verifiable relation constraints.

Given this context, the study of requirements and quality assessment for AI security and trustworthiness ontologies is of critical importance. Establishing clear, systematic requirements ensures that ontologies developed for AI security standardization are comprehensive, consistent, and fit for purpose. An operational quality assessment framework enables objective evaluation and continuous improvement, guiding the evolution of ontologies as the AI security landscape evolves. Together, these elements provide the methodological foundation needed for AI security and trustworthiness ontologies to serve as reliable, maintainable, and interoperable assets for the international standardization community.

Why this study is needed
~~~~~~~~~~~~~~~~~~~~~~~~

An AI security and trustworthiness ontology is needed to address the following critical gaps:

1)  **Semantic interoperability**: Different standards and tools use different terms for the same concept and the same term for different concepts, creating barriers to cross-system information exchange and collaboration.

2)  **Cross-standard harmonization**: ITU-T SG17 is developing multiple AI security standards simultaneously. Without a shared ontology, requirements and definitions in these standards may be inconsistent, contradictory, or redundant.

3)  **Machine-readable knowledge representation**: AI security knowledge is currently locked in unstructured natural language text within standards documents. An ontology enables the transformation of this knowledge into structured, machine-readable form that can be queried, reasoned over, and integrated with downstream applications.

4)  **LLM and AI agent integration**: Emerging AI applications such as LLM-based question answering and autonomous AI agents require structured knowledge anchors to reduce hallucination and support bounded reasoning. Ontologies provide the deterministic entity definitions and relation constraints needed for reliable AI reasoning.

5)  **Support for knowledge graph construction**: Ontologies serve as the schema layer for knowledge graphs, enabling systematic extraction, validation, and linking of AI security knowledge from standards documents into queryable knowledge bases.

6)  **Domain complexity**: The AI security domain is inherently interdisciplinary (spanning computer science, mathematics, cognitive science, law, and ethics) and rapidly evolving. An ontology provides a modular, extensible framework that can adapt to new threats, technologies, and regulatory requirements over time.

What this study is
~~~~~~~~~~~~~~~~~~

This study establishes a comprehensive framework for AI security and trustworthiness ontologies developed within the context of ITU-T SG17. It comprises two complementary parts:

Part 1 defines a systematic set of requirements that an AI security and trustworthiness ontology satisfies. These requirements are organized into nine categories: AI concept coverage (ensuring the ontology adequately describes AI systems themselves), AI security domain coverage (covering threats, vulnerabilities, risks, and controls), compatibility with existing AI ontologies (e.g., AIO, W3C ML-Schema), terminological variant inclusivity (handling synonyms, abbreviations, and word-order variants), structural and formal rigour (taxonomy depth, logical axioms, OWL 2 compliance), terminological standardization (naming conventions and multilingual support), extensibility and maintainability (modular design and version management), interoperability and reusability (mapping to external ontologies such as ETSI AI Threat Ontology and NIST AI RMF), and usability (documentation, competency questions, and serialization formats).

Part 2 defines an operational quality assessment framework comprising six evaluation dimensions: structural quality, AI concept coverage quality, semantic quality, terminological variant inclusivity quality, pragmatic quality, and standardization compliance. Each dimension has associated metrics, evaluation methods, and tools. A weighted scoring model produces a comprehensive quality score, and a four-level classification (Excellent, Good, Acceptable, Unacceptable) determines ontology readiness for standardization.

The study is complemented by two illustrative use cases (semantic interoperability across standards and knowledge graph generation from standards documents), a detailed six-phase ontology construction methodology, and a reference OWL 2 ontology implementation in Turtle format.

Key benefits
~~~~~~~~~~~~

This Recommendation provides the following key benefits to ITU-T SG17 and the broader international standardization community:

1)  **Unified terminology**: Establishes a controlled, standardized core vocabulary for AI security, eliminating ambiguous or conflicting definitions across standards and enabling all stakeholders to “speak the same language”.

2)  **Systematic requirements guidance**: Provides ontology developers with a clear, categorized set of requirements covering all critical dimensions of AI security and trustworthiness ontology quality, reducing the risk of incomplete or inconsistent ontology designs.

3)  **Measurable quality assurance**: Offers an operational evaluation framework with defined metrics, methods, and tools for objectively assessing whether an ontology meets the specified requirements, supporting continuous improvement.

4)  **Cross-standard harmonization**: Enables discovery of logical relationships (inheritance, dependency, complementarity, conflict) between requirements in different standards, supporting consistency review during standards development.

5)  Semantic interoperability: Provides a semantic bridge between different SDOs (ITU-T, ETSI, ISO/IEC, NIST), security tools (STIX, MITRE ATT&CK, MITRE ATLAS), and stakeholder groups, enabling automated cross-standard mapping and information exchange.

6)  **LLM and AI readiness**: Delivers structured, machine-readable knowledge foundations that can be integrated with LLMs for hallucination-reduced question answering and with AI agents for bounded reasoning and decision support.

7)  **Knowledge graph enablement**: Provides the schema layer for constructing AI security knowledge graphs from standards documents, transforming static text into dynamic, queryable, and inferable knowledge assets.

8)  **Future-proof extensibility**: The modular design and explicit variant-handling mechanisms ensure the ontology can evolve with the AI security domain, accommodating new threats, technologies, and standards without structural disruption.

Proposal for new work item
~~~~~~~~~~~~~~~~~~~~~~~~~~

This proposal requests the establishment of a new work item in ITU-T SG17 on the topic “Requirements and quality assessment framework for AI security and trustworthiness ontology”.

This work item studies the specification of requirements and the design of a quality assessment framework for AI security and trustworthiness ontologies within the context of ITU-T SG17 and related international standardization activities. It covers nine categories of requirements — AI concept coverage, AI security domain coverage, compatibility with existing AI ontologies, terminological variant inclusivity, structural and formal rigour, terminological standardization, extensibility and maintainability, interoperability and reusability, and usability — and a six-dimension evaluation framework with associated metrics, methods, and a weighted scoring model for determining ontology readiness for standardization. The work item also provides illustrative use cases, ontology construction methodology guidance, and a reference OWL 2 ontology implementation. It applies to ontologies that model both AI systems themselves (as objects of security protection) and AI security domain knowledge, without prescribing specific ontologies.

The A.1 justification for this proposal is provided in Annex A, and the initial text is provided in Annex B.

Summary
-------

The rapid advancement of AI technologies has introduced new and evolving security challenges that span multiple standards development organizations (ITU-T, ETSI, ISO/IEC, NIST, etc.), each employing its own terminologies and conceptual frameworks. This proliferation of disparate vocabularies — often referred to as the "terminological Tower of Babel" — creates significant barriers to semantic interoperability, knowledge sharing, and cross-standard harmonization. An AI security and trustworthiness ontology provides a formal, shared conceptualization of the AI security domain, serving as a common semantic foundation for standardizing terminology, enabling machine-readable knowledge representation, supporting large language model integration, and facilitating the construction of queryable knowledge graphs.

This draft new Technical Specification studies the quality requirements for an AI security and trustworthiness ontology — covering concepts, security domain knowledge, terminological variants, structural formality, and interoperability — and how to assess whether an ontology meets those quality requirements through a multi-dimensional quality evaluation framework with measurable metrics and a practical scoring model.

History
-------

.. list-table::
    :widths: 10 26 18 14 32

    * - Version
      - Document
      - Approval
      - Focus Group
      - Working Group

To access this Document as a PDF, open the published documentation site in your web
browser and click the PDF download link, or navigate directly to the PDF target of
this repository.

Authors
-------

.. list-table::
    :header-rows: 1
    :widths: 30 40 30

    * - Name
      - Affiliation
      - Contact
    * - Xiongwei Jia
      - China Unicom
      - jiaxw9@chinaunicom.cn

Keywords
--------

Artificial intelligence (AI) security, assessment, ontology, quality, semantic interoperability, trustworthiness

Foreword
--------

Agentic AI systems now act as autonomous entities capable of reasoning, planning, and
executing tasks across services, infrastructures, and organizational boundaries. This
fundamentally changes the nature of identity in digital systems: identity is no longer
limited to human users and static machine instances but must also encompass autonomous,
dynamic, and goal-oriented agents. And identity alone is insufficient — the core question
extends beyond "what an entity is" to "whether, and under what conditions, that entity
should be trusted to act".

The Focus Group on Trust and Identity for humans and agentic AI (FG-TIDA) addresses trust
management and interoperable digital identity infrastructure for humans and for agentic AI,
supporting the development of secure, trustworthy digital ecosystems in which humans and
agentic AI can safely interact and collaborate.

FG-TIDA was established under Recommendation ITU-T A.7 (Focus groups: Establishment and
working procedures), with ITU-T Study Group 17 as its parent group. Further details are
available in the group's terms of reference.

For more news and updates about the TIDA Community, including its supporter organizations,
please refer to the community's published resources.

Note
----

*[Editor: add any note on the status of this Technical Report.]*

.. raw:: latex

    %% Copyright notice commented out. To restore, uncomment the lines below.
    %% \vspace{4em}
    %% \begin{center}\textcopyright{} ITU 2026\end{center}
    %%
    %% \medskip
    %% All rights reserved. No part of this publication may be reproduced, by any means whatsoever, without the
    %% prior written permission of ITU.

    %% Restore \addcontentsline so the TOC below (and Chapter 1 onward) populate.
    \let\addcontentsline\osiaorigaddcontentsline
    \sphinxtableofcontents
    \osiamainmatter
    %% Clauses are \section under an unnumbered chapter, so LaTeX would print
    %% them 0.1, 0.2, ...  Number them from 1, and restart the counter here:
    %% the unnumbered front-matter subsections step it before this point.
    \makeatletter
    \renewcommand{\thesection}{\arabic{section}}
    \renewcommand{\thesubsection}{\thesection.\arabic{subsection}}
    \renewcommand{\thesubsubsection}{\thesubsection.\arabic{subsubsection}}
    \makeatother
    \setcounter{section}{0}

.. toctree::
    :maxdepth: 3
    :numbered:
    :hidden:

    chapters/01_scope
    chapters/02_references
    chapters/03_definitions
    chapters/04_abbreviations
    chapters/05_conventions
    chapters/06_overview
    chapters/07_quality-requirements
    chapters/08_quality-assessment-framework/index

.. toctree::
    :maxdepth: 3
    :hidden:

    chapters/09_appendix-i_use-cases
    chapters/10_appendix-ii_methodology
    chapters/11_appendix-iii_example-ontology/index
    chapters/12_bibliography
    chapters/13_annex-a_justification
    chapters/14_gap-analysis
