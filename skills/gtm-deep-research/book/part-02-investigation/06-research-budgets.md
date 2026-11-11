# Chapter 06 — Research Budgets

[Book home](../index.md) · [Part II](index.md) · [Previous: Chapter 05](05-independent-red-team-review.md) · [Next: Part III](../part-03-okf-architecture/index.md)

**Status:** Approved consolidated specification, operationally specified. **Governing decisions:** DR-028, DR-029, DR-030. See [budget-management procedure](../../references/research-budget-management.md) and [budget-ledger template](../../templates/research-budget-ledger.md).

**Purpose:** Allocate and track research effort and expenditure without mistaking resource use for evidentiary completion or granting Codex authority to exceed approved limits.

## 6.1 Adaptive budgets as authorization, not completion

Each project, phase or subphase may receive an initial effort budget with an explicit authorized extension allowance. Codex must monitor resource consumption, useful evidence gained and outstanding uncertainties. It may recommend an extension with a concrete rationale; no significant additional effort outside approved capacity may be silently authorized.

A budget is **not** evidence. An exhausted budget cannot close a critical gap, independently validate a conclusion, satisfy a red-team review, or mark a subphase complete. **Budget exhaustion is not evidence exhaustion.**

No numerical budget is required when none is assigned. Record only dimensions that are authorized and meaningful to track. Do not invent limits, cost or consumption for convenience.

## 6.2 Multidimensional units

| Optional dimension | Acceptable units and caveats |
|---|---|
| Source investigations | Count meaningful inspected sources, not discovered URLs |
| Investigation passes | Count distinct substantive research/review passes, including independent red-team passes |
| Exploration allowance | Number of approved adjacent investigation branches, tracked separately |
| Time | Measured clock or active time when observable; estimates explicitly labeled |
| Model tokens | Provider-reported usage when available, not invented counts |
| Money | Actual committed/paid expense by currency and approved category; no implicit paid access |

Each dimension has a separate authorization. Remaining allowance in one dimension does not permit exceeding another. Do not convert sources to arbitrary monetary equivalents or require mandatory numeric information-gain scoring.

## 6.3 Measurement integrity

Resource use must be classified as:

- **Measured:** Supported by observed counts, reliable time capture, provider usage or receipts; record source/basis.
- **Estimated:** Approximate with transparent method and limitations, never represented as actual expenditure.
- **Unavailable:** Reliability is insufficient to calculate usage; explicitly state unavailable rather than substituting zero.

The ledger must distinguish authorized, reserved, consumed, remaining and proposed allocations where those are meaningful. A source is counted as investigated only when actually examined to a material degree. Summaries or search snippets are not equivalent to examining an original.

## 6.4 Authorization hierarchy and single-count accounting

For project/phase/subphase budgets, the ledger must identify source decision records, versions, dimensions, base limits, extensions and applicable parent ceilings. Individual subphase reservations may not enlarge the project's approved total.

One consumption event should be charged once in the ledger and reflected consistently in all applicable scope totals. The system must not count the same event twice merely because it appears in both a phase and project report.

Before an operation, Codex must check **all** configured dimension ceilings and the strongest applicable limit, including direct paid charges. An unapproved charge is prohibited even if other research dimensions have remaining capacity.

## 6.5 Preauthorized extension allowance

A separately approved extension allowance is part of the existing total authorized capacity. Codex may autonomously **consume** it when a documented research benefit justifies doing so; it may not autonomously **increase** it.

Before drawing on the extension, document:

1. Approved original amount and extension allowance, with decision reference.
2. Consumption so far and the measured/estimated/unavailable status.
3. Remaining critical questions, new leads and evidence avenues.
4. Expected information gain and alternative outcomes.
5. Exact amount/dimension to draw and checks against all applicable parent/other-dimension ceilings.
6. Consequences of stopping now versus continuing.

An allowance to investigate additional sources is not permission to make a paid purchase. An estimated financial charge is not authorization to pay it.

## 6.6 Hard ceilings and unobservable usage (R-04)

If compliance with an authorized hard ceiling cannot be **reliably enforced**, Codex must not initiate an operation that risks exceeding it. It must request a verifiably bounded alternative or additional human authorization.

A token, time or cost estimate may guide planning, but does not prove that the remaining amount is safe. Where a provider supports a reliably enforceable cap, Codex may use that capability under the actual approval. No automated or speculative payment is permitted.

## 6.7 Adaptive reassessment

At meaningful resource checkpoints, compare what evidence has been obtained, what remains unknown, which source avenues appear promising, which competing models remain viable, and how likely additional authorized effort is to change the answer.

Possible decisions: prioritize higher-information avenues; continue within base; consume justified preauthorization; request new allocation; pause budget-dependent work; or close a **separately evidenced noncritical exhausted gap** under Chapter 03's protocol.

An information-gain justification should be qualitative, auditable and claim-specific. A numerical score is not required. Exhausting a quota is never a reason to upgrade confidence or close an investigation.

## 6.8 Ledger and audit fields

A logical budget record must preserve:

| Field | Requirement |
|---|---|
| Identity/scope | Project, phase/subphase, plan/contract references |
| Authorization | Actual human decision ID, version and effective constraints |
| Dimensions | Unit, base, extension, hard ceiling, paid-access limits |
| Consumption | Event-level usage and reliability status; actual vs estimate |
| Hierarchy | Allocation and non-duplicated rollups under all parent ceilings |
| Extension decisions | Expected information gain, lead, proposed draw, source of preauthorization |
| Amendments | Previous and revised authorization, reasons and human approval |
| Recovery | Interrupted usage reconciliation and stop conditions |

Budget changes that modify authorization must be durably recorded in the project `DEC` ledger; the budget ledger is not a competing approval registry. Save substantive decisions/usage, update journal/indexes, validate and checkpoint last.

## 6.9 Examples (illustrative only)

**Source count:** Initial 40 meaningful source investigations plus an approved +15 extension allow up to 55 under this dimension, subject to project-level limits and all other constraints. A 56th requires additional explicit approval.

**Paid archive:** A budget of 40 free sources does not authorize spending to open a paid archive. The payment must have its own actual approval and an enforceable cost limit.

**Unknown tokens:** If a hard token budget is configured but the environment cannot report or safely cap tokens, Codex must not assume the ceiling is being honored; seek a measurable alternative or an amended authorization.

**Conflicting allocations:** Two subphases with reserved 60-source allowances do not expand a 100-source parent ceiling to 120. Reconcile allocations before dispatch and report the real aggregate capacity.

## 6.10 Completion and later work boundary

Research budget reporting must be proportional: authorized versus used, measurement caveats, expected next evidence, critical open questions, proposed extensions and human decisions needed. A budget report is not an evidence assessment and not a project completion dossier.

**Current lifecycle rule:** Budget governance applies during investigation, book revisions, criterion-verified completion and reopening. It never authorizes new work or spending beyond the explicit limits. Refer to [completion](../../references/completion-and-acceptance.md) and [reopening](../../references/dependency-impact-and-reopening.md).

**Previous:** [Chapter 05 — Independent Red-Team Review](05-independent-red-team-review.md) · [Part II index](index.md).
