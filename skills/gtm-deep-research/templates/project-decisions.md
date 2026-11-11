# Project Decisions — {{PRJ_ID}}

> **Template only.** A proposal does not constitute approval. Record actual human authorization before gated actions.

## Required entry fields

- **Decision ID:** `{{PRJ_ID}}:DEC-0001` (issue through scoped ledger)
- **Subject:** `{{PROPOSAL}}`
- **Affected scope:** `{{CHARTER_VERSION_OR_PLAN_OR_BUDGET}}`
- **Status:** `proposed` / `approved` / `rejected` / `amended` (choose only with actual evidence)
- **Human decision statement:** `{{EXACT_OR_FAITHFUL_DECISION}}`
- **Authorization reference:** `{{TRACEABLE_USER_APPROVAL_POINTER}}`
- **Reasoning and impact:** `{{SUMMARY}}`
- **Consequential revisions:** `{{LINKS_OR_NONE}}`

Never manufacture a timestamp or approval attribution absent from the available record. Preserve previous decisions when amended.

**Operational rule:** For budget amendments, distinguish an existing **preauthorized allowance** (with original decision reference) from a proposed **new increase**. Usage/draw events belong to the budget ledger, while human authorization remains in this `DEC` ledger. Do not infer paid authorization from a source-investigation quota.
