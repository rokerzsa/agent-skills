# Activation and approval gates — complete six-increment workflow

[Book home](../book/index.md) · [Chapter 01](../book/part-01-foundations/01-research-modes-and-charters.md) · [Chapter 02](../book/part-01-foundations/02-governance-and-planning.md)

## Choose research depth, not answer length

Deep Research is for consequential GTM investigation and historical reconstruction, including market context, early users, paying customers, business model, distribution, sales, pricing, competition, failed experiments, and causal claims.

Consider **complexity, evidence uncertainty, causal significance, decision impact and expected effort**. A short question can require extensive research; a long explanatory question may not. When genuinely borderline, ask **one targeted clarification**, not a discovery questionnaire.

| Mode | Illustrative request | Response |
|---|---|---|
| Lightweight | “When was this company founded?” | Direct answer or ordinary lookup; no charter machinery |
| Borderline | “Compare two assessment companies' pricing.” | Assess complexity; clarify rigor only if material |
| Full | “Reconstruct the first 100 paying customers and causal GTM changes.” | Bounded reconnaissance → goal grilling → approved charter/plans/contract → authorized question-driven evidence investigation under approved investigation, review, budget, book and completion safeguards |

## Approval matrix

| Action | Authority and timing | Evidence required |
|---|---|---|
| Brief bounded reconnaissance for informed questions | Codex, within constraints; **not** full investigation | Record important provisional findings if a workspace exists |
| Initialize or change the live OKF workspace root | Explicit human authorization before writes | Root and non-destructive initialization approval |
| Approve goal and charter | Human; before planning is treated as authorized | Identified charter version and explicit decision |
| Approve high-level phase outline | Human; separate from charter approval | Plan version and phase outline identified |
| Approve immediate detailed plan | Human; before contract execution | The detailed phase/subphase and attached contract(s) explicitly identified |
| Prepare contract within approved immediate plan | Codex may draft; execution governed by detailed approval | Charter, plan and decision references |
| Routine scope-respecting planning refinements | Codex | Document substantive change; no new consequential authority |
| Consequential charter, question, scope or plan change | Human before taking effect | Amendment, impact and explicit approval |
| Material expansion of approved subject-specific discovery framework | Human | Proposed extension with rationale and approval |
| Use preauthorized research effort extension | Codex only within an expressly approved allowance | Authorized ceiling and justification |
| Exceed hard budget ceiling or incur new paid cost | Explicit human approval **before** action | Scope, amount/dimension and decision |
| Conduct substantive investigation | Only after relevant approvals and the authorized investigation/budget start gate is satisfied | Approved contract, authorized workspace, checkable budget ceiling and recovered state |
| Mark subphase or project complete | Codex, after objective charter/contract conditions and mandatory reviews pass | Valid [completion dossier](completion-and-acceptance.md) and checkpoint-last update; no extra human acceptance by default |
| Reopen completed work upon material evidence | Codex may flag/reopen, not silently spend or expand | Reopening reason, affected scope, applicable fresh approvals |
| Install skill or advance implementation increments | Human | Explicit increment/release authorization |

Approval of one gate does not approve the next. A combined review of the detailed plan and its exact contract can be one human decision when both are clearly identified; it does **not** collapse charter or high-level plan approvals into that decision.

## Approval recording

After user approval and **only in an authorized initialized workspace**, issue the next project-scoped `DEC` identifier and write to `decisions.md` using [project decision conventions](standalone-okf-conventions.md). Preserve:

- Actual human decision statement or faithful quotation, with usable conversation/document reference when available.
- Identified target and version (charter, high-level plan, immediate detailed plan, specific contract, or amendment).
- Disposition (`approved`, `rejected`, `revision requested`, etc.), consequential rationale and dependencies.
- Link to previous versions and affected decisions.

If approval evidence cannot be persisted or a user decision is ambiguous, **do not** mark the action approved. Preserve the proposal, ask the targeted question, or halt the affected write. No fabricated approval attribution or timestamps.

## Gate sequence and example

1. User requests substantial GTM reconstruction; Codex determines this is full Deep Research.
2. Codex performs bounded reconnaissance and targeted rounds of discovery covering all thirteen mandatory dimensions.
3. Codex drafts charter version `v1` and asks for its explicit approval. A tentative “interesting” is not approval.
4. Only after charter authorization: Codex proposes the full high-level phase outline. Obtain a separate approval decision.
5. Codex proposes detailed first-phase plan `P1-v1` with contract `RC-0001` and asks for the exact execution boundary to be approved.
6. Save the decisions and approved versions, update links and state in recoverable write order.
7. Once the authorized start gate is verified, investigate contract questions and evidence, perform substantively independent [red-team work](red-team-and-adjudication.md) where mandatory, track [budget usage](research-budget-management.md), and when warranted apply the independent [completion audit](completion-and-acceptance.md). Do not infer completion from a performed search, a passed review or a finished-looking book.

## Failure cases

- **Workspace absent or root not authorized:** may discuss the plan in chat; must not silently persist it to a made-up root or pretend approvals are durable.
- **Workspace inconsistent or recovery pending:** halt affected persistent writes and reconcile first.
- **Charter approved, plan not approved:** high-level planning may be proposed, not executed as approved research.
- **Detailed plan approved but contract materially expands it:** revise the plan and obtain the consequential approval before execution.
- **An approved contract exists:** verify the actual research authorization, workspace consistency, budget constraints and contract fit before any authorized source investigation. A completed review requires a genuine separate [red-team pass](red-team-and-adjudication.md); never infer completion authority.
- **Hard limit unmeasurable:** do not risk overrunning it; propose a safer measurable approach or seek new authorization.

Learning discussions remain distinct from evidence assessments and governance decisions. Nonblocking learning cannot override a mandatory approval gate.

## Concurrency boundary

The foundational Markdown workspace assumes **one authorized writer** for counters, decisions, indexes and checkpoints. If simultaneous writers or ambiguous external synchronization are detected, halt affected operations and reconcile; do not claim transactional multi-file safety.

## Independent review, budget and derived-book gates

- A major/aggregate conclusion triggers an independent source-seeking red-team pass; the approved plan/contract and budget must cover its search methods. [Review procedure](red-team-and-adjudication.md).
- Use only documented explicitly preauthorized extension allowance; log the information-gain justification before draw. A proposed increase or paid access requires a separate **actual human `DEC` authorization**. [Budget management](research-budget-management.md).
- Review `passed`, `qualified` and `unresolved` are procedural dispositions, **never** automatic changes to evidence confidence, approval records, or contract/project completion.


## Derived output, learning, completion and reopening boundaries

- Draft book chapters may be written only from existing traceable `K`/`CLM`/`SRC` and applicable `RT` records, using the [synthesis](research-synthesis-and-lessons.md) and [book authoring](research-book-architecture.md) procedures. A book is not independent evidence.
- Material revisions require [preservation of prior interpretation](synthesis-revisions.md) and link updates; consequential top-level book restructuring must be approved under the charter.
- Optional [learning checkpoints](human-learning.md) are nonblocking by default and **never** stand in for charter, plan, budget or evidentiary approval.
- [Autonomous subphase/project completion](completion-and-acceptance.md) is allowed only after objective approved criteria, required independent review, critical-gap disposition and an auditable dossier. [Selective reopening](dependency-impact-and-reopening.md) is allowed on encountered material evidence with old dossiers preserved; reopening **does not** authorize new scope, spending or detailed plan. Human release/installation approval is still separate.
