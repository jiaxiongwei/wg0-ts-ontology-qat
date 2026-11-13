Namespace and ontology declaration
----------------------------------

.. code-block:: turtle

    @prefix : <https://itu.int/ontologies/ai-security#> .
    @prefix owl: <http://www.w3.org/2002/07/owl#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
    @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix foaf: <http://xmlns.com/foaf/0.1/> .
    <https://itu.int/ontologies/ai-security>
      rdf:type owl:Ontology ;
      dcterms:title "AI Security Ontology"@en ;
      dcterms:description "An ontology for AI security standardization, developed for ITU-T SG17"@en ;
      dcterms:creator "ITU-T Study Group 17" ;
      dcterms:date "2026-07-19"^^xsd:date ;
      owl:versionInfo "1.0" ;
      owl:imports <http://www.w3.org/2002/07/owl> .
