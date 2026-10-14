# Technical Architecture — EXTRACTION_FRAMEWORK

**Upstream:** [https://github.com/dbpedia/extraction-framework](https://github.com/dbpedia/extraction-framework)
**License:** Apache 2.0
**Category:** PHILOSOPHY_SEMANTICS
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

DBpedia semantic web data extraction

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local ontology reasoning and argumentation analysis
2. AIOSS provenance chain for all published arguments and revisions
3. AES-256 encryption for unpublished manuscript drafts
4. Single-binary semantic analysis tool with no cloud NLP dependency
5. Zero-cloud: all reasoning, search, and annotation runs locally
6. GPU/CPU equalizer: large language reasoning on GPU or CPU
7. Offline knowledge graph with local OWL/RDF store
8. Open OWL/RDF export replacing proprietary knowledge base formats

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_extraction_framework.spec` or `go build -o extraction_framework`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |