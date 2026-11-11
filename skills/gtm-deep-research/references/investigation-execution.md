# Authorized research investigation — question-driven execution

[Book home](../book/index.md) · [Chapter 03](../book/part-02-investigation/03-research-contracts-and-investigation.md) · [Evidence protocol](source-and-claim-evidence.md) · [Gaps and journal](gaps-and-journal.md)

**Current capability:** Authorized question-driven investigation and durable source/claim/concept/gap/journal evidence integrate with **independent red-team/adjudication**, adaptive budgets, evidence-linked book synthesis/revisions, learning, and the **separate completion/reopening lifecycle procedures**. Investigation alone never pronounces a subphase complete; [completion](completion-and-acceptance.md) must independently verify the contract and mandatory reviews. Skill release remains separately human-gated.

## 1. Start gate: verify *all* authorizations

Before substantive investigation, verify against durable project records:

1. The standalone workspace exists at the user-approved root and has no unresolved inconsistent state; there is **no Goal Memory dependency**.
2. The project charter version and high-level phase plan have separate recorded human approvals.
3. The active immediate detailed plan and exact contract version have explicit coverage under recorded human approval (one combined detailed-plan/contract decision is permitted when both versions are named).
4. The contract's objective, boundaries, mandatory questions, dependencies, source methods, review triggers, completion criteria, and allowed discretionary exploration are consistent with those approvals.
5. Resource activities are within **measurably enforceable** authorized constraints. Use the [budget protocol](research-budget-management.md): check assigned dimensions, parent and subphase ceilings, measured/estimated/unavailable usage, and actual spending authorization. A **documented preauthorized extension draw** is allowed inside its original approved ceiling; exceeding the total or risking an unenforceable hard limit is not.
6. Scoped ID counters, indexes, current checkpoint, and pending recovery are consistent. Do not create or repair a shadow store.

If any precondition fails, record the actual blocker without implying authorization and **do not begin substantive investigation**. A research contract file does not by itself grant authority.

## 2. Decompose the approved subphase by *questions*, not URLs

- Assign local question labels from the approved contract (these are not new global concept IDs).
- For each question state what evidence would answer it, what would disconfirm current hypotheses, and what distinctions matter (e.g. first *user* vs first *paying organization* vs first *invoiced revenue*).
- Prioritize critical/dependent questions and high-information evidence avenues while honoring depth-first investigation.
- Maintain a live ledger of question status through the contract or journal, referencing durable claim, gap, and concept IDs rather than creating redundant knowledge files.
- A newly discovered adjacent topic can be noted as a lead. Pursue only within approved scope/discretion; material changes require approved charter/plan amendment.

### Example: an early-customer research question

**Question:** Which organizations were among the first ten paying customers, and when did they pay? **Evidence targets:** contemporaneous invoices/contracts if accessible, dated customer announcements, product/pricing archives, verifiable participant interviews, independent coverage. A customer logo is *not* proof of a paid contract; a founder recollection is evidence of a recollection, not necessarily proof of payment. If no direct evidence survives, record the narrower supported observation and the unresolved gap instead of filling a ranked list with guesses.

## 3. Investigation loop

For each meaningful lead:

1. **Discover** a candidate source and record its identity/lead as appropriate. Discovery alone does not mean inspected.
2. **Inspect** what is legitimately accessible; record publication/event dates separately, accessed form, precise supporting location, chain of attribution, and limitations. A snippet/secondary quotation must be labeled as such.
3. **Extract and qualify** distinct material claims; classify observation vs reported assertion vs causal hypothesis; link supporting/contradicting source IDs and source independence, qualitative confidence, evidence state, and separate review state.
4. **Challenge** emerging claims with alternative sources, explanations and disconfirmation avenues, including contemporary/archival evidence and contradictory accounts. Treat copies of one originating interview as one evidentiary lineage.
5. **Synthesize provisionally** into relevant reusable `K-...` OKF concepts, explicitly carrying unknowns, contradictions, confidence and pending reviews. Do not promote a hypothesis to fact because it is polished or indexed.
6. **Journal** meaningful work, failed avenues, hypothesis changes, gap assessments, source recovery and consequential decisions, by reference. Summarize repetitive low-value tool calls.
7. **Reassess** the active question and its dependencies. Continue a promising authorized lead, document a defensible noncritical exhausted gap, or escalate a critical/material issue. Only unaffected independent work may continue when dependencies are blocked.
8. **Persist in recoverable order** using the standalone OKF issuance and checkpoint-last protocol.

Do not wait until the final report to persist provisional evidence. Conversely, not every search result needs its own claim or source record: record materially relevant evidence with proportionate granularity.

## 4. Source discovery and recovery

Search primary, contemporaneous, retrospective, independent and contradictory material **according to what each can establish for the question**. Prefer strong claim-specific evidence, not a rigid universal ranking. Follow [source and claim evidence](source-and-claim-evidence.md).

When a crucial original is missing, make **bounded legitimate** recovery attempts through publicly accessible archives, original publishers, filings, authorized databases and independent corroboration. Document failures in the gap record and journal. Never bypass paywalls/access controls, claim an original was viewed when only a description was available, or invent a contract's content.

## 5. Critical findings and reviews

- Preserve important rival hypotheses and distinguish source claim from underlying historical fact.
- Detect possibly invalidated charter/plan assumptions; document precise impacts and selectively pause dependent work before requesting necessary amendment approval. Do not independently rewrite an approved objective.
- Identify **major conclusions**, including consequential aggregate causal/strategic models, by impact, dependencies and uncertainty. Mark review **pending** until an actual separate [independent red-team investigation](red-team-and-adjudication.md) with distinct evidence search and adjudication completes; never simulate a passed review. A completed review still does not authorize subphase closure.
- Normal investigation can continue for authorized independent questions; a blocked conclusion is not an excuse to discard other research.

## 6. Durable write sequence and ID use

Use [standalone OKF conventions](standalone-okf-conventions.md) and these [templates](../templates/source-register.md) / [claim register](../templates/claim-register.md) / [concept](../templates/knowledge-concept.md) / [gap register](../templates/gap-register.md) / [journal](../templates/investigation-journal.md).

- Validate the workspace single-writer assumption and counters; issue `SRC`, `CLM`, `GAP`, `RT` and `DEC` through the project's durable `record-ids.md`; issue concepts `K` only through workspace state. Persist issuance **before** using the ID; never reuse gaps.
- Append or revise substantial records; add stable qualified IDs within grouped registries. Record supersession or meaningful changes without quietly overwriting contrary earlier evidence.
- Update stable indexes, consequential dependencies and journal references; verify known links resolve; **checkpoint last**.
- On interrupted or ambiguous writes, halt new issuance, preserve good records and reconcile the counters, records and references before resuming.

## 7. Investigation handoff, not subphase closure

The investigation procedure may report **investigation and independent-review progress**: questions and evidence, actual red-team `RT` verdicts or pending status, competing interpretations, claim evidence and confidence, critical gaps, blocked dependencies, and measured/estimated/unavailable budget usage. It must **not by itself** issue final completion dossiers or certify the book; these follow separate chapter/book and completion audits.

**Do not infer a completion state from this handoff.** Use [synthesis and books](research-synthesis-and-lessons.md), optional [human learning](human-learning.md), [contract/charter completion](completion-and-acceptance.md) and [material reopening](dependency-impact-and-reopening.md) only through their separate rules. The approved contract's completion criteria remain intact, never waived.

## Review and budget integration

Before source acquisition, an independent red-team search, or a proposed exploration, inspect all applicable allocations using [research budget management](research-budget-management.md). Record new sources and counterclaims discovered by the red-team as ordinary honest provenance records; its [independent review](red-team-and-adjudication.md) must maintain a separate `RT` research pass and final disposition. Preserve a material unresolved dispute as `review=unresolved`, escalate and selectively pause dependent claims. Neither a completed review nor a budget report closes the subphase.
