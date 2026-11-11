# Adaptive multidimensional research budgets

[Book home](../book/index.md) · [Chapter 06](../book/part-02-investigation/06-research-budgets.md) · [Approval gates](activation-and-approval-gates.md) · [Ledger template](../templates/research-budget-ledger.md)

**Principle:** Budget is an **authorization and effort-management instrument**, never a proxy for evidence quality, completed red-team, or evidence exhaustion. Only configured/measurably meaningful dimensions need tracking; do not fabricate costs, usage or limits.

## 1. Establish authorization before an investigation

For each project/phase/subphase as applicable, record: scope, human approval/decision reference and version, measurement unit, base allocation, optional **explicitly preauthorized extension**, hard ceiling, already consumed amount, method/quality of measurement, and whether it is paid. Proposed numbers are **not** granted permission. When no dimension is configured, record `not assigned`; the absence of a price budget never permits spending.

Supported optional dimensions: meaningful source investigations (inspected, not merely listed URLs); substantial research passes; exploratory branches; active/elapsed time (say which); model tokens (only provider-reported measured values where exposed); money (actual authorized expenditure/currency). A project may assign additional dimensions with reviewable units. Avoid dollar-equivalent conversions or mandatory numeric information-gain scores.

Track parent/child allocations and actual consumption in one logical ledger: allocations earmark capacity **within** parent ceilings; **do not double count** the same consumption at a project, phase and subphase. Child approval does not increase the parent ceiling. For each dimension, enforce the most restrictive applicable authorized ceiling.

## 2. Measure, estimate or declare unavailable

| Usage status | Rule |
|---|---|
| `measured` | Backed by a real counter, provider report, expense receipt or observed investigation ledger; cite the measurement basis. |
| `estimated` | Approximate with basis, uncertainty and date/range when appropriate; never call actual or audit-grade. |
| `unavailable` | Environment cannot reliably observe usage; say unavailable, do not invent a number. |

Source investigations and passes may be reliably counted from documented actions; tokens, time, or cost may be inaccessible. `0` may only be reported when verified, not as a substitute for missing usage. Unknown consumption is not "remaining budget".

## 3. Before each resource-consuming action

1. Verify contract/detailed-plan scope, project/phase/subphase approval references and ledger consistency; recover interrupted writes first.
2. Identify **all affected dimensions**, including exploration allowance, paid access and the applicable parent ceilings.
3. Determine a defensible maximum prospective charge/usage. If a hard ceiling cannot be safely enforced because measurement or upper bound is unavailable, **do not run** the potentially exceeding operation; use a measurable lower-risk option or seek approval. Even an estimate does not authorize expenditure.
4. If within **remaining base**, proceed under existing permissions and log actual usage afterward.
5. If base would be exceeded but a suitable **preauthorized extension allowance** exists, record an **information-gain justification** and the amount to draw *before* use, check all other dimensions/ceilings, then execute. This is autonomous *consumption* of granted capacity, not autonomous budget expansion.
6. If authorized total would be exceeded, or activity introduces a new paid commitment or hard-limit uncertainty, **stop affected work and request explicit human approval**. Do not quietly transfer allowance between dimensions or contracts.

Previously granted extensions require evidence of the explicit authorization and must not be retroactively added by Codex. If an authorized monetary ceiling is enforced externally, record the mechanism; otherwise use a safer authorized method. Reserve/estimate worst-case cost when necessary, then reconcile against measured actual consumption. Do not overspend on the assumption that a later refund/reconciliation will fix it.

## 4. Adaptive reassessment and extension rationale

When approaching a limit, compare useful evidence obtained, still-critical uncertainties, independent corroboration opportunities, rival hypotheses, likely next information gain and effort. Options: reprioritize; consume justified preauthorization; seek a revised ceiling/charter; pause budget-dependent work; or record truly evidence-exhausted **noncritical** gaps under the independent gap rule.

A valid extension justification includes: current allocation/consumption with status, exact lead and question, evidence already searched, expected discriminating value, proposed additional units, project/phase ceiling checks, stop consequence, and approving decision or preauthorization reference. If a hypothesis has poor expected gain, do not spend just to use the allocation. **No hard rule to keep searching until quota is reached.**

## 5. Multi-level ceiling and mixed-dimension examples

- A subphase is allocated 40 source investigations plus **preauthorized** 15; autonomous justification can authorize use of investigations 41–55 *within* any project/phase caps. Source 56 requires a new human approval even if a different allowance remains.
- A monetary limit of ₹1,000 is independent of a source limit: five free-source slots remaining do not authorize a paid archive purchase.
- If the provider does not expose token usage and a hard token cap is configured, do **not** guess at the exact remaining tokens and risk crossing it; use a reliably capped method or ask for a different limit/approval.
- If a project has a 100-source ceiling and two subphases have 60 each reserved, their 120 total proposed allocations **do not** increase project authority above 100; reconcile reservations before dispatch.

## 6. Persist consumption and decisions

Use [budget ledger template](../templates/research-budget-ledger.md). Resource events must retain source/pass identifiers as appropriate, measurement status, actual or estimated amount (not invented), basis, linked contract, charged parent hierarchy, before/after authorized capacity, original approval and extension justification. Link meaningful budget decisions to the existing scoped `DEC` ledger; do not create a competing approval system or new global allocator. An authorization amendment requires explicit human decision and preserved prior version.

Persist budget events/approval records and dependent indexes/journal before advancing the project's active state. After interruption reconcile reservations, issued records and measured consumption; if indeterminate, halt affected usage. Consult [standalone OKF](standalone-okf-conventions.md) for single-writer and recovery requirements.

## 7. Escalation and stop conditions

When further important work exceeds authorization, report remaining uncertainty, value of extra research, dimension/units, remaining measured/estimated budget, review/critical gap impact, and next needed human decision. **Budget exhaustion cannot complete a question, red-team review, subphase or project**. Unresolved critical gaps remain critical; only unaffected work may continue.

**Lifecycle boundary:** Budget and red-team procedures apply throughout investigation, research-book revisions, [autonomous criterion-based completion](completion-and-acceptance.md) and [selective reopening](dependency-impact-and-reopening.md). Reopening does not grant extra budget. **Skill installation/release still requires separate human approval.** New investigation or paid source access prompted by a synthesis gap must respect the same ceilings.
