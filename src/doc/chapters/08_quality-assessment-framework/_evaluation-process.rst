Evaluation process
------------------

The evaluation process follows a six-step method, moving from preparation through automated assessment, LLM-enhanced assessment, expert review, comprehensive scoring, and final reporting. The process combines quantitative metrics, automated tools, LLM-assisted analysis, and expert judgment to produce a holistic quality assessment of an AI security and trustworthiness ontology against the requirements defined in clause 7.

**Step 1: Preparation Phase**

This phase involves gathering all necessary materials for the evaluation. The activities include collecting the ontology files in OWL or RDF format, gathering accompanying documentation such as class hierarchy diagrams and property descriptions, preparing a list of competency questions that the ontology is expected to answer, and constructing a terminological variant test set that includes synonyms, word-order variants, abbreviations, and cross-terminology mappings.

**Step 2: Automated Assessment**

This phase applies automated tools to evaluate the ontology across multiple dimensions. Structural assessment involves running OWL reasoners (such as Pellet, HermiT, or FaCT++) and structural analysis tools to verify syntactic correctness, logical consistency, and structural metrics. AI Concept Coverage assessment performs automated comparison with reference ontologies such as the Artificial Intelligence Ontology (AIO) to evaluate coverage of AI-related concepts. Semantic assessment employs LLM evaluation and embedding similarity analysis to assess concept accuracy, definition completeness, and label-definition alignment. Terminological Variant Inclusivity assessment runs the terminological variant test set to verify the ontology's ability to recognize and map variant expressions. Standardization assessment checks term alignment with ITU-T published standards and verifies compliance with naming conventions.

**Step 3: LLM-Enhanced Assessment**

This phase leverages large language models for deeper semantic evaluation. LLMs are used to evaluate the completeness of AI concept coverage by generating expected concept lists and comparing them against the ontology. They are also employed to discover potential missing terminological variants that are not covered by the initial test set. Additionally, LLMs assess the ontology's capability to describe AI security scenarios by evaluating its ability to represent realistic use cases and security situations.

**Step 4: Expert Review**

This phase engages domain experts for qualitative validation. ITU-T security experts review the accuracy of AI concept definitions and the correctness of relationships between concepts. AI domain experts assess whether the ontology's description of AI systems is adequate and comprehensive. Terminology experts evaluate the reasonableness of terminological variant handling, including synonym coverage, abbreviation mappings, and cross-terminology alignments. Pragmatic assessment involves reviewing the quality of answers produced for the competency questions, evaluating both correctness and completeness.

**Step 5: Comprehensive Scoring**

This phase consolidates all evaluation results into a unified quality score. Scores from each of the six assessment dimensions are aggregated according to the weighting scheme defined in clause 8.8. The comprehensive quality score is calculated on a 0-100 scale, and the ontology is assigned a quality level (Excellent, Good, Acceptable, or Unacceptable) based on the score thresholds. The scoring process also identifies which dimensions contributed positively or negatively to the overall result.

**Step 6: Assessment Report and Improvement Recommendations**

This phase produces the final evaluation output. A detailed assessment report is generated, documenting the results of each evaluation dimension, including specific metrics, expert findings, and LLM observations. Weak areas are identified with special attention to AI concept coverage and terminological variant handling. Specific, actionable improvement recommendations are provided for each identified weakness, prioritised by their impact on overall quality. The report serves as both a quality certificate and a roadmap for ontology refinement.
