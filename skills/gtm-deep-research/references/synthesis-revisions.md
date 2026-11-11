# Selective synthesis revisions and durable history

[Book home](../book/index.md) · [Chapter 10](../book/part-04-outputs-lifecycle/10-research-synthesis-and-lessons.md) · [Revision template](../templates/synthesis-revision-log.md) · [OKF persistence](standalone-okf-conventions.md)

**Rule:** When evidence materially changes, revise only affected derived book sections while preserving sufficient history to reconstruct prior significant conclusions. Underlying evidence/claim/review records retain factual authority; an updated report version is not automatically more certain. Material changes may trigger [impact-based reopening](dependency-impact-and-reopening.md), subject to its objective threshold and authorization checks; a revision alone never implies completion or approval of new work.

## 1. Trigger classification

- **Editorial-only:** Spelling, formatting, clearer explanations, improved introductions and reordered sections within approved chapter scope, with the historical meaning and evidence qualifications preserved. Substantial narrative rewrites should retain a prior version and a concise editorial revision note; minor fixes need no heavy revision record.
- **Material evidence/interpretation change:** New direct source, contradiction, altered original-source lineage, confidence change, major red-team qualification, corrected GTM customer/timeframe definition, invalidated causal assumption. Requires a traceable revision entry and affected-section assessment.
- **Consequential structure/scope change:** Replacing top-level chapter organization or changing charter questions/central narrative beyond approved discretion requires the appropriate **human** authorization, even when evidence updates themselves are mandatory.

## 2. Revision protocol

1. **Persist upstream first:** Verify the source/claim/concept/`RT`/decision record changes and evidence rationale have been durably recorded in OKF. A revision log cannot create historical truth by itself.
2. **Identify dependence:** Find affected book passages, linked `K`/`CLM` conclusions, lesson recommendations, neighboring section summaries and known cross-project reuse; note incomplete dependency coverage openly.
3. **Assess impact:** Determine whether the old text is factually wrong, now too certain, under mandatory new red-team review, or only imprecisely worded. Mark *draft/revision-pending* as needed; never continue publishing an unqualified contradicted assertion.
4. **Check governance:** New investigation follows approved contracts/budgets. Material charter/top-level book changes need approval; do not interpret a revision as automatic permission to reopen completed subphases/projects or expand scope.
5. **Preserve former meaning:** In a [revision log](../templates/synthesis-revision-log.md), retain prior claim wording or a versioned artifact reference, relevant context, old confidence/review state, evidence trigger and reason. Full snapshots of every minor edit are unnecessary.
6. **Integrate and resynthesize:** Put new evidence in the historical stage or explanation it changes. Rebuild the affected section and its transitions when needed, consolidate duplicates, and remove superseded passages. Do not append a new source summary or repeat the same customer dispute merely because another source arrived. Preserve unaffected chapters and factual qualifications; use the narrative and evidence reviews in the synthesis procedure.
7. **Repair references:** Update navigation, inward/outward links, topic indexes and version pointers, validate essential IDs and links, then advance the project checkpoint **last**.
8. **Report consequences:** State what changed, which conclusions/lessons are now weaker or stronger, remaining uncertainty, pending red-team work, cross-project notices and any outstanding human decision.

## 3. Revision record minimal fields

| Field | Meaning |
|---|---|
| Local revision marker | Stable local anchor/entry ID in book revision ledger; **not** a new global allocator |
| Project/book/section | Stable project ID, book version and relative link/path |
| Trigger | Canonical changed `SRC`/`CLM`/`K`/`RT`/decision reference(s) |
| Prior interpretation | Retained wording or durable previous version location |
| Revised interpretation | New wording or linked updated section |
| Review impact | Prior/current evidence state, qualitative confidence and `RT` status |
| Approval boundary | Whether any charter/plan/top-level chapter change was approved or remains blocked |
| Dependency/limitations | Affected neighboring or cross-project conclusions, unknown propagation coverage |
| Validation | Link checks and checkpoint update state |

A local sequence or heading anchor is enough for a revision entry. Avoid inventing another workspace-wide ID namespace; if a true semantic concept is needed, issue a `K` using the approved allocator.

## 4. Example — hypothetical only

A draft paragraph says, "ExampleCo had 100 paying enterprise customers by Year N," based only on a founder recollection. A contemporary invoice ledger subsequently contradicts the definition of *paying*.

- Persist the new actual-access source and narrower revised `CLM` first.
- Record original wording and original `SRC` reliance; preserve what the founder said as a reported claim.
- Revise customer chronology and dependent sales/lesson sections, not unrelated market history.
- Mark a major aggregate growth conclusion `review: pending` when fresh independent challenge is required; do not invent a passed review.
- Document unresolved first-customer counts and their effect on charter criteria. Perform a separate [completion audit](completion-and-acceptance.md) when requirements are met; if the material-change threshold applies, follow [reopening](dependency-impact-and-reopening.md) without assuming new budget or scope authority.
