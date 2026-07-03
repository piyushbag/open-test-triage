# HW-Triage-Bench — Title and Abstract (SRG deck, v1, not submitted)

> **Source:** OCMS Pitch Deck — SRG (7 slides). Sanitized; no employer name.
> **Status:** Starter abstract only. Benchmark data must be synthetic or anonymized before arXiv.

---

## Title (recommended for this deck)

**HW-Triage-Bench: A Benchmark for Hardware Test Failure-to-Report Automation**

### Alternate titles

| Venue | Alternate |
|-------|-----------|
| DATE Track T2 (diagnosis) | *Automated Post-Test Documentation from Heterogeneous Validation Logs and Schematics* |
| DAC EDA2 / AI1.3 (agentic verification) | *Closing the Loop from Validation Failure Logs to Reviewer-Ready Diagnostic Reports* |
| OCP FTS | *Open Patterns for Agentic Hardware Validation Triage in Hyperscale Labs* |

---

## Abstract (~180 words)

Hardware validation engineers spend more time debugging and documenting failures than running tests. Industry surveys report debugging as the dominant verification activity, and recent academic work notes that automated analysis of engineering validation logs still lacks a standard, reproducible approach. Commercial EDA flows automate simulation and formal verification but typically stop before the post-test step: assembling failure evidence, locating affected components in schematics, and producing a reviewer-ready report remains manual across large program portfolios.

We introduce **HW-Triage-Bench**, an open benchmark and reference pipeline for the **failure-to-report** path. Given heterogeneous validation logs and schematic PDFs, systems must classify failure signatures, retrieve relevant design context, and emit structured diagnostic summaries suitable for design review. We evaluate rule-based, retrieval-augmented, and agentic baselines on **[N]** anonymized projects spanning **[M]** failure classes, reporting precision/recall on log classification and human-judged report usefulness.

We release benchmark tasks, evaluation harness code, and a non-proprietary **valtriage** module integrated with open lab stacks (OpenTAP, labgrid, OCP diag-core). HW-Triage-Bench establishes the first public baseline for a gap the field describes as open but rarely measures.

**Keywords:** hardware validation, test log analysis, post-silicon debug, agentic triage, benchmark, design review automation

---

## Metrics from deck (verify before publishing)

| Claim | Deck value | Public use |
|-------|------------|------------|
| Logs per project | 1,000+ | OK as aggregate |
| Active programs | 250+ | OK if approved |
| Manual time | ~1 hour / project | OK |
| Automated runtime | hours → minutes | Needs measured p50/p95 on open benchmark |
| Build date | Q1 2025 | OK in narrative |
| External adoption | None yet | State honestly; benchmark IS the external artifact |

---

## Open-source slice (non-proprietary)

Ship without internal DB schemas:

1. **Log classifier** — tiered fuzzy/regex on synthetic HW-Triage-Bench logs
2. **Schematic snippet locator** — PDF text/bbox heuristics on open reference schematics (KiCad exports)
3. **Report assembler** — Markdown/Jinja template (replaces internal doc output)
4. **Evaluation harness** — classification F1 + report rubric (design-review checklist)

Internal connectors (arjob, ahardware, Perforce) stay private; adapters documented as interfaces only.
