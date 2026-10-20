---
name: "dev-ontology-knowledge"
description: "Use for ontology design, knowledge graphs, RAG memory, entity modeling, taxonomy, or compounding project knowledge bases."
---
# Dev Ontology Knowledge

Design minimal, testable knowledge models that compound instead of being re-derived.

## Workflow

1. Collect competency questions: what must the graph answer?
2. Define entities, relations, and constraints justified only by those questions.
3. Keep taxonomy depth at most 3; push deeper detail into examples or annotations.
4. Ground entities with standard vocabularies where possible.
5. Convert ontology to implementation schema for RAG or GraphRAG extraction.
6. Ingest once: store raw evidence, wiki pages, entities, and relations separately.
7. Run quality checklist before finalizing: orphan entities, ambiguous relations, missing evidence links.

## Decision rules

- Stay minimal: add a class or property only with supporting evidence.
- Treat ontology like code: version it, review structural changes, re-run pipeline after updates.
- Prefer additive changes over renames or deletions on live graphs.
- Every relation must link back to source evidence.
- Separate methodology skill from domain requirements.

## Examples

- "Model medical domain": Party, Event, Finding entities tied to competency questions.
- "Build project wiki": ingest docs once, extract entities, cross-reference over time.
- "Add RAG memory": define schema, extract, store raw plus graph, retrieve with evidence.

## References reviewed

- Neo4j Going Meta ontology-builder assistant methodology.
- jbarrasa/goingmeta session46 modular skill structure.
- github/awesome-copilot mini-context-graph ingestion and retrieval pattern.
- cognee persistent agent-memory approach.





























