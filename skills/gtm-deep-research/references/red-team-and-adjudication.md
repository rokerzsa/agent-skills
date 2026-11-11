# Independent red-team investigation and adjudication

[Book home](../book/index.md) · [Chapter 05](../book/part-02-investigation/05-independent-red-team-review.md) · [Evidence protocol](source-and-claim-evidence.md) · [Budget protocol](research-budget-management.md)

**Capability:** Perform a distinct, evidence-seeking adversarial investigation for each **major conclusion**, document the challenge under stable `PRJ:RT` identity, adjudicate within authorization and budgets, and preserve qualified or unresolved outcomes. **Not by itself a subphase/project completion authority**; a separate [contract/charter completion audit](completion-and-acceptance.md) is required. Neither a polished narrative nor human endorsement establishes historical truth.

## 1. Major-conclusion triage before relying on a synthesis

For each candidate conclusion (including one composed of individually small claims), record whether review is mandatory and why. Evaluate **impact**, not source count: charter significance, causal/strategic consequences, dependency centrality, uncertainty/contradictions, potential to change the interpretation, and cost of a mistaken conclusion. Important causal and strategic explanations are presumptive review candidates. A set of minor claims cannot avoid a required review by decomposition.

- **Major:** Create/issue project-scoped `RT` ID through `record-ids.md`; link the conclusion's exact `CLM`/`K` references; set the claim's **review state `pending`** until the review concludes.
- **Not major:** Record a concise *not-required rationale* for material interpretations; do not invent a completed review. Reassess classification if downstream use makes the conclusion consequential.
- **Unclear:** Treat the consequential use as pending and investigate the classification rather than silently exempting it.
- **Cross-project reuse:** A passed review in an earlier project is not a blanket substitute for review of a materially stronger or different conclusion in this project.

## 2. Separate adversarial research pass — substantive independence

The red-team pass is a **new investigation**, not an editing/criticism prompt. A separate model is optional; even in one model/session, separate the original researcher case from the adversarial work and **perform distinct source discovery**.

1. Freeze the **target wording, scope, timeframe, original supporting source/claim IDs, initial confidence and review state** in the `RT` record before looking for rebuttals. This preserves the initial case and avoids hindsight rewriting.
2. Form explicit counterhypotheses and falsification questions **without assuming the original explanation is true**. For GTM: demand vs distribution vs product/market timing; paying customer vs user/customer logo; list pricing vs realized revenue; selection and survivorship bias.
3. Independently search the authorized evidence space for **disconfirming contemporary/primary records, independent accounts, archival variants, disinterested witnesses and confounding mechanisms**. Record attempted avenues, new `SRC` IDs, actual access modes, failures and shared information lineages. Reusing the same sources is permitted *only if the search for alternatives is independently documented*; a simple summary of the original source list is insufficient.
4. Assess each contradiction and competing explanation against the original exact proposition. Preserve the strongest objection, its evidence, source quality and independence, and what observation would resolve it.
5. Issue a challenge report: what holds, what may be overstated, what remains unknown and the preliminary verdict. Distinguish a verified *statement about an event* from proof of the event itself.
6. Persist source/claim updates and the `RT` review record in the ordered OKF write protocol; link review IDs to target claims/concepts and journal; checkpoint **last**.

A review lacking real disconfirmation *attempts*, distinct source discovery, or alternative-model examination must remain **`pending`** (not `passed`). Never pretend a separate agent or tool ran if it did not.

## 3. Adjudicate original and red-team positions

When the challenge finds a consequential issue, conduct a **bounded, evidence-based adjudication** rather than a forced consensus:

- Compare exact wording, time period and definitions; investigate whether disagreement is terminological or substantive.
- Compare access form, dates, independence, directness, incentives, and what each source **actually** establishes.
- Investigate missing, potentially decisive sources or alternative causal mechanisms *only under the approved contract, limits and budget ledger*.
- Revise the claim's evidentiary confidence/state **only when evidence warrants**; keep procedural review state independent. A `passed` review does not mechanically upgrade confidence.
- If a material dispute remains, document opposing interpretations and why evidence cannot adjudicate. Flag affected dependencies and selectively pause work relying on the conclusion if needed.
- If adjudication would change charter scope, plan, or exceed a resource ceiling, propose the consequential amendment and request human approval **before** dependent investigation.

## 4. Verdicts and permitted transitions

Use existing claim **review states**: `not-required`, `pending`, `passed`, `qualified`, `unresolved`. Red-team working records may have workflow progress such as `in-progress` or `adjudicating` separately, but these are **not** claim review states.

| Claim review state | Required basis |
|---|---|
| `pending` | Review required, absent, incomplete or lacking independent investigation. |
| `passed` | A distinct completed adversarial pass found no *material unresolved challenge* to the **exact, limited conclusion**; evidence confidence is assessed independently. |
| `qualified` | Review completed and outcome narrowed/conditioned by significant limitations; revised target proposition and qualifications recorded. |
| `unresolved` | Consequential competing positions remain after bounded adjudication; preserve both, escalate and block dependent completion where required. |
| `not-required` | Impact-based non-major classification with reviewable rationale; revisit on material downstream use. |

Do **not** use `refuted` as a review state: it is an **evidence state**. If evidence refutes a claim, change the evidence state with citation/rationale and preserve the review outcome separately. Review records must retain original claim, independent challenge, adjudication, final disposition, citations, confidence effect, reviewers/method honestly represented, and relevant history. If new evidence later materially undermines a `passed`/`qualified` review, flag the earlier verdict stale and set affected conclusions **`pending`**, without erasing prior `RT` history.

## 5. Critical escalation and completion boundary

Escalate consequential unresolved disputes and missing decisive evidence with: question, original and counterpositions, independent evidence reviewed, gap/assumption effects, bounded avenues tried, costs/limits, proposed next authorization and impacted work. Do not downgrade criticality to close; no human approval creates fact certainty.

Even after a `passed` or `qualified` review, **this red-team procedure does not itself close a subphase/project or certify a final book**. The separate [completion procedure](completion-and-acceptance.md) verifies current contract/charter conditions, gaps, mandatory reviews and deliverables. New material counterevidence may trigger [selective reopening](dependency-impact-and-reopening.md) only after impact assessment and with previous dossiers preserved. Routine authorized investigation may continue while unrelated dependencies remain unblocked.

## 6. Review record linkage and durability

Issue `RT` ID durably, e.g. `PRJ-0001:RT-0001`, through the existing project scoped ledger **before** creating the record. Use the [red-team review template](../templates/red-team-review.md). A single `RT` may cover a clearly defined aggregate conclusion and referenced component claims; avoid per-trivial-claim paperwork.

Record new independent sources in [source register](../templates/source-register.md), changes in [claim register](../templates/claim-register.md), and meaningful work in the [journal](../templates/investigation-journal.md). Ensure source access and information origin are real, review records can be found via stable ID, references resolve, and the active checkpoint advances only after validation. Failure/recovery follows [standalone OKF conventions](standalone-okf-conventions.md).

**Exit checklist:** target frozen; classification justified; genuinely separate counter-search documented; alternative models/falsifiers tested; counterevidence assessed; bounded adjudication and budget checks recorded; review disposition justified; target claim evidence/confidence/review independently updated; affected dependencies/escalation preserved; no false subphase closure.
