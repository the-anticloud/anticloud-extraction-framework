# Educators — EXTRACTION_FRAMEWORK

**Project:** EXTRACTION_FRAMEWORK  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/dbpedia/extraction-framework  
**Pinned commit:** `b66cb8b976d69b17b0afa11fa701d5ae8463f42e`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d75114c2d4992cf9d9e74d709bc19a2ea515884649bb1a08f39bf5bc56557bf5`  
**Date:** October 2026

## Teaching with EXTRACTION_FRAMEWORK

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `d75114c2d4992cf9d9e74d709bc19a2ea515884649bb1a08f39bf5bc56557bf5` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
