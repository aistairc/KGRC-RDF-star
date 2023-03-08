# KGRC-RDF-star
The KGRC-RDF-star is an RDF-star dataset converted from [KGRC-RDF](https://github.com/KnowledgeGraphJapan/KGRC-RDF/tree/ikgrc2023).

 The same <i>s</i>, <i>p</i>, and <i>o</i> combinations may occur in different scenes when the KGRC-RDF is converted to the KGRC-RDF-star. It is necessary to distinguish these QTs and assign different metadata to them. Therefore, we solved this problem by assigning a unique ID to each QT and nested these triples as a QT as follows: &lt;&lt; &lt;&lt; s p o &gt;&gt; id val &gt;&gt; p' o'.
- [rdf-star_ext_ikgrc2023.nt](./rdf-star_ext_ikgrc2023.nt)
    - All data included.
- [rdf-star_ext_ikgrc2023_remove_Person_Place_Object.nt](./rdf-star_ext_ikgrc2023_remove_Person_Place_Object.nt)
    - Removed the values of rdf:type (Person, Object, and Place).
- [rdf-star_ext_ikgrc2023_remove_Situation_Statement_Thought.nt](./rdf-star_ext_ikgrc2023_remove_Situation_Statement_Thought.nt)
    - Removed the values of rdf:type (Situation, Statement, and Thought).