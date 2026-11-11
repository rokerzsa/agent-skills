# Contract- and charter-verified completion

[Book home](../book/index.md) · [Chapter 13](../book/part-04-outputs-lifecycle/13-completion-and-acceptance.md) · [Contract/investigation](investigation-execution.md) · [Independent red-team](red-team-and-adjudication.md) · [Completion templates](../templates/subphase-completion-dossier.md) / [project](../templates/project-completion-dossier.md)

**Authority:** DR-026 and DR-037. Codex may close a subphase or project **without a second human acceptance** only after the objectively approved contract/charter conditions are met. Completion is a procedural finding about authorized research work, **not** a claim that all historical uncertainties have been resolved. Never use budget exhaustion, a polished book, or a person's agreement to manufacture evidence.

## 1. Subphase closure gate

Before declaring a subphase complete, freeze the exact versions of its approved charter, high-level plan, detailed plan and contract; identify their actual scoped `DEC` authorization references. Evaluate each mandatory question against its contract outcome and supporting `SRC`/`CLM`/`K` evidence; preserve unknown answers and contradictory evidence. Confirm required source inspections and independently recorded `RT` reviews of **all impact-classified major and aggregate conclusions**, including review results and bounded adjudication. Check original/final evidence states and qualitative confidence independently from procedural review status.

Then evaluate unresolved gaps using [gaps and journal](gaps-and-journal.md). A noncritical evidence-exhausted gap may have a documented closure with searched avenues, why further effort is unlikely to help, downstream limitations and revisit trigger. A **critical** gap or consequential unresolved red-team dispute cannot be closed merely by renaming it: determine whether it blocks the charter/contract. An explicitly authorized qualified outcome is valid **only if** the currently approved completion conditions permit it and the critical issue has received its mandated escalation/disposition. If the requirement cannot be satisfied, leave status `blocked/incomplete` and request an amendment or needed decision; human authorization may change criteria but never turns historical uncertainty into certainty.

Validate dependent claims and concepts, approved budget/extension decisions, no unrecovered write/identity inconsistencies, and outputs required by the contract. Where the completed subphase is an upstream dependency, flag downstream work that must revalidate it before execution.

### Required closure dossier

Create a [subphase completion dossier](../templates/subphase-completion-dossier.md) with:

- Project/subphase ID, `RC` ID and version, charter/plan versions and exact `DEC` authorization references.
- Mandatory questions with `answered / qualified / unresolved`, the evidence chain, confidence and material rival explanations.
- All applicable `RT` IDs, adjudication dispositions and review-state caveats.
- Gaps, criticality, evidence-exhaustion rationale, escalations and revisit triggers.
- Material dependencies, downstream impacts, source/claim/concept and draft-book outputs.
- Budget allocations/consumption with measurement status, and any pending authorization.
- A **criterion-by-criterion** completion check, a reasoned disposition (`complete`, `complete with qualifications`, `blocked/incomplete`), reviewer/decision trace and outstanding actions.

Persist the dossier and required durable links/decisions, update project navigation and the meaningful journal, validate and **only then** advance the single [active-state checkpoint](../templates/project-active-state.md). A dossier *draft* with an unchecked requirement is not a completed subphase.

## 2. Phase progression is a separate gate

Autonomous closure of the present contract **does not approve** the next detailed phase plan. Before beginning dependent new work, verify the next plan/contract and resources have their own required authorization. Independent unrelated work may continue within its approved scope.

## 3. Project-level final charter audit

When all required phases/subphases have valid dispositions, compare the *current approved charter*, not merely the task list, with actual research outputs:

1. Each mandatory research question and completion criterion has an evidence-backed or expressly charter-permitted qualified outcome.
2. Every required phase/subphase meets its approved contract, with versioned dossiers and valid authorization.
3. All material sources, claim states, contradictions and confidence rationales are accessible from stable references; no source was falsely represented as inspected.
4. Consequential causal/strategic and aggregate conclusions have independent `RT` coverage and valid adjudication/disposition.
5. Critical gaps, material red-team disputes and invalidated charter assumptions have no unresolved blocker inconsistent with charter completion.
6. Cross-project and within-project dependencies are checked for materially invalidated upstream evidence, with limitations stated if coverage is incomplete.
7. The **reader-facing Markdown-first OKF research book** has the approved high-level structure, index/chapters, evidence links, relevant limitations, revision history and verified internal navigation.
8. Approved budget limits, actual/estimated/unavailable use, amendments and pending resource constraints are recorded, never fabricated.
9. No outstanding required human approval, recovery marker or durable-write inconsistency prevents completion.

Create the [project completion dossier](../templates/project-completion-dossier.md), referencing rather than copying source registries and the book. Distinguish `complete`, `complete with qualifications` (only when permitted by the charter), and `blocked/incomplete`. If criteria are satisfied, Codex may autonomously mark `complete` and present the dossier for human review. Do not invent final human acceptance; no such extra gate exists by default. If a charter explicitly requires a human review, obtain it first.

### Persistent write order

Persist completion evidence/dossier and authorized decisions → update relevant status, indexes, book links, dependencies and journal → validate exact referents and unfinished reviews → advance project checkpoint **last**. A partial closure attempt or invalid dossier must not appear as completed state. See [recovery](recovery-and-consistency.md).

## 4. Failure/exception matrix

| Situation | Valid treatment |
|---|---|
| Source evidence exhausted on a noncritical question | Qualified answer or documented noncritical gap closure when the contract allows |
| Critical first-paying-customer question unanswered and required | `blocked/incomplete`, escalate; do not mark `complete with qualifications` without an authorized criterion change |
| Required major conclusion review pending | Not complete; perform actual independent `RT` or remain blocked |
| Red-team review unresolved but charter explicitly permits qualified synthesis after required adjudication/escalation | Document permitted qualified outcome and rival explanations; do **not** mark fact verified |
| Project spent its full research budget | Reassess, request extension, or report blocked; never equate spending with completion |
| Chapter present but its evidence links broken | Book deliverable incomplete; repair before project closure |
| Active checkpoint says complete but dossier or permission absent | Recovery/inconsistency; do not ratify claimed completion |
| New evidence undermines prior completed conclusion | Follow [impact and reopening](dependency-impact-and-reopening.md), preserving old dossier |

## 5. Completion report to human

Present scope/charter version, verified outcome, findings and confidence limitations, reviewed major conclusions, unresolved gaps, spent/remaining budgets with measurement basis, accessible book and dossier references, and next decisions/revisit triggers. Do not claim a live research run was validated merely because the skill instructions passed static inspection.
