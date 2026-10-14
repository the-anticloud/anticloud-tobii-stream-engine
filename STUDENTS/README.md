# Students — TOBII_STREAM_ENGINE

**Project:** TOBII_STREAM_ENGINE  
**Category:** PSYCHOLOGY  
**Upstream:** see BENCH.json  
**Pinned commit:** `0eebec6df6f95521ab2209aa2eb424afcaff4885`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0569e2327480a5482c19dfbbaa2f9c02acd776321ed96f6bd855cb30e62b943c`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `0eebec6df6f95521ab2209aa2eb424afcaff4885`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `0569e2327480a5482c19dfbbaa2f9c02acd776321ed96f6bd855cb30e62b943c`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
