# GraphCoBots-KG

## Overview

GraphCoBots-KG is the core Knowledge Graph (KG) repository of the GraphCoBots research initiative.  
It contains the semantic models, ontology definitions, and structured graph data used to represent cultural heritage knowledge related to:

- the life and works of Nikos Kazantzakis, and  
- selected artefacts from the Nikos Kazantzakis Museum.

This repository provides the declarative knowledge layer that underpins the distributed and collaborative conversational AI architecture presented in the GraphCoBots research work. It is designed as a reusable, version-controlled research artifact that supports transparency, reproducibility, and long-term knowledge maintenance.

---

## Research Context

Knowledge Graphs play a central role in the GraphCoBots architecture by enabling:

- structured and semantically rich knowledge representation,
- interoperability across multiple chatbot services,
- continuous knowledge updates without retraining conversational models, and
- controlled access to sensitive or partially documented cultural heritage data.

Rather than embedding museum knowledge directly into chatbot logic, GraphCoBots-KG externalizes domain knowledge into a graph-based representation, allowing conversational agents to retrieve, reuse, and reason over shared knowledge resources.

---

## Repository Structure

.
├── schema/                 # Ontology and schema definitions  
├── data/                   # Knowledge Graph exports and Cypher scripts  
├── examples/               # Example Cypher queries and import scripts  
├── docs/                   # Modeling notes and documentation  
├── KazantzakisOnto_v5.owl  # Core ontology of the domain  
├── Full KG.txt             # Complete Cypher export of the Knowledge Graph  
├── LICENSE                 # Apache License 2.0  
├── LICENSE-DATA            # Creative Commons Attribution 4.0  
└── README.md               # Repository documentation  

---

## Usage

### Loading the Knowledge Graph into Neo4j

The Knowledge Graph can be reconstructed in a Neo4j database using the provided Cypher export.

1. Start a Neo4j instance (Desktop, Docker, or Cloud).
2. Ensure Cypher execution is enabled.
3. Load the graph using:

:source Full KG.txt

This command recreates the nodes, relationships, and properties defined in the Knowledge Graph.

Note: No Neo4j database files are stored in this repository. Only declarative artifacts are provided to ensure portability and reproducibility.

---

## Licensing

This repository follows a dual-license model, separating software artifacts from knowledge content:

- Code, scripts, and tooling are licensed under the Apache License 2.0.
- Knowledge Graph data and ontology files are licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0).

Please consult the respective license files before reuse or redistribution.

---

## Reuse and Reproducibility

GraphCoBots-KG is intended for:

- academic research on Knowledge Graph–based conversational AI,
- experimentation with cultural heritage knowledge modeling,
- integration into distributed or collaborative chatbot systems,
- reproducible evaluation of KG-driven information retrieval.

The repository avoids proprietary formats and binary database dumps, ensuring long-term accessibility and transparency.

---

## Relation to the GraphCoBots System

This repository provides the knowledge backbone for the GraphCoBots system, supporting:

- domain-specific chatbot services,
- collaborative multi-chatbot orchestration,
- hybrid Conversational AI and Generative AI integration.

While designed to be used alongside the GraphCoBots chatbot repositories, GraphCoBots-KG can also be reused independently in other Knowledge Graph–driven applications.

---

## Citation

If you use this repository or its contents in academic work, please cite the corresponding GraphCoBots publications that describe the architecture, implementation, and evaluation of the system.

---

## Contact

For questions regarding the Knowledge Graph design, ontology modeling, or reuse in research contexts, please contact the repository owner via GitHub.

---

## Acknowledgements

This repository supports ongoing research in Knowledge Graph–driven conversational AI for cultural heritage, contributing to scalable, interpretable, and curator-controlled museum information systems.
