# Ethics — EXTRACTION_FRAMEWORK

**Project:** EXTRACTION_FRAMEWORK  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/dbpedia/extraction-framework  
**Pinned commit:** `b66cb8b976d69b17b0afa11fa701d5ae8463f42e`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d75114c2d4992cf9d9e74d709bc19a2ea515884649bb1a08f39bf5bc56557bf5`  
**Date:** October 2026

## Position

EXTRACTION_FRAMEWORK is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
