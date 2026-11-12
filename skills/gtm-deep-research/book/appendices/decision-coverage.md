# Decision coverage index — DR-001 through DR-052

[Book home](../index.md) · [Reconciliations and supersession](audit-reconciliations.md)

**Approved behavioral specification:** 52 design decisions, five parts, fourteen chapters. This appendix maps the decisions to their *primary* governing chapter. The complete package documents all Chapters 01–14, including completion, reopening, dependencies, recovery and static-audit procedures. The existence of documented procedures is **not** proof of successful live execution.

## Part I — Research Foundations (13)

| Decision | Primary rule | Chapter |
|---|---|---|
| DR-001 | Adaptive hybrid research and human learning | 01 |
| DR-002 | Rigorous iterative goal-grilling | 01 |
| DR-003 | Bounded researcher discretion | 02 |
| DR-005 | Adaptive human collaboration | 02 |
| DR-006 | Depth-first investigation | 02 |
| DR-007 | Bounded preliminary reconnaissance | 01 |
| DR-008 | Mandatory discovery dimensions | 01 |
| DR-009 | Core discovery with approved subject extensions | 01 |
| DR-010 | Versioned auditable research charter | 01 |
| DR-011 | Full-run agreement and autonomous internal planning | 02 |
| DR-017 | Invalidated assumptions and selective pausing | 02 |
| DR-046 | Intent-based activation | 01 |
| DR-047 | Risk- and complexity-based research depth | 01 |

## Part II — Investigation Methodology (17)

| Decision | Primary rule | Chapter |
|---|---|---|
| DR-004 | Evidence-calibrated observations and interpretations | 04 |
| DR-012 | Autonomous evidence-exhausted noncritical gap closure | 03 |
| DR-013 | Impact-based criticality assessment | 03 |
| DR-014 | Substantively independent red-team on major conclusions | 05 |
| DR-015 | Major conclusion classification by consequence | 05 |
| DR-016 | Bounded disagreement adjudication | 05 |
| DR-018 | Structured subphase research contracts | 03 |
| DR-019 | Three-layer provenance, claims, semantic concepts | 04 |
| DR-020 | Qualitative confidence with rationale | 04 |
| DR-021 | Continuous provisional OKF evidence integration | 04 |
| DR-022 | Distinct evidence and review states | 04 |
| DR-023 | Structured chronological investigation journal | 03 |
| DR-028 | Adaptive assigned research effort budgets | 06 |
| DR-029 | Measured-versus-estimated multidimensional budgets | 06 |
| DR-030 | Explicit preauthorized extensions and hard ceilings | 06 |
| DR-031 | Claim-specific source triangulation | 04 |
| DR-032 | Bounded legitimate source recovery | 04 |

## Part III — OKF Knowledge Architecture (11)

| Decision | Primary rule | Chapter |
|---|---|---|
| DR-024 | Compact authoritative research checkpoint | 07 |
| DR-025 | Ordered writes with lightweight recovery | 07 |
| DR-027 | Impact-based subphase reopening | 09 |
| DR-038 | Impact-based autonomous project reopening | 09 |
| DR-039 | Shared knowledge with contextual revalidation | 09 |
| DR-040-R | **Standalone GTM skill; no Goal Memory dependency** | 07 |
| DR-041-R | Self-contained workspace initialization and fail-safe recovery | 07 |
| DR-042-R | Minimal documented **internal** OKF contract | 07 |
| DR-043 | Hybrid semantic and operational record organization | 08 |
| DR-044-R | Workspace-wide concept IDs and scoped research IDs | 08 |
| DR-045 | Lightweight consequential cross-project dependencies | 09 |

## Part IV — Research Outputs and Lifecycle (8)

| Decision | Primary rule | Chapter |
|---|---|---|
| DR-026 | Autonomous contract-verified subphase completion | 13 |
| DR-033 | Evidence-calibrated transferable lessons | 10 |
| DR-034 | Authoritative OKF plus derived research synthesis | 10 |
| DR-035 | Configurable, nonblocking learning checkpoints | 12 |
| DR-036 | Versioned selective synthesis maintenance | 10 |
| DR-037 | Autonomous charter-verified project completion | 13 |
| DR-050 | Docusaurus-style Markdown-first OKF book | 11 |
| DR-051 | Complete company GTM overview and adaptive deep dives | 11 |

## Part V — Implementation and Quality (3)

| Decision | Primary rule | Chapter |
|---|---|---|
| DR-048 | Static specification/implementation review | 14 |
| DR-049 | Consolidated specification before small implementation increments | 14 |
| DR-052 | Four internal quality checks and final user review | 14 |

**Primary coverage:** 13 + 17 + 11 + 8 + 3 = **52 unique decisions**. `-R` marks the standalone architectural replacement of the corresponding earlier wording; it is not an additional decision. Original decision histories and the standalone amendment must be preserved.

## Namespaces

The `DR-###` strings above are **skill-design decision labels**, not OKF semantic concept IDs. Future research operational decisions use scoped IDs such as `PRJ-0001:DEC-0001`, and reusable semantic concepts use workspace-wide IDs such as `K-000001`.

## v2 interpretation

The 52 historical labels retain identity, with current workflow semantics governed by the [v2 amendment](audit-reconciliations.md). No new project decision or historical approval is fabricated. Consolidated authority replaces per-phase gates; specification chapter count is not company-book chapter count.
