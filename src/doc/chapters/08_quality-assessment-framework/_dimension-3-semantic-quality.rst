Dimension 3: Semantic quality
-----------------------------

Objective: To evaluate how accurately and consistently the ontology represents the meaning of the concepts and the relations of the AI security and trustworthiness domain.

Evaluation metrics
~~~~~~~~~~~~~~~~~~

1)  Concept Definition Accuracy — Whether each class definition states the intension of its concept correctly and agrees with the source standards, for the security concepts and the trustworthiness concepts alike.

> Assessment method: Definition-by-definition comparison with the source standards, plus expert review.

2)  Relation Correctness — Whether the properties and the relations between classes express the intended meaning, including their domain, range and direction.

> Assessment method: Axiom review against the domain model, plus reasoner checks.

3)  Taxonomic Consistency — Whether the class hierarchy contains no cycles, unsatisfiable classes or unintended equivalences, in the security branch and the trustworthiness branch alike.

> Assessment method: Reasoner classification and disjointness checking.

4)  Cross-domain Linking — Whether each trustworthiness characteristic is linked to the security concepts it depends on, and each security control to the trustworthiness characteristic it supports.

> Assessment method: Traceability check over the trustworthiness-to-security relations.

5)  Ambiguity and Redundancy — Whether each concept carries a single intended meaning and no concept is duplicated under a different identifier across the two domains.

> Assessment method: Lexical and structural redundancy analysis, plus reference-vocabulary alignment.

Evaluation methods
~~~~~~~~~~~~~~~~~~

1)  Definition and relation review:

- Each class definition and each relation is compared with its source standard;

- Domain experts review the accuracy of the security concepts and of the trustworthiness concepts in the same pass;

- The relations that link a trustworthiness characteristic to the security concepts it depends on are verified explicitly.

2)  Consistency and redundancy analysis:

- Reasoner classification and disjointness checking detect unsatisfiable classes and unintended equivalences;

- A lexical analysis flags synonyms modelled as separate classes and classes that are candidates for merging, in either domain.

3)  Cross-domain traceability analysis:

- The trustworthiness-to-security relations are traversed to confirm that each trustworthiness characteristic is traceable to the security concepts it depends on;

- The converse relations are traversed to confirm that each security control is traceable to the trustworthiness characteristic it supports.
