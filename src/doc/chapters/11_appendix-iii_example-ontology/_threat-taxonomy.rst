Threat taxonomy
---------------

Based on the ETSI AI Threat Ontology classification approach, covering both "Security for AI" and "Security by AI" dimensions.

\### Classification by attack stage

:DataPoisoning

rdf:type owl:Class ;

rdfs:label "Data Poisoning"@en ;

rdfs:comment "An attack in which an adversary injects malicious data int..."@en ;

rdfs:subClassOf :Threat .

:AdversarialAttack

rdf:type owl:Class ;

rdfs:label "Adversarial Attack"@en ;

rdfs:comment "An attack in which an adversary crafts inputs to cause an..."@en ;

rdfs:subClassOf :Threat .

:ModelExtraction

rdf:type owl:Class ;

rdfs:label "Model Extraction"@en ;

rdfs:comment "An attack in which an adversary extracts the parameters or..."@en ;

rdfs:subClassOf :Threat .
