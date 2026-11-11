# Claim and evidence register — {{PRJ_ID}}

> **TEMPLATE ONLY.** Populate from actually inspected/accurately represented evidence after durable scoped `CLM` allocation. One registry can hold many material claims; preserve stable qualified IDs across splits. Recording is not accepting or approving a claim.

[Project index]({{PROJECT_INDEX_RELATIVE_LINK}})

## Registry lookup

| Canonical claim ID | Current record location | Evidence state | Confidence | Review state | Material dependencies |
|---|---|---|---|---|---|
| `{{PRJ_ID}}:CLM-{{NNNN}}` | {{LOCATION}} | `unverified` | `unverified` | `not-required / pending` | {{REFERENCES_OR_NONE}} |

## Claim record — {{PRJ_ID}}:CLM-{{NNNN}}

**Canonical ID:** `{{PRJ_ID}}:CLM-{{NNNN}}`  
**Record version / supersession:** {{VERSION_AND_HISTORY}}  
**Exact assertion:** {{SPECIFIC_TIME_BOUND_ASSERTION}}  
**Subject / period / GTM definition:** {{BOUNDARIES_EG_SIGNED_VS_PAID_CUSTOMER}}  
**Assertion kind:** `observation / reported-assertion / historical-proposition / interpretation / causal-hypothesis`  
**Relevant contract question(s):** {{QUESTION_IDS}}  
**Evidence state:** `supported / disputed / unverified / refuted` — {{STATE_RATIONALE}}  
**Qualitative confidence:** `high / medium / low / unverified` — {{CONFIDENCE_RATIONALE}}  
**Independent review state:** `not-required / pending / passed / qualified / unresolved` — {{QUALIFIED_RT_ID_AND_DISPOSITION_RATIONALE_IF_EXISTS}}  
**Major-conclusion trigger/classification:** {{CAUSAL_STRATEGIC_AGGREGATE_DEPENDENCY_IMPACT_OR_NOT_REQUIRED_RATIONALE}}
**Independent red-team record:** {{PRJ_ID}}:RT-{{NNNN}} / {{NOT_REQUIRED_WITH_RATIONALE_OR_PENDING}}
**Adjudication and material review revisions:** {{ORIGINAL_VS_COUNTER_POSITIONS_VERDICT_REFERENCES_AND_HISTORY}}  
**Lifecycle status:** `active / superseded / retained-historical`  
**Dependencies / related concepts:** {{QUALIFIED_IDS_OR_NONE}}

### Supporting evidence

| Source ID | Access mode | What it legitimately supports | Original information lineage | Locator |
|---|---|---|---|---|
| `{{PRJ_ID}}:SRC-{{NNNN}}` | {{DIRECT_PARTIAL_SNIPPET_SECONDARY}} | {{NARROW_SUPPORT}} | {{SHARED_ORIGIN_OR_INDEPENDENT_RATIONALE}} | {{ACTUAL_SECTION_OR_PAGE}} |

### Contradicting or qualifying evidence

| Source ID | What it contradicts/qualifies | Reliability and independence |
|---|---|---|
| `{{PRJ_ID}}:SRC-{{NNNN}}` | {{COUNTEREVIDENCE}} | {{EVALUATION}} |

### Alternatives, tests and limitations

**Rival explanations:** {{ALTERNATIVES_OR_NOT_APPLICABLE}}  
**Potential falsifiers:** {{WHAT_NEW_EVIDENCE_WOULD_CHANGE_ASSESSMENT}}  
**Unresolved gaps:** {{GAP_IDS_OR_NONE}}  
**Original statement versus historical truth:** {{IF_REPORTED_CLAIM_EXPLAIN_NARROWER_VERIFIED_FACT}}

### Review and amendment history

{{STATE_CHANGE_DATE_IF_KNOWN_TRIGGER_SOURCE_AND_REASON}}

> **Major-conclusion review gate:** A major conclusion starts `pending`. It can become `passed` or `qualified` only after a separate evidence-seeking [independent red-team investigation](../references/red-team-and-adjudication.md) with a stable `RT` record, or `unresolved` after bounded adjudication. Review state is separate from evidence state and confidence. **None of these review outcomes completes a subphase/project.**
