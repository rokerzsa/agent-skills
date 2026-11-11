# Final audit reconciliations — R-01 through R-08

[Book home](../index.md) · [Decision map](decision-coverage.md)

The complete consolidated behavioral specification and these eight safeguards were explicitly approved. A **subsequent approved standalone amendment** removed the previous Goal Memory dependency, superseding the original generic-OKF-integration wording in Chapters 07–09 and 14, with conforming terminology changes elsewhere.

| ID | Safeguard | Standalone interpretation |
|---|---|---|
| R-01 | Prevent identity collisions | Distinguish `DR-###` skill decisions, workspace concepts (`K-...`), and qualified project records (`PRJ-...:SRC-...`). Never use the design-decision label as a live concept allocator result. |
| R-02 | Make contract authorization unambiguous | Every executable contract fits an explicitly approved detailed plan; material new scope/approach requires approval before work. |
| R-03 | Protect critical-gap and red-team completion gates | A critical unresolved blocker cannot be relabeled as noncritical. Required disputes must be resolved, authorized as qualified outcomes when permitted, or remain blocked. Human approval does not confer historical certainty. |
| R-04 | Protect hard budgets with uncertain usage | If compliance with an authorized hard ceiling cannot be verified, do not risk exceeding it; seek measurable usage, a safer alternative or fresh authorization. Estimates are not spending authority. |
| R-05 | Reconcile continuous evidence recording with unavailable OKF | Substantial stateful research cannot proceed without durable recording and recovery. Read-only diagnosis is permitted; no shadow store. |
| R-06 | Separate reopening from permission to execute | Material new evidence can reopen/flag a project; it cannot authorize new spending, charter scope or unapproved plans. |
| R-07 | Distinguish specification authority from historical evidence authority | The approved specification governs skill behavior. The research book is derived from authoritative OKF sources, claims and concepts; elegant prose does not override evidence. |
| R-08 | Static inspection is not runtime verification | Static review supports coverage and consistency claims, not proven reliability. Under the standalone amendment, verify the **internal OKF workspace contract**; do **not** inspect or depend on Goal Memory. |

## Architecture supersession record

**Original wording:** DR-040/041/042 required a research skill layered on generic OKF/Goal Memory. DR-044 delegated global concept identities externally.

**Approved replacement:** DR-040-R/041-R/042-R/044-R establish a standalone GTM Deep Research skill that owns its OKF workspace, initialization, identity allocation, decisions, checkpoints, and recovery. Chapters 07–09 and 14 were revised; Chapters 01–04 and 10–13 receive conforming ownership terminology. Other research rigor and governance decisions remain substantively unchanged.

**Implementation implication:** the standalone package now also documents contract/charter-verified autonomous completion, selective reopening, dependencies and recovery; all fourteen chapters are materialized. Do not initialize a user workspace, install the skill, or conduct real company research as part of packaging. When later authorized, the same evidence and human approval gates remain binding.

## Review boundary

The full specification is materialized as fourteen Markdown chapters. Implementation history is retained in the separate historical review appendices. **Installation, user workspace initialization and live GTM execution require their own applicable authorizations.** All eight reconciliations and the standalone amendment remain in force.
