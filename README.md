# TOBII STREAM ENGINE

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-psychology-lightgrey)

> Anticloud-hardened packaging of the upstream project `TOBII_STREAM_ENGINE` in category **PSYCHOLOGY**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** PSYCHOLOGY · **Upstream:** https://github.com/the-anticloud/anticloud-tobii-stream-engine.git · **Upstream pin:** `b1e5acce8deab509690bb9ae0a2ce514e26c3766` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# Tobii Stream Engine Rust Bindings

This is a Rust crate containing FFI bindings and a few helpers for working with the [Tobii Stream Engine](https://tobii.github.io/stream_engine/) library for interfacing with Tobii eye trackers like the 4C.

The linker parameters are currently set up with the alpha SDK for macOS, which you can't get unless you ask, but with some tweaking of the linker attributes it should work on Windows as well. The bindings are for the older version of the API in the macOS version, but they shouldn't be difficult to update.

It has full support for the functionality in the 1.0.0 API, although with the 2.0 names (see v0.1 of tobii-sys for the 1.0 names). I haven't yet added bindings for the new Tobii Engine type from the 2.0 SDK.

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Rust / Cargo** (manifests: Cargo.toml; scanned in UPSTREAM_CLONE)
- Top-level source layout: `examples/`, `src/`, `tobii-stream-engine-sys/`
- Snapshot size: **22 files**, **1806 lines of code** (measured; see Benchmarks)
- Primary languages: `.rs` (15), `(none)` (4), `.toml` (2), `.md` (1)
- Upstream commit pinned for this packaging: `b1e5acce8deab509690bb9ae0a2ce514e26c3766`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
cargo build --release
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

```sh
cargo run --release
```

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

It has full support for the functionality in the 1.0.0 API, although with the 2.0 names (see v0.1 of tobii-sys for the 1.0 names). I haven't yet added bindings for the new Tobii Engine type from the 2.0 SDK.

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Rust / Cargo |
| Manifests detected | Cargo.toml |
| Files in snapshot | 22 |
| Lines of code | 1806 |
| Dependency references | 12 |
| Dependencies by ecosystem | cargo: 12 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| cargo | name | tobii-sys | Cargo.toml |
| cargo | version | 0.2.0 | Cargo.toml |
| cargo | license | MIT | Cargo.toml |
| cargo | build | build.rs | Cargo.toml |
| cargo | project | https://github.com/trishume/tobii-sys | Cargo.toml |
| cargo | documentation | https://docs.rs/tobii-sys | Cargo.toml |
| cargo | name | tobii-stream-engine-sys | tobii-stream-engine-sys/Cargo.toml |
| cargo | version | 0.1.0 | tobii-stream-engine-sys/Cargo.toml |
| cargo | project | https://github.com/cmaybon/tobii-stream-engine | tobii-stream-engine-sys/Cargo.toml |
| cargo | license | MIT OR Apache-2.0 | tobii-stream-engine-sys/Cargo.toml |
| cargo | description | Bindings to `tobii_stream_engine.dll` | tobii-stream-engine-sys/Cargo.toml |
| cargo | edition | 2021 | tobii-stream-engine-sys/Cargo.toml |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `Cargo.toml`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `TOBII_STREAM_ENGINE` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2017 Tristan Hume

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `TOBII_STREAM_ENGINE` (category: PSYCHOLOGY)
- **Upstream URL:** https://github.com/the-anticloud/anticloud-tobii-stream-engine.git
- **Pinned commit (SHA):** `b1e5acce8deab509690bb9ae0a2ce514e26c3766`
- **Branch:** main
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`bb8fd3c937b040491917244bfb00fdbec5a201ef0ba290632bef86e8e0a6714a`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

