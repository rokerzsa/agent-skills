# Chapter 08 — Research Records and Identity

[Previous: Chapter 07](07-standalone-okf-workspace.md) · [Part III](index.md) · [Book home](../index.md) · [Next: Chapter 09](09-shared-knowledge-and-dependencies.md)

**Governing decisions:** DR-043, DR-044-R. **Purpose:** Keep researched evidence and semantic knowledge stable, discoverable and reusable without one file per trivial claim or reliance on an external goal-memory allocator.

## 8.1 Hybrid semantic and operational organization

The standalone GTM workspace has two complementary knowledge arrangements. **Semantic OKF concepts** cover substantive subjects (e.g. market conditions, early enterprise acquisition, pricing evolution, distribution mechanisms and causal hypotheses), organized by meaning and linked across projects. **Operational records** serve execution, audit and recovery: charters, plans, contracts, source/claim registers, gaps, journals, `RT` reviews, budget ledgers, approvals, dependency impacts and completion dossiers. The operational layout must not dictate a reader-facing book's chapter structure.

Prefer consolidated, predictable registries for many related short records; split when clarity, audit, size or maintenance warrants it. Do not create hundreds of empty directories or one file per trivial source/claim. A substantive concept may have its own Markdown document and stable workspace identity when important or reusable.

## 8.2 Logical workspace layout

The authorized root has `index.md` for project navigation; `control/workspace-state.md` for shared allocation and convention version; `knowledge/` for workspace-wide semantic concepts and indexes; and `projects/<PRJ>/` for charter, plans, decisions, active state, scoped record issuance, evidence, contracts, journal and the project's derived research `book/`. Exact physical directories are created only when needed, based on [standalone conventions](../../references/standalone-okf-conventions.md). No Goal Memory or `memory temp/` dependency is permitted. The workspace is authoritative for research records; the book is derived and may reside in the same workspace.

## 8.3 Workspace-wide semantic concept IDs

Substantive semantic concepts receive `K-000001`, `K-000002`, etc., in one standalone workspace-wide monotonic sequence. The workspace control record is the sole allocation authority. Persist an increment **before** creating its concept; gaps in IDs are acceptable after interruptions but reuse is forbidden. Reorganizing or renaming files does not change `K` identity, and a concept's semantic links must remain resolvable when it is superseded. IDs are unique to the approved workspace, not necessarily globally unique across unrelated repositories.

## 8.4 Project-scoped operational IDs

Projects use a durable `record-ids.md` ledger to issue locally unique IDs. Typical prefixes include `SRC` for an inspected/source provenance entry, `CLM` for a defined assertion and evidence, `RC` for research contract, `RT` for independent red-team review, `GAP` for an unresolved question, and `DEC` for consequential human decisions. Their **qualified** form includes an unambiguous project identity, e.g. `PRJ-0001:SRC-0001`. These are not global concepts. Local `DEP`, `REV` or `LRN` navigation anchors may identify entries in their containing registries; they must not silently become a second global allocator.

Preserve identity across record movement/splitting, version changes and supersession. Never derive logical identity solely from line number or filename. Retire rather than reissue IDs; recover allocation counters after crash before issuing another. See [project ID template](../../templates/project-record-ids.md).

## 8.5 Distinct namespaces and state dimensions

`DR-001`–`DR-052` are skill-design decision labels, not live workspace IDs; research decisions use qualified `DEC` IDs. Do not conflate record identity with contents, supporting evidence, review disposition or lifecycle stage. Keep these separate:

| Dimension | What it means |
|---|---|
| Evidence | Supported, disputed, unverified or refuted assertion |
| Confidence | High, medium, low or unverified, with explanatory rationale |
| Review | Pending, passed, qualified, unresolved or not required |
| Record lifecycle | Current, superseded or retained for history |
| Execution | Planned, active, blocked, completed or reopened work |
| Resource authorization | Base allocation, approved extension, hard ceiling and consumption measurement status |

Recording a claim in an OKF registry does not endorse it. A completed procedural `RT` is not automatically high confidence. A completed phase is not proof of every historical proposition.

## 8.6 Reference and evidence integrity

The workspace supports relationships including: `SRC` supports/contradicts `CLM`; `CLM` contributes to `K`; `RT` challenges a major claim or aggregate conclusion; `RC` requires questions/outputs; a `K` concept depends on another concept/claim; a book chapter cites current `K`, `CLM`, `RT` and `SRC`; project conclusions materially depend on shared upstream evidence. Record source independence and original information lineage to avoid treating multiple copies of one interview as independent corroboration.

Implement with qualified IDs, Markdown references and lightweight indexes, not a mandatory graph database. Each material link must resolve or be explicitly flagged for repair/impact. Navigation and identity have different functions: moving a book chapter may change relative hyperlinks but cannot change the underlying source or concept's identity.

## 8.7 Recoverable creation and mutation

Allocate IDs durably; persist substantive records with real provenance or explicit provisional status; update index/reference/journal records; validate referents; advance the single active checkpoint **last**. When new evidence changes a claim, preserve consequential former meaning and affected `RT` state; update dependent `K` concepts/book sections only with appropriate evidence checks. A research contract cannot gain authorization through changing its metadata. For failure windows and non-reused issued IDs, follow [recovery](../../references/recovery-and-consistency.md).

## 8.8 Reader-facing presentation

The project book follows a charter-approved high-level outline with introduction, parts, chapters, topic and evidence indexes, a navigable sequence, limitations and revision links; its authoring rules are in [Chapter 11](../part-04-outputs-lifecycle/11-book-architecture-and-navigation.md). Raw registry order must not become the book's reading order. Significant historical conclusions remain traceable from book prose to concepts, claims, reviews and inspected sources.

## 8.9 Completion of record-architecture requirements

The architecture is sufficient when workspace concepts have stable `K` IDs; operational records have stable scoped IDs; sources/claims/reviews are traceable; files can split or move without losing logical identity; shared evidence is reusable with contextual checks; and no second authoritative store, global allocator, or external goal-memory dependency is introduced.

**Next:** [Chapter 09 — Shared Knowledge and Dependencies](09-shared-knowledge-and-dependencies.md) · [Recovery and consistency procedure](../../references/recovery-and-consistency.md).
