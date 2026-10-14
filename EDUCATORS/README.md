# Educators — TOBII_STREAM_ENGINE

**Project:** TOBII_STREAM_ENGINE  
**Category:** PSYCHOLOGY  
**Upstream:** see BENCH.json  
**Pinned commit:** `0eebec6df6f95521ab2209aa2eb424afcaff4885`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0569e2327480a5482c19dfbbaa2f9c02acd776321ed96f6bd855cb30e62b943c`  
**Date:** October 2026

## Teaching with TOBII_STREAM_ENGINE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `0569e2327480a5482c19dfbbaa2f9c02acd776321ed96f6bd855cb30e62b943c` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
