# Shared evidence dependencies, selective invalidation and reopening

[Book home](../book/index.md) · [Chapter 09](../book/part-03-okf-architecture/09-shared-knowledge-and-dependencies.md) · [Dependency register](../templates/dependency-impact-register.md) · [Reopening record](../templates/reopening-record.md) · [Revisions](synthesis-revisions.md)

**Authority:** DR-027, DR-038, DR-039, DR-045. Reuse authoritative evidence **by reference**, with contextual revalidation. A known material upstream change triggers downstream *reassessment*, not automatic proof that all dependents are false. Reopening a completed project changes lifecycle status; it **never** grants new scope, spending or plan execution authority.

## 1. Record only consequential dependencies

Use [the dependency impact register](../templates/dependency-impact-register.md) for important links: qualified upstream `PRJ:SRC` or `PRJ:CLM`, workspace `K`, reviewed major conclusion or approved assumption; downstream scoped claim, concept, chapter, research contract or project. Capture the actual dependence (e.g. an asserted early-enterprise-sales date is used in comparative timing), significance, evidence/review state at last validation, and when/whether it needs revalidation. Maintain a lookup from upstream stable ID to known dependents. Ordinary hyperlinks need not become dependency entries; do not introduce a mandatory full graph service.

When Project B reuses Project A evidence: follow qualified source identities, verify relevance, timeframe, origin, independence, contradictions, confidence and current review status. Distinguish source reuse from independent corroboration. A causal interpretation approved in Project A does not automatically meet Project B's research/red-team standard; record Project B's contextual conclusion separately.

## 2. Trigger and materiality assessment

Trigger assessment on **encountered** credible new evidence, substantive corrected dates/definitions, previously hidden shared-source lineage, changed confidence/contradiction, major red-team qualification, invalidated causal assumption or a changed completion basis. A mere formatting edit, file move with stable links, or equivalent wording should not initiate broad reopening.

For each material candidate:

1. Persist the newly accessed source and qualified claim/review change using normal [evidence rules](source-and-claim-evidence.md).
2. Find known dependents via qualified stable IDs, semantic links and impact register; state when lookup coverage is incomplete.
3. Assess whether the dependency changes an important claim, causal/strategic conclusion, approved assumption, mandatory review, completion dossier or final book passage.
4. Record materiality and reason; mark affected dependents `reassessment pending` (a dependency status, **not** an evidence-state verdict).
5. Selectively pause dependent work when an invalidated assumption makes continuing unsafe; leave independent tasks authorized and active.
6. Determine needed source checks, new red-team passes, charter/plan amendments and budget/paid authorization; do not execute missing approvals.
7. Complete authorized reassessment, update actual downstream evidence/review states independently, revise affected book sections and indexes, then clear only validated dependency flags.

**Rule:** An upstream change can make a dependent justification inadequate without proving the downstream claim false. Preserve competing interpretations until reassessed.

## 3. Completed subphase reopening

Reopen when credible new evidence materially affects a major subphase conclusion, critical dependency or the documented contract-completion basis. Preserve the original [subphase dossier](../templates/subphase-completion-dossier.md) and old completion checkpoint/record. Create [a reopening record](../templates/reopening-record.md) with original status and dossier version, new evidence/`SRC`/`CLM` or `RT` trigger, materiality threshold, directly affected questions and descendants, missing reviews, authorized versus pending action, and future closure conditions.

Minor evidence changes that do not undermine the conclusion or completion criteria update existing evidence and derived outputs without formal reopening. Do not restart unrelated subphases.

## 4. Completed project reopening

Codex may **autonomously mark** a completed project `reopened — assessment pending` when encountered credible evidence materially undermines a major project conclusion, critical dependency or approved charter completion basis. Persist the trigger and preserved previous [project completion dossier](../templates/project-completion-dossier.md). Identify affected scope and keep unaffected research closed.

Reopening does not mean research automatically resumes. New work requires the existing charter/detailed-plan/contract approvals and applicable [budget checks](research-budget-management.md). If new scope or spending is needed, prepare a proposal and wait. A new research plan cannot retroactively be treated as approved just because the project was reopened. The old completion status remains in history; the latest checkpoint may show `reopened/pending authorization` after consistent durable writes.

Retest applicable `RT` major-conclusion challenges and original completion conditions before closing reopened scope. Subsequent closure yields a new versioned dossier, not an overwritten original.

## 5. Cross-project impact and limits

A single changed shared `K` may affect multiple project-specific conclusions. Treat each dependency context separately; Project B's interpretation might remain valid despite Project A's changed definition. Explain every known impacted research project, affected draft or completed book sections, their status (`unaffected`, `reassessment pending`, `blocked`, `resolved`) and evidence basis. If indexes are incomplete or external copies cannot be reached, explicitly mark the propagation limit and escalation need; never claim exhaustive coverage.

Do not create a permanent background monitoring process. Only react when evidence is encountered during approved activity or separately authorized monitoring. Do not invent source notifications.

## 6. Durable propagation and recovery

Persist trigger evidence and original versions → dependency-impact/reopening records → changed review or claim states when justified → affected indexes/book revision entries/journal → validate links and dependent flags → checkpoint last. On interruption, preserve the previous completion dossier and pending flags; do not silently restore `complete` or clear flagged dependencies without reassessment. Recover via [consistency procedure](recovery-and-consistency.md).

**Exit condition:** All *known affected* dependencies receive an explicit, supportable disposition; requirements to authorize new work are identified; old completion and revision histories remain; any incomplete dependency coverage is disclosed rather than hidden.
