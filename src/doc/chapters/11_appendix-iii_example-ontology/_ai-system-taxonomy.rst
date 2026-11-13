AI system taxonomy
------------------

Classification by AI type, task, and capability dimension.

\### Classification by technical approach

:DiscriminativeAI

rdf:type owl:Class ;

rdfs:label "Discriminative AI"@en ;

rdfs:comment "AI systems that learn the boundary between different class..."@en ;

rdfs:subClassOf :AI System .

:GenerativeAI

rdf:type owl:Class ;

rdfs:label "Generative AI"@en ;

rdfs:comment "AI systems that generate new content, such as text, images..."@en ;

rdfs:subClassOf :AI System .

:LargeLanguageModel

rdf:type owl:Class ;

rdfs:label "Large Language Model"@en ;

rdfs:comment "A type of generative AI model with billions of parameters..."@en ;

rdfs:subClassOf :GenerativeAI .
