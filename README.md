# SPARQLing Archaeology: Knowledge Graphs, Wikidata, and QGIS in Practice
 
An Open Educational Resource (OER) introducing archaeologists to the practical use of archaeological Knowledge Graphs. Examples from NFDI4Objects Task Area 2, TRAIL 2.5 and 2.8.
 
**Live version:** <https://n4o-rse.github.io/oer-001-sparqling-archaeology/>
 
---
 
## About this module
 
This hands-on course introduces learners to querying, analysing, and visualising Linked Open Data with **SPARQL**, **Python**, and **QGIS**, using Wikidata and the NFDI4Objects Knowledge Graph as primary examples. It also covers fuzzy reasoning over RDF graphs with the **Academic Meta Tool (AMT)** and the integration of SPARQL into QGIS via the **SPARQLing Unicorn Plugin**.
 
All Jupyter notebooks are available in two variants: a browser-executable Quarto-Live version that runs in-page via Pyodide (no installation required) and a classical `.ipynb` version for local execution.
 
In this module, learners will:
 
- understand and articulate the core principles of Linked Data, RDF, and SPARQL;
- query public Knowledge Graphs (Wikidata, NFDI4Objects KG) with SPARQL and process the results programmatically in Python;
- load and analyse local Turtle (TTL) files with `rdflib`;
- visualise query results as diagrams and as interactive Leaflet maps;
- apply fuzzy reasoning over RDF graphs using the Academic Meta Tool and model simple attribution scenarios;
- integrate SPARQL queries into a GIS workflow via the SPARQLing Unicorn QGIS Plugin.
The module is organised into three sections: browser-executable notebooks for Knowledge Graphs (Ogham stones, Roman Samian ware, Campanian Ignimbrite sites), a notebook for the Academic Meta Tool, and a collection of QGIS example queries.
 
---
 
## Requirements
 
[Quarto ≥ 1.8](https://quarto.org) is required to render the module locally.
 
---
 
## Rendering locally
 
Clone the repository and render it with:
 
```bash
quarto render
```
 
The output is an HTML site in the automatically created `_site/` subdirectory. For live-reload during editing, use:
 
```bash
quarto preview
```
 
---
 
## Re-using this module as a template
 
If you want to build your own OER on the same structural basis, this repository can be used as a starting point. The repository is itself a derivative of the generic NFDI4Objects OER skript template (<https://github.com/nfdi4objects/oer-template-skript>), and the same template-use workflow applies:
 
```bash
quarto use template nfdi4objects/oer-template-skript
```
 
This creates a new project directory and copies all required files. You can then adapt:
 
1. author metadata in `_autor_innen.yml`;
2. module metadata (title, DOI, keywords, license) in `_oer_metadata.yml`;
3. content in `index.qmd` and — for this OER — the notebooks in `notebooks_lod/`, `notebooks_amt/`, and the QGIS query collection in `unicorn/`.
All template files are extensively commented in the source.
 
---
 
## Documentation
 
The [FAIR-OER template documentation](https://nfdi4objects.github.io/n4o_oer-template-dokumentation/) provides comprehensive guidance for educators, practitioners, and developers.
 
---
 
## Licence
 
This material is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
 
The templates in this repository are licensed under **[Creative Commons Attribution–ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/legalcode.en)**.
 
This choice is deliberate, as the templates are not software in the strict sense, but rather **structural, configuration, and text templates** for teaching and learning materials.
 
The licence not only enables the openness of the templates, but **permanently safeguards it**.
 
## Funding 
 
These materials were created within the DFG-funded project "[NFDI4Objects – Research Data Infrastructure for the Material Remains of Human History](https://gepris.dfg.de/gepris/projekt/501836407?language=en)" and were developed by Task Area 2 at [Leibniz-Zentrum für Archäologie](https://leiza.de).
<p align="center">
  <img src="https://www.dfg.de/resource/image/192702/16x9/858/483/8813c508271c12712973e1955ffdc082/86E5C6B4E28AAD65D48521A7A7498BF2/logo-gefoerdert-415.png" alt="Funded by the DFG" width="250">
</p>