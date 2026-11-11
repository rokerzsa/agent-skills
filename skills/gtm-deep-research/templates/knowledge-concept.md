---
# TEMPLATE ONLY — frontmatter fields filled after a workspace-wide K-ID is durably issued
id: "{{K_ID}}"
title: "{{SEMANTIC_CONCEPT_TITLE}}"
status: "provisional"
origin_project: "{{PRJ_ID}}"
---

# {{SEMANTIC_CONCEPT_TITLE}}

> **TEMPLATE ONLY.** Create a separate concept only when semantically useful or reusable. An indexed concept is not automatically a verified fact. `K-...` is issued from the workspace counter, not the project-scoped ledger; `DR-...` design labels are never concept IDs.

[Knowledge index]({{KNOWLEDGE_INDEX_RELATIVE_LINK}}) · [Originating research project]({{PROJECT_INDEX_RELATIVE_LINK}})

## Scope and key definitions

{{TOPIC_DOMAIN_TIMEFRAME_GTM_TERMS_AND_BOUNDARIES}}

## Evidence-calibrated synthesis

{{WHAT_THE_EVIDENCE_CURRENTLY_ESTABLISHES_AND_WHAT_IS_REPORTED_ONLY}}

## Related claims, sources, contradictions

| Relation | Qualified ID | Meaning and evidentiary status |
|---|---|---|
| supports | `{{PRJ_ID}}:CLM-{{NNNN}}` | {{WHAT_IS_SUPPORTED}} |
| contradicts / qualifies | `{{PRJ_ID}}:CLM-{{NNNN}}` | {{WHAT_IS_DISPUTED}} |
| original source | `{{PRJ_ID}}:SRC-{{NNNN}}` | {{SOURCE_AND_LIMITATION}} |

## Competing explanations and unknowns

{{HYPOTHESES_ALTERNATIVES_FALSIFIERS_GAPS_AND_PENDING_REVIEWS}}

## Dependencies and reuse

{{OTHER_K_IDS_QUALIFIED_RECORDS_AND_PROJECT_DEPENDENCIES}}

## Review and lifecycle

**Evidence qualification:** {{CONFIDENCE_AND_RATIONALE}}  
**Review status:** `pending / not-required` (until a valid later review exists)  
**Record lifecycle:** `provisional / active / superseded`  
**Material revisions:** {{TRIGGERS_OLD_INTERPRETATION_AND_NEW_VERSION_REFERENCE}}

> **Concept-versus-book boundary:** This is a provisional semantic concept, not a reader-facing research chapter or separate source. It may be cited by a [draft book chapter](research-book-chapter.md) using its stable `K` identity. A major conclusion may reflect a genuine independent `RT` verdict, but neither the concept nor book publication makes the subphase/project complete.
