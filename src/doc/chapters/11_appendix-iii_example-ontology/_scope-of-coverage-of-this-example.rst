Scope of coverage of this example
---------------------------------

This example ontology demonstrates the key characteristics listed in Table 2:

.. list-table:: Table 2 – Scope of coverage of the example ontology
    :header-rows: 1
    :widths: 11 78 11

    * - Characteristic
      - Description
      - Corresponding Requirements
    * - AI Concept Coverage
      - Covers AI types including large language models, generative AI, discriminative AI, AI agents, multi-agent systems
      - R-AC-01, R-AC-02, R-AC-03
    * - AI Capability Dimensions
      - Covers perceptive AI, reasoning AI, agentic AI
      - R-AC-04
    * - Threat Coverage
      - Covers data poisoning, adversarial attacks, model extraction, prompt injection, jailbreak, and other AI-specific threats
      - R-AS-02
    * - Vulnerability Coverage
      - Covers data vulnerability, model vulnerability, infrastructure vulnerability
      - R-AS-03
    * - Control and Mitigation
      - Covers controls, mitigations, and their associations with threats
      - R-AS-03
    * - Trustworthiness Coverage
      - Covers reliability, availability, resilience, safety, robustness, privacy, transparency, explainability, fairness and accountability, and links each to the security concepts it depends on
      - R-AT-01, R-AT-02
    * - Standards and Requirements
      - Covers ITU-T standards and their associated security requirements
      - R-TS-03
    * - Logical Reasoning
      - Supports property chain reasoning (e.g., `exploits` + `hasVulnerability` → `hasTarget`)
      - R-SF-03, R-SF-04
    * - Cardinality Constraints
      - Each threat has at least one mitigation
      - R-SF-03
    * - Value Constraints
      - Severity level restricted to enumerated values
      - R-SF-03
    * - Multilingual Support
      - All classes, properties, and individuals have both English and Chinese labels
      - R-TS-04, R-TV-05
    * - Extensibility
      - Modular design enabling independent extension of threat, vulnerability, and other branches
      - R-EM-01
