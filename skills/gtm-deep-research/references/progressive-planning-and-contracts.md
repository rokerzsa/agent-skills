# Progressive research planning and contract preparation

[Book home](../book/index.md) · [Chapter 02](../book/part-01-foundations/02-governance-and-planning.md) · [Plan template](../templates/research-plan.md) · [Contract template](../templates/research-contract.md) · DR-003/006, DR-011/017/018, R-02

**Full assembled workflow:** Prepare/approve plans/contracts; execute authorized investigation; record sources, claims, concepts, gaps, journal, independent [red-team reviews](red-team-and-adjudication.md) and [budget usage](research-budget-management.md); **draft charter-scoped evidence-linked research books** and offer [adaptive learning](human-learning.md). Subsequent [contract/charter-verified completion](completion-and-acceptance.md) and [material-impact reopening](dependency-impact-and-reopening.md) are separate lifecycle gates; planning alone does not authorize either or bypass new budget/scope approvals.

## 1. Maintain distinct objects and approvals

| Object | Question it answers | Approval rule |
|---|---|---|
| Versioned research charter | What/why/boundaries/evidence/outputs/complete? | Explicit human approval first |
| High-level phase plan | Which major phases, order, dependencies and milestones? | Separate explicit human approval |
| Immediate detailed phase/subphase plan | What specific work is authorized next? | Explicit human approval before execution |
| Research contract (`RC-...`) | What are the exact executable questions/strategy/reviews/outputs/closure criteria? | Must fit the approved detailed plan; may be approved **together with that plan** when explicitly attached and identified |

A high-level plan need not detail every future subphase. A detailed plan is not automatically approved because the high-level outline was approved. A draft contract has `proposed` status until its execution authorization is verifiable.

## 2. Prepare a complete high-level phase outline

From the **approved** charter, propose coherent major phases, each with:

- Objective and mandatory question groups.
- Logical boundaries and dependencies.
- Expected evidence classes and broad investigation strategy.
- Proposed outputs and important reviews.
- Approximate effort/budget assignment where authorized or appropriate.
- Phase-specific uncertainty and potential change triggers.

Order phases depth-first where dependencies matter. A typical GTM study might start with market and inception, proceed through early adoption and first paying customers, then channels/pricing/sales, growth/competition, causal adjudication and synthesis. This is an example, not a universal GTM template. Only the **high-level outline** needs full upfront detail.

Present the outline and request explicit human approval **separately** from charter approval. Preserve approved version and decision reference before progressing.

## 3. Elaborate the immediate detailed phase or subphase

For the next authorized block of investigation, specify:

1. Exact objective and bounded scope.
2. Mandatory research questions and crucial definitions.
3. Already known dependencies and assumptions.
4. Source-discovery avenues and how findings could be corroborated/challenged.
5. Evidence expectations appropriate to each claim (avoid arbitrary source quotas).
6. Rival explanations, uncertainties and expected red-team triggers.
7. Resource allocation and available preauthorized extension allowance, **only if assigned**.
8. Required OKF records, concepts, journal entries and planned book contributions.
9. Completion tests and handling of material unresolved gaps.
10. Human review, stop/escalation points and contract identity.

Do not dictate every search query or presume exact future sources. A detailed plan should constrain outcomes and essential research method, leaving authorized tactical discretion.

## 4. Author the structured research contract

Create the contract from [the template](../templates/research-contract.md) with stable project-scoped `RC` ID (issued durably only in a ready workspace). The contract must identify the approved charter version, high-level plan, and immediate detailed plan plus evidence of their authorization.

Contract fields must include: identity, objective, scope/exclusions, mandatory questions, dependencies, investigative strategy, evidence/source expectations, alternative hypotheses, mandatory reviews, budget references, expected OKF outputs, completion conditions, and execution status.

Use explicit `not yet determined` values when research itself will resolve a detail; do not fabricate sources or review results. No fixed minimum source count substitutes for an evidence standard.

## 5. Authorization equivalence and material changes

One explicit human decision may approve **the immediately detailed plan together with its specifically attached contract**. This avoids a redundant contract-specific gate. The approval record must name both objects and versions, or otherwise unambiguously identify the contract being authorized. It does **not** replace the charter or high-level phase-plan approvals.

If the drafted contract includes a new consequential objective, method, resource risk, dependency or boundary beyond the approved detailed plan, stop and obtain the appropriate plan/charter amendment before making it executable.

Routine wording corrections and tactical search adjustments inside the approved scope do not require reapproval. Material scope, budget, central narrative or assumption changes do.

## 6. Depth-first progression and bounded discretion

At execution time under the authorized research protocol, Codex should investigate each active subphase to its approved depth before dependent work. Evidence exhaustion is separate from budget exhaustion. Investigation and justified noncritical gap closure do not themselves complete a subphase. Mandatory red-team review stays pending until a substantive independent pass finishes; closure follows a separate [completion audit](completion-and-acceptance.md).

Codex may identify possible adjacent leads while **planning** and document them as proposals or deferred leads. It must not investigate them substantively or expand the approved charter without human approval.

## 7. Invalidated assumptions at planning time

If reliable preliminary information contradicts an assumption supporting the approved plan:

1. Record the challenged assumption and what actually supports the contradiction (do not overclaim reconnaissance evidence).
2. Identify which proposed or approved work materially depends on it.
3. Suspend only affected dependent planning or execution requests.
4. Propose a charter or plan amendment with alternatives, scope/budget consequences and rationale.
5. Obtain explicit human approval where the change is consequential.
6. Continue unaffected authorized planning and preserve the revision history.

Never autonomously replace the goal based on one attractive new hypothesis. Independent red-team adjudication follows [review procedures](red-team-and-adjudication.md), and material new evidence may trigger [selective reopening](dependency-impact-and-reopening.md). Investigate and preserve provisional evidence under authorization; reopening does not authorize fresh scope or budget.

## 8. Durable status sequence

Use the existing [standalone OKF conventions](standalone-okf-conventions.md) and [approval protocol](activation-and-approval-gates.md):

1. Verify authorized workspace and counters; recover inconsistent state.
2. Persist proposals and exact version references without asserting approval.
3. On explicit approval, issue `DEC` IDs and persist actual decision evidence; update the approved version without deleting prior history.
4. For a new contract, durably issue `RC` ID before creating its content.
5. Persist approved charter/plan and attached contract, update references and indexes, validate, then checkpoint.
6. Mark next authorized action **“Verify investigation and budget start gates”**. Do not treat the plan as evidence of any source already inspected. After authorization and start-gate checks, actual evidence records can be added by [investigation execution](investigation-execution.md).

If steps cannot be safely persisted, halt dependent persistent work rather than inventing a second authority.

## 9. Planning deliverable and exit checklist

- [ ] Approved charter and its decision reference exist.
- [ ] Complete high-level outline, dependencies and plan approval exist.
- [ ] Immediate detailed plan is bounded and approved.
- [ ] Contract matches that detailed plan and includes all required fields.
- [ ] Combined plan/contract approval identifies both objects if used.
- [ ] Scope, budget, source standards and review triggers are explicit or properly deferred.
- [ ] Material assumption conflicts and proposed amendments remain visible.
- [ ] Durable IDs and references resolve; checkpoint is consistent.
- [ ] Do not claim that a planning artifact itself proves execution or source access; an authorized research block may be executed separately. Do not claim an unperformed red-team verdict or completed subphase.

**Proceed under the authorized research protocol start gate only.** Once the approved charter, high-level plan, exact detailed plan and contract authorization are durable, follow [authorized investigation](investigation-execution.md). Perform red-team adjudication and preauthorized budget draws only through their documented authorized procedures. Evidence-linked synthesis follows [book procedures](research-book-architecture.md), and subphase/project closure requires the independent [completion audit](completion-and-acceptance.md).
