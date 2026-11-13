Competency questions and SPARQL query examples
----------------------------------------------

Based on the example ontology defined in this appendix, the following demonstrates how to answer typical competency questions using SPARQL queries.

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT DISTINCT ?threat ?threatLabel WHERE {

\# ?threat rdf:type :Threat ;

\# :hasTarget ?target .

\# ?target rdf:type :LargeLanguageModel .

\# ?threat rdfs:label ?threatLabel .

\# }

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?mitigation ?mitigationLabel WHERE {

\# :PromptInjectionAttack :hasMitigation ?mitigation .

\# ?mitigation rdfs:label ?mitigationLabel .

\# }

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?requirement ?requirementLabel WHERE {

\# :XSgGenAI :hasRequirement ?requirement .

\# ?requirement rdfs:label ?requirementLabel .

\# }

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?threat ?threatLabel WHERE {

\# ?threat rdf:type :Threat ;

\# :hasSeverity "Critical" ;

\# rdfs:label ?threatLabel .

\# }

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?attack ?attackLabel WHERE {

\# ?attack :exploits :LLMPromptVulnerability .

\# ?attack rdfs:label ?attackLabel .

\# }

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT DISTINCT ?threat ?threatLabel WHERE {

\# ?threat rdf:type :Threat ;

\# :hasTarget ?target .

\# ?target rdf:type :LargeLanguageModel .

\# ?threat rdfs:label ?threatLabel .

\# }

\### CQ2: Query all mitigations for the "Prompt Injection" threat

\### SPARQL query:

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?mitigation ?mitigationLabel WHERE {

\# :PromptInjectionAttack :hasMitigation ?mitigation .

\# ?mitigation rdfs:label ?mitigationLabel .

\# }

\### CQ3: List all security requirements specified in the X.sgGenAI standard

\### SPARQL query:

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?requirement ?requirementLabel WHERE {

\# :XSgGenAI :hasRequirement ?requirement .

\# ?requirement rdfs:label ?requirementLabel .

\# }

\### CQ4: Query all threats with severity level "Critical"

\### SPARQL query:

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?threat ?threatLabel WHERE {

\# ?threat rdf:type :Threat ;

\# :hasSeverity "Critical" ;

\# rdfs:label ?threatLabel .

\# }

\### CQ5: Query all attacks that exploit the LLM prompt vulnerability

\### SPARQL query (utilizing property chain reasoning):

\# PREFIX : \<https://itu.int/ontologies/ai-security#\>

\# SELECT ?attack ?attackLabel WHERE {

\# ?attack :exploits :LLMPromptVulnerability .

\# ?attack rdfs:label ?attackLabel .

\# }
