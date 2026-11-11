> **Consolidated-run rule:** This is an internal stage assessment under the existing execution agreement, not a fresh human approval gate. Investigated unknowns follow the agreed disposition policy; missing required work still blocks readiness. Final delivery stops for user review.

# Subphase Completion Dossier — {{PRJ_ID}} / {{SUBPHASE_ID}}

> **TEMPLATE — NOT COMPLETION.** Use only with an authorized initialized workspace and actual persisted evidence. Follow [completion protocol](../references/completion-and-acceptance.md). A draft or unchecked dossier cannot close a subphase.

| Field | Evidence-backed entry |
|---|---|
| Project and subphase | `{{PRJ_ID}}` / `{{SUBPHASE_ID}}` |
| Contract / version | `{{QUALIFIED_RC_ID}}` / `{{VERSION}}` |
| Charter and plan versions | `{{CHARTER_VERSION}}` / `{{HIGH_LEVEL_PLAN}}` / `{{DETAILED_PLAN}}` |
| Actual approval decisions | `{{PRJ_ID}}:DEC-____` / `{{AUTHORIZATION_REFERENCE}}` |
| Outcome | `draft` until validated; then `complete`, `complete with qualifications`, or `blocked/incomplete` |
| Completion basis | `{{REASONED_CONTRACT_VERDICT}}` |
| Dossier revision / prior version | `{{REVISION_OR_NONE}}` |

## Mandatory question-by-question contract audit

| Contract question / criterion | Outcome (`answered/qualified/unresolved`) | `K` / `CLM` / `SRC` refs | Evidence/confidence and counterevidence | Criterion satisfied? |
|---|---|---|---|---|
| `{{Q_ID}}` | `{{ACTUAL_OUTCOME}}` | `{{REAL_REFS}}` | `{{RATIONALE}}` | `pending` |

## Mandatory independent red-team and adjudication

| Major/aggregate conclusion | `RT` ID / verdict | Adjudication and competing models | Pending consequential dispute? |
|---|---|---|---|
| `{{CONCLUSION}}` | `{{PRJ_ID}}:RT-____` | `{{ACTUAL_REVIEW_AND_EVIDENCE}}` | `{{YES_NO_WITH_RATIONALE}}` |

## Gaps, dependencies and limitations

- Noncritical evidence-exhausted gaps and searched avenues: `{{REFERENCES_OR_NONE}}`
- Critical gaps / disposition / actual escalation decisions: `{{REFERENCES_OR_NONE}}`
- Material dependency status, affected downstream work, revisit triggers: `{{REFERENCES_OR_NONE}}`
- Qualitative confidence and meaningful unresolved alternatives: `{{RATIONALIZED_SUMMARY}}`

## Outputs, book and resources

- Updated provenance, claims, concepts and journals: `{{REAL_STABLE_REFERENCES}}`
- Book sections or synthesis contributions: `{{REAL_LINKS_OR_NONE}}`
- Authorized budget, measured/estimated/unavailable usage, extension decisions and hard limits: `{{BUDGET_LEDGER_LINK_AND_BASIS}}`

## Objective closure checklist

- [ ] Each mandatory contract criterion addressed, including permissible qualified outcomes.
- [ ] Actual charter/plan/contract approval and versions verified.
- [ ] Material source/claim/counterevidence and confidence references validated.
- [ ] All mandatory individual/aggregate `RT` reviews and adjudication disposition verified.
- [ ] No unresolved critical blocker prevents closure; qualifications are charter-permitted.
- [ ] Downstream dependencies and relevant OKF outputs updated.
- [ ] Budgets and authorization constraints reconciled; no pending recovery.
- [ ] Dossier stored durably; indexes/journal validated; **checkpoint advanced last**.

**Final disposition and rationale:** `{{DO_NOT_MARK_COMPLETE_UNTIL_CHECKED}}`  
**Recorded by / context:** `{{ACTUAL_EXECUTION_CONTEXT_NOT_FABRICATED}}`  
**Outstanding authorizations or next planned action:** `{{ACTUAL_NEXT_STEP}}`
