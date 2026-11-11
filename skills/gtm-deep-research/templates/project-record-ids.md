# Scoped Research Record IDs — {{PRJ_ID}}

> **Template only.** Counter values of zero are valid only before any allocation. Single-writer issuance; no recycling.

| Kind | Prefix | Last issued number |
|---|---|---:|
| Source | `SRC` | 0 |
| Claim | `CLM` | 0 |
| Research contract | `RC` | 0 |
| Red-team review | `RT` | 0 |
| Gap | `GAP` | 0 |
| Project decision | `DEC` | 0 |

**Qualified form:** `{{PRJ_ID}}:SRC-0001`. These IDs are not global concept IDs (`K-...`) or skill-design labels (`DR-...`).

Persist issuance before record creation. Gaps in numbering are acceptable; reused IDs are not.

**Operational rule:** Reopening/dependency records reference qualified existing IDs and may use local stable anchors, not a new global semantic-concept counter. If a record is treated as a separately scoped consequential decision, allocate its `DEC` ID using this existing ledger. Completion dossiers refer to `PRJ`, phase/subphase and versioned contracts rather than inventing a new global completion allocator.

**Operational rule:** `RT` is the existing review namespace: allocate durably before [independent red-team record](red-team-review.md) creation. Budget **events** use stable ledger-local event markers; no extra global or project-wide counter is required. Budget authorization decisions retain existing `DEC` IDs.
