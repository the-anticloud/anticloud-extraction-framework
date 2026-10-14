# Command Line Interface — EXTRACTION_FRAMEWORK

**Upstream:** https://github.com/dbpedia/extraction-framework

## Anticloud CLI

```bash
# Install
pip install anticloud-extraction-framework

# Run offline with PAX inference
anticloud-extraction-framework --offline --pax-local

# Run with AIOSS logging
anticloud-extraction-framework --aioss-log ./ledger.jsonl

# Single binary (after build)
./extraction_framework --config config.yaml
```

## Options

| Flag | Description |
| --- | --- |
| `--offline` | Disable all network calls |
| `--pax-local` | Use local PAX inference at 127.0.0.1:11434 |
| `--aioss-log PATH` | Write AIOSS audit chain to PATH |
| `--encrypt` | Enable AES-256 at rest for output files |
| `--gpu` | Force GPU inference |
| `--cpu` | Force CPU inference |
| `--config PATH` | Load configuration from YAML file |
