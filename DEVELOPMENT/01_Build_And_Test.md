# Build and Test

**Project:** `EXTRACTION_FRAMEWORK`
**Upstream:** https://github.com/dbpedia/extraction-framework
**License:** Apache 2.0

## Quick Start

```bash
git clone https://github.com/dbpedia/extraction-framework
cd extraction-framework
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local ontology reasoning and argumentation analysis
2. AIOSS provenance chain for all published arguments and revisions
3. AES-256 encryption for unpublished manuscript drafts
4. Single-binary semantic analysis tool with no cloud NLP dependency
5. Zero-cloud: all reasoning, search, and annotation runs locally
6. GPU/CPU equalizer: large language reasoning on GPU or CPU
7. Offline knowledge graph with local OWL/RDF store
8. Open OWL/RDF export replacing proprietary knowledge base formats

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
