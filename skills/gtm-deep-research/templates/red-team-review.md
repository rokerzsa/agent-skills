# Independent red-team review — {{PRJ_ID}}:RT-{{NNNN}}

> **TEMPLATE ONLY.** The review ID must be durably issued through the project scoped ledger. Never mark `passed` just because this template exists or a reviewer rephrased the initial conclusion. The investigation must independently search for counterevidence and alternatives. [Procedure](../references/red-team-and-adjudication.md).

| Field | Required value |
|---|---|
| Qualified review ID | `{{PRJ_ID}}:RT-{{NNNN}}` |
| Target claims / aggregate concept | {{QUALIFIED_CLM_OR_K_IDS_AND_PRECISE_AGGREGATE}} |
| Linked charter and authorized contract | {{VERSION_AND_APPROVAL_REFERENCES}} |
| Review trigger and major classification | {{GOAL_CAUSAL_STRATEGIC_DEPENDENCY_OR_UNCERTAINTY_IMPACT}} |
| Review workflow | `proposed / investigating / adjudicating / completed / blocked` |
| Target claim review state | `pending` until justified final disposition |
| Review method / actual investigator | {{SAME_MODEL_SEPARATE_PASS_OR_GENUINELY_SEPARATE_RESEARCHER}} |
| Budget ledger / hard limit check | {{LEDGER_REFERENCE_AND_AUTHORIZATION}} |

## 1. Frozen original research case (before red-team investigation)

**Exact original conclusion and scope/timeframe:** {{TARGET_ASSERTION}}

**Original evidence state / confidence / review state:** {{SEPARATE_VALUES_WITH_RATIONALES}}

**Original supporting sources and originating information lineage:** {{SOURCE_IDS_AND_DIRECTNESS}}

**Original researcher's proposed causal mechanism and dependencies:** {{MODEL_AND_ASSUMPTIONS}}

## 2. Adversarial hypothesis and evidence search

**Strongest rival explanations:** {{ALTERNATIVE_MECHANISMS_AND_CONFOUNDERS}}

**Falsification questions:** {{EVIDENCE_THAT_COULD_REJECT_OR_NARROW_TARGET}}

| Independent avenue / query or method | Actually accessed evidence and `SRC` IDs | Counterfinding or negative result | Source lineage / access limits |
|---|---|---|---|
| {{DISTINCT_ADVERSARIAL_SEARCH}} | {{QUALIFIED_SOURCE_IDS_OR_NONE}} | {{WHAT_WAS_FOUND_OR_NOT}} | {{INDEPENDENCE_AND_ACCESS_MODE}} |

**Evidence not retrievable / attempts made:** {{BOUNDED_RECOVERY_AND_GAP_IDS}}

**Strongest challenge:** {{PRECISE_OBJECTION_AND_PROVENANCE}}

## 3. Researcher–red-team adjudication

| Disputed point | Original argument and evidence | Red-team counterargument and evidence | Disposition and reason |
|---|---|---|---|
| {{POINT}} | {{ORIGINAL_CLM_SRC_IDS}} | {{COUNTER_CLM_SRC_IDS}} | {{REASONED_COMPARISON}} |

**Additional bounded authorized investigation:** {{NEW_SOURCE_IDS_OR_NONE_AND_BUDGET_EFFECT}}

**Definitional/timeframe reconciliation:** {{WHAT_CHANGED_OR_NONE}}

**Residual consequential dispute:** {{UNCERTAINTY_OR_NONE}}

## 4. Final independent review disposition

**Claim review state:** `pending / passed / qualified / unresolved` — {{SELECT_ONLY_AFTER_SUBSTANTIVE_REVIEW}}

**Evidence state (separate):** `supported / disputed / unverified / refuted` — {{WITH_CITATIONS}}

**Qualitative confidence (separate):** `high / medium / low / unverified` — {{RATIONALE}}

**Revised exact conclusion, if qualified:** {{NARROWED_TARGET_OR_NOT_APPLICABLE}}

**Unresolved critical gaps / escalations / selectively paused dependencies:** {{GAP_IDS_AND_DECISIONS_OR_NONE}}

**Reasoning and source references for verdict:** {{CITATIONS_AND_WHY_ALTERNATIVES_WERE_ADDRESSED}}

**Review history / future revisit triggers:** {{VERSION_OR_NEW_EVIDENCE_TRIGGER}}

**Persist and checkpoint sequence:** Source/claim/review records → indexes/journal and dependencies → validate → active state. A red-team verdict alone never completes a subphase or project; apply the separate [completion criteria](../references/completion-and-acceptance.md).
