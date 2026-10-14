# Extension Guide — EXTRACTION_FRAMEWORK

**Upstream:** https://github.com/dbpedia/extraction-framework

## Adding New PAX Integration Points

1. Import `from anticloud.pax import pax_infer`
2. Call `pax_infer(prompt, max_tokens=512)` — returns locally-generated text
3. Log result with `aioss_append('PAX_INFERENCE', result_hash)`

## Adding AIOSS Hooks

1. Import `from anticloud.aioss import aioss_append`
2. Call before any write: `aioss_append(event_type, subject, content)`
3. Chain head is stored in `LEDGERS/aioss.jsonl`

## Single Binary Build

```bash
pyinstaller --onefile --name extraction_framework anticloud_main.py
```
