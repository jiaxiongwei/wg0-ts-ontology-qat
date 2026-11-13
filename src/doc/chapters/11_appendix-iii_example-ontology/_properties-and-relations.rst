Properties and relations
------------------------

::

    ### Object Properties
    :hasThreat
      rdf:type owl:ObjectProperty ;
      rdfs:label "has threat"@en ;
      rdfs:comment "Links an entity to a threat that affects it."@en ;
      rdfs:domain :AI System ;
      rdfs:range :Threat .
    :exploits
      rdf:type owl:ObjectProperty ;
      rdfs:label "exploits"@en ;
      rdfs:comment "Links a threat to a vulnerability it exploits."@en ;
      rdfs:domain :Threat ;
      rdfs:range :Vulnerability .
    :mitigates
      rdf:type owl:ObjectProperty ;
      rdfs:label "mitigates"@en ;
      rdfs:comment "Links a mitigation or control to a threat it mitigates."@en ;
      rdfs:domain :Mitigation ;
      rdfs:range :Threat .
    :addresses
      rdf:type owl:ObjectProperty ;
      rdfs:label "addresses"@en ;
      rdfs:comment "Links a requirement to a threat or vulnerability it addres..."@en ;
      rdfs:domain :Requirement ;
      rdfs:range :Threat .
