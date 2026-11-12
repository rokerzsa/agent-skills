# GTM Deep Research — Complete Specification Book

**Status:** Approved five-part, fourteen-chapter **standalone GTM Deep Research** behavioral specification (DR-001–DR-052, safeguards R-01–R-08 and standalone architectural amendments). All chapters are materialized. This book is the normative skill specification; static validation is not a live execution test.

## How to read this book

The sections form a Docusaurus-style, Markdown-first **OKF specification book**. It governs the skill's intended behavior. A *company research book* is a different, charter-defined, evidence-linked output derived from the research workspace's source/claim/concept records. Readers may follow the sequence or jump to the indexed procedure.

| Part | Chapter range | Start here |
|---|---|---|
| I — Research Foundations | 01–02 | [Part I index](part-01-foundations/index.md) |
| II — Investigation Methodology | 03–06 | [Part II index](part-02-investigation/index.md) |
| III — OKF Knowledge Architecture | 07–09 | [Part III index](part-03-okf-architecture/index.md) |
| IV — Research Outputs and Lifecycle | 10–13 | [Part IV index](part-04-outputs-lifecycle/index.md) |
| V — Implementation and Quality | 14 | [Part V index](part-05-implementation/index.md) |

## Complete chapter reading order

1. [01 — Research Modes and Charters](part-01-foundations/01-research-modes-and-charters.md)
2. [02 — Governance and Planning](part-01-foundations/02-governance-and-planning.md)
3. [03 — Research Contracts and Investigation](part-02-investigation/03-research-contracts-and-investigation.md)
4. [04 — Evidence and Source Integrity](part-02-investigation/04-evidence-and-source-integrity.md)
5. [05 — Independent Red-Team Review](part-02-investigation/05-independent-red-team-review.md)
6. [06 — Research Budgets](part-02-investigation/06-research-budgets.md)
7. [07 — Standalone OKF Workspace and Research State](part-03-okf-architecture/07-standalone-okf-workspace.md)
8. [08 — Research Records and Identity](part-03-okf-architecture/08-research-records-and-identity.md)
9. [09 — Shared Knowledge and Dependencies](part-03-okf-architecture/09-shared-knowledge-and-dependencies.md)
10. [10 — Research Synthesis and Lessons](part-04-outputs-lifecycle/10-research-synthesis-and-lessons.md)
11. [11 — Book Architecture and Navigation](part-04-outputs-lifecycle/11-book-architecture-and-navigation.md)
12. [12 — Human Learning](part-04-outputs-lifecycle/12-human-learning.md)
13. [13 — Completion and Acceptance](part-04-outputs-lifecycle/13-completion-and-acceptance.md)
14. [14 — Standalone GTM Research Skill Implementation and Review](part-05-implementation/14-skill-implementation-and-review.md)

## Operational reference index

| Area | Procedure(s) |
|---|---|
| Activation, reconnaissance and approval | [Activation and gates](../references/activation-and-approval-gates.md) · [Discovery/charter](../references/goal-discovery-and-charter.md) · [Planning/contracts](../references/progressive-planning-and-contracts.md) |
| Investigation and evidence | [Execution](../references/investigation-execution.md) · [Sources/claims](../references/source-and-claim-evidence.md) · [Gaps/journal](../references/gaps-and-journal.md) |
| Review and resources | [Independent red-team](../references/red-team-and-adjudication.md) · [Adaptive budgets](../references/research-budget-management.md) |
| OKF identity, persistence and recovery | [Standalone conventions](../references/standalone-okf-conventions.md) · [Recovery and consistency](../references/recovery-and-consistency.md) |
| Research outputs and learning | [Synthesis/lessons](../references/research-synthesis-and-lessons.md) · [Book structure](../references/research-book-architecture.md) · [Selective revisions](../references/synthesis-revisions.md) · [Learning](../references/human-learning.md) |
| Research lifecycle | [Completion and acceptance](../references/completion-and-acceptance.md) · [Dependencies/reopening](../references/dependency-impact-and-reopening.md) |
| Quality | [Final static audit](../references/final-static-audit.md) · [Glossary/topic index](appendices/glossary-and-topic-index.md) |

## Empty templates — not actual researched evidence

- **Authorization:** [Charter](../templates/research-charter.md) · [Plan](../templates/research-plan.md) · [Contract](../templates/research-contract.md) · [Decisions](../templates/project-decisions.md) · [Budget ledger](../templates/research-budget-ledger.md)
- **Research records:** [Sources](../templates/source-register.md) · [Claims](../templates/claim-register.md) · [Gaps](../templates/gap-register.md) · [Journal](../templates/investigation-journal.md) · [Knowledge concept](../templates/knowledge-concept.md) · [Red-team](../templates/red-team-review.md)
- **Knowledge books and teaching:** [Book index](../templates/research-book-index.md) · [Chapter](../templates/research-book-chapter.md) · [Revision log](../templates/synthesis-revision-log.md) · [Learning note](../templates/learning-checkpoint.md)
- **Completion/reopening/recovery:** [Subphase dossier](../templates/subphase-completion-dossier.md) · [Project dossier](../templates/project-completion-dossier.md) · [Dependency impact](../templates/dependency-impact-register.md) · [Reopening](../templates/reopening-record.md) · [Active state](../templates/project-active-state.md) · [Workspace state](../templates/workspace-state.md)

## Book reference aids

- [Glossary and topic index](appendices/glossary-and-topic-index.md)
- [First-time OKF initialization checklist](../references/workspace-initialization.md) · [Synthetic evidence-link example](../references/examples/synthetic-evidence-chain/index.md)

## Indexes, decisions and implementation history

- [Primary DR-001–DR-052 coverage](appendices/decision-coverage.md)
- [R-01–R-08 and standalone architecture supersession](appendices/audit-reconciliations.md)
- [Increment 1 history](appendices/increment-1-review.md) · [Increment 2](appendices/increment-2-review.md) · [Increment 3](appendices/increment-3-review.md) · [Increment 4](appendices/increment-4-review.md) · [Increment 5](appendices/increment-5-review.md) · [Increment 6 implementation history](appendices/increment-6-review.md)

## Evidence and governance invariants

**Source actually inspected → qualified and contradicted claims → semantic `K` concepts → independent `RT` where major → derived research book → dossier-based completion**, with adaptive budgets and optional learning throughout. Evidence state, qualitative confidence, review, project lifecycle and progress are distinct. A material newly encountered contradiction may reopen only affected work; no monitoring service is implied. Human charter, plan, budget and release gates cannot be bypassed.

**Operational and historical distinction:** This book defines how an authorized GTM research session operates. Build history and package-review decisions are recorded separately in the historical appendices; opening this book never authorizes installation, workspace initialization, expenditure, or substantive research.

## Current workflow amendment

User-directed v2: [one execution agreement](../references/activation-and-approval-gates.md), [strategy/current-state coverage](../references/strategy-and-current-state.md), one whole-company GTM chapter with adaptive deep dives, autonomous internal reviews and delivery ready for user review. See [supersession record](appendices/audit-reconciliations.md); historical increment reports do not certify this revision.
