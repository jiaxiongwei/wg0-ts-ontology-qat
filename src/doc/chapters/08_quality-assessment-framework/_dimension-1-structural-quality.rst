Dimension 1: Structural quality
-------------------------------

**Objective**: To evaluate the syntactic correctness, structural reasonableness, and logical consistency of the ontology.

Evaluation metrics
~~~~~~~~~~~~~~~~~~

1)  **Syntactic Correctness** — Whether the ontology conforms to specific syntax specifications (such as OWL 2).

> Assessment method: Syntax checking using Pellet, HermiT, and other reasoners.

2)  **Class Hierarchy Depth** — Maximum depth of the inheritance tree (recommended :math:`\leq` 5 levels).

> Assessment method: Automated calculation.

3)  **Average Number of Subclasses** — Number of direct subclasses per class (recommended 2-12).

> Assessment method: Automated calculation.

4)  **Logical Consistency** — Whether the ontology contains logical contradictions (e.g., disjoint class conflicts).

> Assessment method: Reasoner consistency checking.

5)  **Modularity** — Whether the ontology is divided into independently reusable modules.

> Assessment method: Expert review + graph theory analysis (modularity calculation).

6)  **Property Richness** — Average number of properties per class.

> Assessment method: Automated calculation.

Evaluation methods
~~~~~~~~~~~~~~~~~~

The structural quality evaluation employs a combination of automated tools and expert review to assess the syntactic correctness, structural reasonableness, and logical consistency of the ontology.

**a) Syntax and consistency checking**

The ontology's syntactic conformance to OWL 2 specifications and its logical consistency are verified using standard OWL reasoners. These reasoners perform the following checks:

- Syntax validation against the OWL 2 specification;

- Consistency checking to detect logical contradictions (e.g., disjoint class conflicts, unsatisfiable classes);

- Classification to verify the coherence of the class hierarchy.

**b) Structure metrics calculation**

Structural metrics, including class hierarchy depth, average number of subclasses, and property richness, are automatically calculated using ontology analysis tools. The calculation process comprises:

- Parsing the ontology file (OWL/RDF format) to extract class and property structures;

- Computing the inheritance tree and identifying root classes, leaf classes, and intermediate nodes;

- Deriving the maximum depth, average subclass count, and average property count per class.

**c) Modularity analysis**

Modularity is evaluated through a combined approach of graph theory analysis and expert review:

- Graph theory analysis: The ontology's class and property structures are represented as a directed graph, and modularity scores are calculated to identify clusters of highly interconnected concepts. Tools or custom scripts using network analysis libraries are used for this purpose.

- Expert review: ITU-T domain experts assess whether the identified modules are logically cohesive, independently meaningful, and reusable in specific subdomains of AI security (e.g., threat modelling, control implementation, incident response).

**d) Validation of recommended ranges**

The recommended ranges for hierarchy depth (:math:`\leq` 5 levels) and average subclass count (2–12 per class) are assessed against established ontology engineering best practices. If the calculated values deviate from these ranges, the ontology is flagged for expert review to determine whether the deviation is justified by the domain complexity or indicates a structural flaw.

The results from automated tools and expert reviews are consolidated to produce a comprehensive structural quality score for the ontology. Any identified issues (e.g., inconsistencies, excessive depth, low property richness) are recorded as part of the assessment report with actionable improvement recommendations.
