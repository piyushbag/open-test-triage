# Conference targeting matrix — SRG / HW-Triage-Bench

Research loops: official CFP pages fetched Jul 3, 2026. **Projected** deadlines follow the prior-year cycle when 2027 CFP is not yet posted.

| Conference | Submission type | Specific topic to target | Deadline |
|------------|-----------------|--------------------------|----------|
| **IEEE ITC 2026** | **Call for poster** (1-page; late-breaking / seeking feedback) | **Verification, Debug & Analysis → Diagnosis & Defect Analysis** (frame failure-log triage + schematic localization as post-test diagnosis automation) | **Jul 10, 2026** (confirmed) |
| **DATE 2027** | Research paper (Track **T**) | **T2: Test generation, test architectures, design for test, and diagnosis** — post-silicon debug + failure documentation gap | Abstract **Sep 13, 2026** AoE; paper **Sep 20, 2026** AoE (confirmed) |
| **IEEE ITC 2027** | Research paper (up to 10 pp.) | **Verification, Debug & Analysis → Data-Driven Test & End-to-End Analytics** (benchmark + pipeline for validation artifact analytics) | **~Mar 20, 2027** abstract; **~Apr 24, 2027** paper (projected from 2026 CFP) |
| **DAC 2027** | Research manuscript (6 pp. + refs) | **EDA2. Design Verification and Validation → EDA2.1** functional/transaction-level validation **or** **AI1.3 Agentic AI for verification** (failure-to-report as closed-loop validation) | **~Nov 11, 2026** abstract; **~Nov 18, 2026** paper (projected; 2027 CFP TBD) |
| **OCP Future Technologies Symposium 2027** | 2-page IEEE paper (presentation and/or poster) | **Future Tech from Complementary Communities** or **AI/HPC** — open validation-ops pattern aligned with OCP diag-core | **~Jun 2027** (projected; 2026 closed Jun 15, 2026) |
| **Architecture 2.0** (ISCA 2027 workshop) | Extended abstract / WIP (2–4 pp.; no formal proceedings) | **Infrastructure and Evaluation → Benchmarks for assessing agent-driven system workflows** (HW-Triage-Bench as agent-eval dataset) | **~May 2027** AoE (projected; ISCA 2026 was May 19, 2026) |
| **HotInfra** (ISCA 2027 workshop) | Regular or **industry paper** (3 pp.) | **Empirical evaluation of real infrastructures** — industry validation-ops case + InfraBench-style agent eval for lab triage | **~May 2027** (projected; 2026 was May 30, 2026) |
| **IEEE VTS 2027** | Research paper | **Validation, debug, and diagnosis** for system/board-level test (VTS scope: test, reliability, validation of microelectronic systems) | **~Nov 17, 2026** abstract; **~Nov 24, 2026** paper AoE (projected from VTS 2026) |
| **IEEE ETS 2027** | Regular / research paper | **T7 – Validation, Verification, and Debug** or **T8 – Test Generation, Fault Modeling & Simulation, Diagnosis** | **~Dec 2026** abstract; **~Jan 2027** full paper (projected; ETS 2026 was Dec 15 / Jan 14) |
| **IEEE IPDPS 2027** | Research paper (10 pp.; double-blind) | **Measurements, Modeling, and Experiments** — performance/latency study of failure-to-report pipeline (weaker fit; optional) | **~Oct 2, 2027** abstract; **~Oct 9, 2027** paper AoE (projected from annual cycle) |
| **OCP Test & Validation sub-project** | Community contribution (not archival) | **ocp-diag-core** schema + open triage adapter — T&V initiative meetings / GitHub review | **Rolling** (no fixed CFP) |

## Common theme (10-loop synthesis)

All ten targets sit on the same gap, expressed with different venue vocabulary:

1. **Post-execution validation gap** — EDA and lab tools generate failures; they do not produce stakeholder-ready diagnostic reports.
2. **Debug / diagnosis / analytics** — every test-track venue lists diagnosis, debug, or data-driven test analytics as in-scope.
3. **Heterogeneous artifacts** — logs, schematics, and metadata must be fused; no standard benchmark measures this fusion path.
4. **Automation at portfolio scale** — manual assembly does not scale with program count; reproducible pipelines and benchmarks are needed.
5. **Closing the loop** — emerging agentic/ML framing (DAC AI1.3, Architecture 2.0 benchmarks) matches failure-to-report orchestration without changing the core SRG problem.

## One-line problem statement (paper thesis)

**Hardware validation lacks an automated, reproducible path from heterogeneous test failure logs and schematic design artifacts to reviewer-ready diagnostic reports, leaving engineers to manually reconcile thousands of logs per program before design review can begin.**

## Venue-specific framing (same theme, different emphasis)

| Venue | One-line angle |
|-------|----------------|
| DATE / ITC / VTS / ETS | Diagnosis and post-silicon debug automation |
| DAC | Closed-loop design verification / agentic validation |
| OCP FTS / T&V | Open hyperscale validation operations on diag-core |
| Architecture 2.0 / HotInfra | Benchmark + agent evaluation for infrastructure triage |

## Nearest actionable deadline

**ITC 2026 poster — July 10, 2026** (7 days from Jul 3). Use 1-page poster to preview HW-Triage-Bench task definition; does not block DATE/ITC 2027 full paper.
