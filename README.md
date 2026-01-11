# GraphCoBots-KG

**GraphCoBots-KG** contains the core **Knowledge Graph (KG) artifacts** that support the GraphCoBots family of conversational AI chatbots for museums and cultural heritage organizations. The repository provides the semantic structures, schema definitions, and structured data exports used consistently across the GraphCoBots ecosystem.

This repository is part of the broader **GraphCoBots** research initiative, which investigates distributed, collaborative, and Knowledge Graph–driven multi-chatbot architectures for cultural heritage applications.

---

## Research Context

This repository serves as a research artifact addressing:

* Knowledge Graph modeling for cultural heritage domains
* Semantic representation of museum knowledge
* Interoperable and reusable graph datasets for conversational AI
* Reproducibility and transparency in KG-based systems

The Knowledge Graph artifacts are designed to be **declarative, portable, and version-controlled**, enabling both experimental evaluation and practical deployment.

---

## Repository Structure

```
.
├── schema/                 # Schema definitions, constraints, and indexes
├── data/                   # Knowledge Graph exports (Cypher, CSV, JSON-LD)
├── examples/               # Example queries and usage scripts
├── docs/                   # KG documentation and modeling notes
├── .gitignore              # Git ignore configuration
├── LICENSE                 # Apache License 2.0 (code and tooling)
├── LICENSE-DATA            # CC BY 4.0 (Knowledge Graph content)
└── README.md               # Project documentation
```

---

## Knowledge Graph Artifacts

### Schema Definitions

The `schema/` directory contains:

* Node label definitions
* Relationship type specifications
* Property constraints and index configurations

These ensure semantic consistency and data integrity across all GraphCoBots Knowledge Graph instances.

---

### Data Exports

The `data/` directory provides structured Knowledge Graph exports in portable formats, such as:

* `.cypher` scripts for Neo4j import
* `.csv` files compatible with graph import pipelines
* Optional Linked Data serializations (e.g., JSON-LD)

Binary database files are intentionally excluded to support reproducibility.

---

### Examples

The `examples/` directory includes:

* Sample Cypher queries
* Import and initialization scripts
* Demonstrative graph traversal examples

These files are intended to facilitate reuse by researchers and developers.

---

## Usage

### Importing into Neo4j

1. Start a Neo4j instance (Desktop, Docker, or Aura)
2. Ensure APOC procedures are enabled
3. Load schema definitions:

```cypher
:source schema/constraints.cypher
```

4. Load Knowledge Graph data:

```cypher
:source data/graph.cypher
```

These steps reconstruct the Knowledge Graph in a clean Neo4j database instance.

---

## Licensing

This repository follows a **dual-license model**:

* **Code and tooling**: Apache License 2.0 (see `LICENSE`)
* **Knowledge Graph content and data**: Creative Commons Attribution 4.0 International (CC BY 4.0) (see `LICENSE-DATA`)

Users are responsible for complying with the applicable license depending on the material reused.

---

## Citation

If you use this Knowledge Graph or its components in academic research, please cite the relevant **GraphCoBots** publications. A `CITATION.cff` file may be added to facilitate automated citation workflows.

---

## Notes for Researchers and Developers

* Knowledge Graph artifacts are provided in declarative formats
* Database binaries are intentionally excluded
* Schema and data should be versioned separately
* Follow semantic naming conventions to preserve interoperability

---

## Contact

For research inquiries, collaboration opportunities, or technical questions, please contact the repository owner via GitHub.

---

## Acknowledgements

This repository supports ongoing research on Knowledge Graph–driven conversational AI for cultural heritage, contributing to transparent, reusable, and semantically rich museum information systems.
