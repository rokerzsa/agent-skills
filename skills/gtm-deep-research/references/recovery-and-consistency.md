# Recoverable OKF writes and consistency

[Book home](../book/index.md) · [Chapter 07](../book/part-03-okf-architecture/07-standalone-okf-workspace.md) · [Standalone conventions](standalone-okf-conventions.md) · [Workspace state](../templates/workspace-state.md) · [Active state](../templates/project-active-state.md)

**Authority:** DR-024, DR-025 and R-01/R-05/R-06. The self-contained GTM workspace uses lightweight, single-writer Markdown conventions. This procedure provides *logical recovery*, not a promise of cross-file transactions, concurrency safety, or atomic distributed commits. No Goal Memory dependency, no shadow store.

## 1. One writer and one checkpoint per project

Before any stateful operation verify the user-approved workspace root; workspace identity/convention version; `control/workspace-state.md` project and concept counters; project `record-ids.md` counters; active checkpoint; pending recovery markers; and whether other writers or inconsistent external sync make writes unsafe. If conflicting writers or stale snapshots cannot be reconciled, **stop affected writes**. There is no automatic safe concurrent allocator.

`control/workspace-state.md` is the authority for workspace-wide `K` and project identities. `projects/<PRJ>/record-ids.md` is the authority for scoped `SRC`/`CLM`/`RC`/`RT`/`GAP`/`DEC` IDs. Local ledger entry anchors (e.g. `REV` or `LRN`) are not global concepts or permission to reset counters. `DR-###` labels refer solely to approved skill-design decisions.

## 2. Before operation: identify dependencies and approval

- Determine the approved charter/plan/contract, and actual `DEC` authorization when a human gate applies. No inference of approval from a drafted proposal.
- Identify target stable IDs, existing record versions, affected dependent indexes/chapter links, journals, reviews, budgets and project checkpoint.
- Assess budget observability/limits for any further source or model work, including paid access; if enforcement is uncertain, do not risk overrun.
- Check pending recovery; do not start a new dependent write while earlier work could be incomplete.

## 3. Ordered write protocol

**Allocate identity durably → persist substantive records → update dependent references/indexes/journal → verify consistency → advance checkpoint last.**

For an allocated `K` or scoped ID, advance and persist the authoritative issuance counter **before** creating the corresponding record. Number gaps are acceptable after crash; reusing an issued number is forbidden. Keep a short operation/recovery marker indicating what the current multi-record change is doing when consistency depends on more than one write. For changes requiring no new IDs, retain stable IDs and previous substantive versions where materially necessary.

Substantive content may include inspected source provenance, changed claim confidence, `RT` verdict, authorized `DEC`, budget ledger event, semantic concept, reopening impact record, versioned synthesis revision or completion dossier. Record the actual artifact and its traceable basis before dependent status is advanced. Update related links, indexes and meaningful journal entries. Then check exact reference resolution and status coherence: e.g. complete implies valid dossier and mandatory reviews; reopened implies old dossier retained; review `passed` does not mean evidence verified.

Advance *only* the single authoritative project checkpoint after the above checks. Its next action must be one that is currently authorized.

## 4. Failure-window repair table

| Last durable state after interruption | Correct recovery |
|---|---|
| Counter increased, target record missing | Preserve spent identity; inspect any partial artifact; repair using **new** identity if needed, never decrement allocator |
| Substantive source/claim record exists, index link missing | Preserve source/claim; update appropriate link, registry and journal, then validate |
| `RT` review partly written with no evidentiary verdict | Preserve separate investigation history; leave `pending`, never fabricate `passed` |
| Budget event reserved, actual usage uncertain | Reconcile with available measurement and ledger; halt affected work until hard-limit safety is demonstrable |
| Material evidence revision made, dependent conclusions not yet marked | Record/recover pending dependency-impact flags, repeat required review and selective book updates |
| Completion dossier exists, checkpoint still active | Validate *all* charter/contract gates, approvals, evidence, book and links; advance only if valid; otherwise retain dossier as draft |
| Checkpoint says complete, required dossier or review absent | Treat as inconsistent, suspend dependent work, restore accurate checkpoint only from durable evidence; do not invent history |
| Project reopened, old dossier overwritten or missing | Halt and recover prior history from valid version/audit artifact; do not claim clean reopening without it |
| Approval proposal exists but actual human decision is missing | Keep `proposed`; do not grant authority |
| Book chapter moved but semantic links broken | Preserve stable `K`/qualified record IDs; repair navigation and references before checkpoint advance |

## 5. Invariant checks before resumption

1. Workspace root and convention version are known and authorized; one active writer.
2. Issuance counters are monotonic, not below any issued/reserved ID evidence, and never reset.
3. Every currently referenced material `K`/`PRJ:SRC`/`CLM`/`RT`/`DEC` resolves or is explicitly marked temporarily missing with impact.
4. Approval status is grounded in actual human decision statements and exact target versions.
5. Evidence, confidence, review, lifecycle and execution states are not silently collapsed.
6. Required red-team/adjudication and budget ceilings are respected.
7. Completion and reopening dispositions agree with dossiers/impact records.
8. Revision history preserves material former interpretations.
9. Only after these checks is the next action authorized to proceed.

If any invariant cannot be confidently restored, leave a visible recovery marker and escalate; a partial recovery report is preferable to false success. Avoid heavyweight rollback/transaction machinery unless separately approved.

## 6. Packaging versus live workspace

Templates and procedures shipped in the skill bundle are not an initialized project. Do not create a live workspace, install the skill, spend money, research a real company or alter a user's repository during package production. Static checks of package links cannot establish live recovery correctness or actual concurrency safety.
