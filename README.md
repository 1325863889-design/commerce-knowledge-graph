# Commerce Knowledge Graph

> Repository: 1325863889-design/commerce-knowledge-graph  
> Status: portfolio-ready source package

## Overview

A commerce knowledge-graph project for entity extraction, annotation workflows, relational-data synchronization, and Neo4j graph modeling.

The repository is organized as a source-first engineering project. Local datasets, model weights, environment files, binary installers, generated outputs, and bulky media archives are intentionally excluded from version control. When those assets are required, keep them in external storage and document the download or provisioning process.

## Capabilities

- Commerce entity modeling for products, brands, categories, and attributes
- NER annotation and training workflow
- MySQL-to-Neo4j synchronization patterns
- Cypher query and graph-view assets

## Technology Stack

Python, Neo4j, MySQL, Label Studio, Transformers

## Repository Layout

- src/: application source, services, scripts, or runtime package code.
- docs/: architecture notes, diagrams, and implementation references.
- data/: lightweight sample data or schema files that are safe to version.
- infra/: Docker, database, or service-bootstrap configuration.
- prompts/: prompt templates and LLM workflow assets.
- ssets/: UI, image, diagram, or static resources.
- examples/: iteration snapshots, demos, or reference implementations.
- esources/: supporting files that do not fit the categories above.

## Local Setup

Prepare MySQL and Neo4j services, load sample data from `data`, then run entity extraction or graph synchronization scripts from `src`.

General setup checklist:

1. Create a Python or Node environment based on the dependency files in src or examples.
2. Copy .env.example to .env if an example file is provided, then fill in local service credentials.
3. Start required backing services such as MySQL, Neo4j, Milvus, MinIO, Elasticsearch, or model APIs.
4. Run the smallest backend script, API entrypoint, or test workflow before starting the complete application.

## Data and Model Artifacts

The following assets are intentionally not committed:

- API keys, database passwords, and local .env files.
- Virtual environments, dependency folders, caches, logs, and generated outputs.
- Model checkpoints, pretrained weights, TensorBoard runs, and large binary artifacts.
- Private business data, bulky datasets, media archives, and installer packages.

For production use, store large assets in Git LFS, object storage, Hugging Face, ModelScope, or an internal artifact registry.

## Maintenance Notes

- Add .env.example files for services that require configuration.
- Pin runtime dependencies once the deployment target is fixed.
- Add smoke tests for the primary service entrypoints.
- Keep sample data small and move bulky artifacts outside Git.