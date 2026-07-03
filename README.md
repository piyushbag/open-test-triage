# OpenTestTriage / HW-Triage-Bench

Open research artifact for **hardware test failure-to-report automation**: classify validation logs, localize schematic context, and emit reviewer-ready diagnostic reports.

**Author:** Piyush Jagadish Bag · Test Automation Engineer, Platform Hardware · [piyushbag.com](https://piyushbag.com)

**EB-1A hub:** [eb1a-profile](https://github.com/piyushbag/eb1a-profile)

## Problem

Validation engineers manually assemble design review reports: sort **1,000+ logs per project**, query engineering databases, locate components in schematic PDFs, and format output by hand (**~1 hour per project** at portfolio scale). EDA tools automate simulation and verification but rarely close the loop to **structured post-test documentation**.

## This repo

| Path | Purpose |
|------|---------|
| [`paper/`](paper/) | LaTeX source, abstracts, conference targets |
| [`benchmarks/hw-triage-bench/`](benchmarks/hw-triage-bench/) | Public evaluation benchmark (in progress) |
| [`oss/opentesttriage/`](oss/opentesttriage/) | Non-proprietary reference pipeline |
| [`evidence/`](evidence/) | Public trail: publications, outreach, external interest |

## Paper

**Title:** HW-Triage-Bench: A Benchmark for Hardware Test Failure-to-Report Automation

- **Overleaf:** see [`paper/overleaf.md`](paper/overleaf.md)
- **LaTeX source:** [`paper/latex/`](paper/latex/)

## Status

| Milestone | Status |
|-----------|--------|
| Benchmark spec | Draft |
| Open reference pipeline | Scaffold |
| arXiv preprint | Not submitted |
| Peer conference | Target DATE / ITC 2027 |

## License

Apache-2.0 (code) · Paper text CC BY 4.0
