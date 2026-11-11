# Standalone OKF workspace — foundational conventions

[Back to book](../book/index.md) · DR-024/025, DR-040-R–042-R, DR-043/044-R · **Standalone workspace conventions**

## Boundary and ownership

The GTM Deep Research skill is standalone. **Do not require Goal Memory, `memory temp/`, any external goal/decision registry, or any inherited allocator.** The skill owns research charters, plans, decisions, concepts, evidence, active-state checkpoints, audit, and recovery in one OKF workspace. OKF here means a Markdown-first, semantic, indexed and linked knowledge organization; no Docusaurus site or database is required.

These conventions govern research records, red-team reviews, budget ledgers, completion dossiers, revision history and recoverable state. They do not themselves initialize a deployed workspace. Do not create a live workspace until the human approves its location and initialization. User research data is not included in the distributed skill package.

## Proposed logical layout

```text
<approved-research-root>/
├── index.md                       # Project list + book/navigation entry
├── control/
│   ├── workspace-state.md         # Workspace identity + monotonic concept counter
│   └── conventions.md             # Pinned local convention revision
├── knowledge/
│   ├── index.md                   # Reusable semantic concept index
│   └── K-000001-topic.md          # Example concept (only when needed)
└── projects/
    └── PRJ-0001-company-gtm/
        ├── index.md               # Project ID, charter/book/records navigation
        ├── charter.md             # Approved scope/criteria and amendments
        ├── plan.md                # Approved phases and immediate plan
        ├── decisions.md           # Human decisions, evidence of authorization
        ├── active-state.md        # Compact authoritative research checkpoint
        ├── record-ids.md          # Issued local IDs per record type
        ├── contracts/             # Created as warranted
        ├── evidence/              # Registries created as warranted
        ├── investigation-journal.md
        └── book/
            ├── index.md
            └── ...                 # Part/chapter Markdown on demand
```

This is a **proposal for the eventual research root**, not a directory tree to instantiate in this review. A real initialization should create only the minimum files necessary for the authorized project. Avoid empty registries and one-file-per-trivial-claim.

### Identity namespaces

| Category | Illustrative ID | Scope | Issuance owner |
|---|---|---|---|
| Workspace-wide semantic concept | `K-000001` | One approved research root | `control/workspace-state.md` |
| Research project | `PRJ-0001` | One approved research root | Workspace project counter |
| Source | `SRC-0001` | A project/registry | Project `record-ids.md` |
| Claim | `CLM-0001` | A project/registry | Project `record-ids.md` |
| Contract | `RC-0001` | A project/registry | Project `record-ids.md` |
| Red-team review | `RT-0001` | A project/registry | Project `record-ids.md` |
| Gap | `GAP-0001` | A project/registry | Project `record-ids.md` |
| Decision record | `DEC-0001` | A project/registry | Project `record-ids.md` |
| Design decision | `DR-001` | Approved *skill-design* history | **Never** issued as research ID |

IDs above are proposed for implementation review. Numeric sequence widths and record conventions may be adjusted by a subsequent **approved** plan change. IDs must remain stable across moves and never be recycled. A gap in a sequence is acceptable after an interrupted allocation. A filename or Markdown line number is **not** the record's canonical identity.

**Qualified reference:** `PRJ-0001:SRC-0001`, not `SRC-0001` alone across projects. The project ID is stable even if the project's directory slug changes. A globally reusable concept is referenced by `K-000001` within that workspace. To reference a separate external workspace, additionally identify the workspace and preserve the provenance; do not assume global uniqueness across repositories.

### Issuance protocol and interrupted writes

- **One writer** at a time may allocate IDs in the Markdown workspace; if concurrent modification is suspected, stop and reconcile.
- Read and validate the authoritative counter against existing IDs. If ambiguous or inconsistent, do not issue an ID; investigate or escalate.
- Increment and persist the counter/issued-ID ledger **before** writing the corresponding record. Once issued, the ID is consumed even if record creation fails.
- Persist the identified substantive record, then repair affected semantic indexes, back-references and journal entries, check consistency, and **only then** advance the authoritative active checkpoint.
- Never decrement the ID counter or fill apparent ID gaps automatically. Preserve tombstones/supersession references where relevant.

A temporary Markdown editor save or shell write is not automatically a transaction. This foundation does not promise atomic multi-file commits.

## Required minimal document contracts

### Workspace index (`index.md`)

- Workspace identity and scope; actual root chosen by user.
- Links to shared knowledge index and existing project indexes.
- Link to `control/conventions.md` and compatible control metadata.
- Navigation only: **not** an alternate active-state or approval ledger.

### Workspace state (`control/workspace-state.md`)

- Stable workspace identity, schema/convention revision, current project ID counter and concept `last_issued` counter.
- Consistency/recovery note if an interrupted allocation or write is discovered.
- This file owns workspace-wide counters, **not** truth of substantive historical claims.

### Project decisions (`decisions.md`)

- Each consequential proposal and explicit human decision has a stable scoped ID and the affected charter/plan/budget or action.
- Store an actual decision statement and a usable pointer or quote from the authorization, not a fabricated timestamp or generic `approved: true` with no attribution.
- If authorization is ambiguous or its evidence absent, treat the action as **not approved** until clarified.
- Design decisions (`DR-###`) and project decisions (`PRJ-###:DEC-###`) are distinct.

### Project active state (`active-state.md`)

- Project ID, current approved charter version, phase/subphase, approved research contract reference, execution status.
- Pending evidence questions/leads, blocked dependencies, review gates, pending human decisions.
- Budget authorization/usage references, next permissible action, interrupted operation/recovery marker.
- References substantive records rather than duplicating their content. Only one authoritative checkpoint per active project.

### Shared knowledge index (`knowledge/index.md`)

- Semantically grouped concepts and stable `K-...` identities.
- Links to source/claim provenance and originating projects where applicable.
- Cross-project dependencies for **consequential** analytical reliance, not every ordinary Markdown link.

## First-time workspace initialization resources

See the [approved initialization checklist](workspace-initialization.md), [workspace conventions template](../templates/workspace-conventions.md) and [knowledge index template](../templates/knowledge-index.md). The templates describe the four minimal control/index documents; they do not create a user workspace or allocate IDs merely by being shipped with the skill.

## Human approvals and start conditions

Workspace initialization requires explicit approval of the selected root and non-destructive creation. A full research project separately requires explicit approval of the charter, high-level phase outline, and immediately executable detailed plan. No project becomes authorized merely because its folders exist.

Early reconnaissance may be bounded and used to ask informed questions, but substantive persistent research cannot proceed without the required durable workspace or approval gates. If the workspace is missing or inconsistent, stop unsafe stateful work. Never create a shadow store to reconcile later without a separate approved change.

## Safe write sequence

1. **Check** workspace readiness, current authorization, source provenance, ID state, and absence of unresolved recovery.
2. **Allocate** stable identities durably before use.
3. **Write** source, claim, concept, decision, review, or contract content as applicable, preserving explicit provisional states.
4. **Update** indexes, consequential dependencies, cross-references and the summarized journal.
5. **Validate** that target records exist, IDs are unique within scope and required links resolve.
6. **Advance** only the affected project's authoritative active state.

If the process stops after step 3, recovery should preserve the valid record and repair references before advancing state. It must not repeat the ID as if unused.

## Recovery and failure policy

- Missing workspace: seek authorization and follow initialization; no destructive "reset".
- Existing inconsistent workspace: inspect references/IDs/checkpoint, preserve valid records and reconcile; unsafe writes halt.
- Incompatible convention/schema: stop affected operations and request a compatible migration or approved update.
- Missing approval: stop the affected consequential action; record a proposal, not an approval.
- Unmeasurable hard budget usage: do not risk passing the authorized ceiling; use safer execution or seek permission.
- Failed write: preserve durable records and issued identities, reconcile linked indexes, then resume authorized work.

## Evidence, research books, completion and reopening invariants

The skill maintains source provenance, claim-level evidence and synthesized semantic concepts as linked but distinct layers; it supports actual documented adversarial reviews, budget ledger events, and **reader-facing Markdown-first research books** with chapter/part indexes and stable evidence links. Evidence states, qualitative confidence, independent review, execution and lifecycle status remain separate. The book is a **derived synthesis**, never a second authority overriding underlying `SRC`/`CLM`/`RT`/`K` records. [Book architecture](research-book-architecture.md) · [Synthesis](research-synthesis-and-lessons.md) · [Revision policy](synthesis-revisions.md).

## Template usage

The `templates/` files are **illustrative, non-executable drafts** for review, not an instruction to initialize the user's workspace automatically. Create only authorized live records after confirming the root. Evidence-linked research books, selective versioned synthesis and optional learning checkpoints are available. [Completion/dossiers](completion-and-acceptance.md), [dependencies/selective reopening](dependency-impact-and-reopening.md), and [interruption recovery](recovery-and-consistency.md) retain their own separate requirements and authorization gates.


## Evidence, independent review and budget-record persistence

- Create an actual [source registry](../templates/source-register.md), [claim registry](../templates/claim-register.md), [gap registry](../templates/gap-register.md), [journal](../templates/investigation-journal.md), or [semantic concept](../templates/knowledge-concept.md) **only after** root and active contract approvals and a material record need. The bundled files are templates, not evidence of real research.
- A grouped registry must carry an explicit canonical `PRJ-...:SRC-...`, `PRJ-...:CLM-...`, or `PRJ-...:GAP-...` on each record; retain a lightweight ID→current-location lookup in the registry or project index. Moving/splitting files changes location, **not identity**.
- Evidence-record access states are distinct from claim confidence, evidence support, review, record lifecycle and active execution. Major conclusions require `review: pending` until a genuine authorized [independent red-team procedure](red-team-and-adjudication.md) completes with a justified `RT` outcome.
- Record direct evidence, secondhand description and failed original-source recovery separately. Preserve source information lineage to avoid treating copy/PR syndication as independent corroboration.
- When an update changes a material claim, preserve reasons, counterevidence and any prior interpretation before updating the related concept/index; unresolved material references block checkpoint advancement.
- Closing an evidence-exhausted **noncritical gap** is permitted under [the gap procedure](gaps-and-journal.md). [Independent red-team verdicts](red-team-and-adjudication.md) and [preauthorized budget extensions](research-budget-management.md) use distinct durable review/ledger records. Derived books and learning do not establish completion; criterion-based closure and material reopening follow their [separate lifecycle procedures](completion-and-acceptance.md).

## `RT` review records and budget ledger linkage

- Issue each independent `RT` ID through the **existing project `record-ids.md`**, before writing the [review record](../templates/red-team-review.md). `RT` is a procedural review identity, never the claim evidence state. Its target claim must reference the actual `RT` verdict and preserve old review history.
- A budget ledger is **one logical project record**, not another decision authority or a new global ID sequence. Reference original charter/plan/contract and scoped `DEC` approvals. Event markers may be ledger-local stable anchors; do not invent a `BUD` global allocator.
- Persist real extension justifications, event-level consumption, source/claim/review changes, budget authorizations and consequential decisions before indexes, journal links, and finally checkpoint. If a usage amount or paid authorization is unknowable, **do not guess, spend or advance the activity**.
- Reconcile parent/phase/subphase allocations against all applicable dimension hard ceilings without counting a consumption event more than once. On interrupted usage or ambiguity, halt affected operations, retain consumed IDs and event history, and reconcile before issuing further resources.
- The [red-team procedure](red-team-and-adjudication.md) and [budget procedure](research-budget-management.md) may execute within an initialized, authorized workspace; **no live research workspace is initialized by this skill package**.


## Book, revisions and learning state

- A project book is a **derived, reader-facing collection** within the one approved workspace. Its `book/index.md`, part indexes, chapters, revision ledger and optional learning notes must **reference** existing semantic concepts and scoped `CLM`/`SRC`/`RT` records. Do not treat chapter prose as a new primary source or create a duplicate evidence/decision ledger.
- Generate draft book navigation from the [charter-approved outline](research-book-architecture.md). Maintain relative Markdown links **and** stable canonical IDs; significant top-level structure changes need the applicable explicit human approval.
- Material evidence changes are persisted upstream before affected [synthesis revisions](synthesis-revisions.md). Retain meaningful prior-version wording, source trigger and current `RT` status; revise only affected sections and downstream lesson statements, then validate links/indexes and advance the project checkpoint **last**.
- [Learning checkpoints](human-learning.md) are optional compact project learning notes. Their `LRN` local anchors and revision ledger `REV` anchors are navigation markers, **not** new workspace-wide `K` or research record allocators; no fabricated learner responses or approvals. Learning is nonblocking by default.
- **Completion:** Autonomous closure follows [criterion-by-criterion contract/charter checks](completion-and-acceptance.md), not polished prose. Material evidence can trigger [selective reopening](dependency-impact-and-reopening.md) while preserving prior dossiers, but new spending or plan execution remains separately authorized. [Recovery](recovery-and-consistency.md) never advances the checkpoint before validated durable records. Skill installation/release is still human-gated.
