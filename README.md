# KGRC-RDF-star
The KGRC-RDF-star is an RDF-star dataset converted from [KGRC-RDF](https://github.com/KnowledgeGraphJapan/KGRC-RDF/tree/ikgrc2023).

 The same <i>s</i>, <i>p</i>, and <i>o</i> combinations may occur in different scenes when the KGRC-RDF is converted to the KGRC-RDF-star. It is necessary to distinguish these QTs and assign different metadata to them. Therefore, we solved this problem by assigning a unique ID to each QT and nested these triples as a QT as follows: &lt;&lt; &lt;&lt; s p o &gt;&gt; id val &gt;&gt; p' o'.
- [rdf-star_ext_ikgrc2023.nt](./rdf-star_ext_ikgrc2023.nt)
    - All data included.
- [rdf-star_ext_ikgrc2023_remove_Person_Place_Object.nt](./rdf-star_ext_ikgrc2023_remove_Person_Place_Object.nt)
    - Removed the values of rdf:type (Person, Object, and Place).
- [rdf-star_ext_ikgrc2023_remove_Situation_Statement_Thought.nt](./rdf-star_ext_ikgrc2023_remove_Situation_Statement_Thought.nt)
    - Removed the values of rdf:type (Situation, Statement, and Thought).

## Statistics

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-dvpl{border-color:inherit;text-align:right;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-c3ow" colspan="2">Class</th>
    <th class="tg-dvpl">17</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-c3ow" colspan="2">Instance</td>
    <td class="tg-dvpl">9,524</td>
  </tr>
  <tr>
    <td class="tg-c3ow" colspan="2">Property</td>
    <td class="tg-dvpl">640</td>
  </tr>
  <tr>
    <td class="tg-c3ow" rowspan="6"><br><br><br><br><br><br>Triple</td>
    <td class="tg-c3ow">Standard triple</td>
    <td class="tg-dvpl">14,180</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Single-nested QT</td>
    <td class="tg-dvpl">9,765</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Double-nested QT</td>
    <td class="tg-dvpl">6,409</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Triple-nested QT</td>
    <td class="tg-dvpl">695</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Quadruple-nested QT</td>
    <td class="tg-dvpl">43</td>
  </tr>
  <tr>
    <td class="tg-c3ow">Total</td>
    <td class="tg-dvpl">31,092</td>
  </tr>
</tbody>
</table>

## Embeddings
If you want to use this dataset for graph embeddings, please see [RDF-star2Vec](https://github.com/aistairc/RDF-star2Vec).
The gold standard datasets and evaluation framework are [here](https://github.com/aistairc/GEval-forKGRC-RDF-star).


## LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">KGRC-RDF-star</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/aistairc/KGRC-RDF-star" property="cc:attributionName" rel="cc:attributionURL">Shusaku Egami</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/KnowledgeGraphJapan/KGRC-RDF" rel="dct:source">https://github.com/KnowledgeGraphJapan/KGRC-RDF</a>.
