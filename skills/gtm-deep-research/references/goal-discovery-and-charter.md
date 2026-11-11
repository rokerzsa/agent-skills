# Bounded reconnaissance, goal discovery and charter authoring

[Book home](../book/index.md) · [Chapter 01](../book/part-01-foundations/01-research-modes-and-charters.md) · [Charter template](../templates/research-charter.md) · DR-001/002, DR-007–010, DR-046/047

**Available under the authorized research protocol:** intake, clarification, charter drafting and explicit authorization; approved contracts may then be investigated through [authorized investigation](investigation-execution.md) and reviewed/budgeted using [red-team](red-team-and-adjudication.md) and [budget procedures](research-budget-management.md). Do not mistake reconnaissance for a fully researched finding.

## 1. Decide whether full research is warranted

Evaluate the number and interdependence of questions, source uncertainty, causal or strategic stakes, decision impact, and expected investigation effort. A quick fact lookup does not need a charter. If borderline, ask one brief question about intended research depth rather than pre-emptively initiating a multi-round discovery protocol.

## 2. Perform bounded preliminary reconnaissance

Reconnaissance exists to formulate **better questions**, not to answer every research question or deliver a preliminary GTM history. Before extensive human grilling, gather only enough background to establish:

- Names, period, product, audience and terminology likely to matter.
- Known distinctions such as users versus paying customers, revenue versus advertised pricing, product launch versus incorporation, and reported versus independently documented events.
- Obvious assumptions, disputes, source-access challenges and unknowns.
- Plausible research angles and questions for the human.

Honor active resource and access limits. Do not incur unapproved costs, bypass access controls, or imply that a snippet/retrospective account verifies the underlying historical event. Mark findings provisional and identify the sources actually inspected. If a durable workspace is not authorized or available, keep reconnaissance small and conversational; do not continue substantial stateful research without safe persistence.

**Reconnaissance output:** a short discovery brief with preliminary subject, important terminology, provisional knowledge, critical gaps, likely assumptions and proposed clarification questions. Avoid an invented factual chronology.

## 3. Complete the mandatory thirteen-dimension discovery matrix

Every full research charter must address each dimension. Gather information conversationally, adapting question order and grouping; do not insist on a giant form or ask everything at once. If a dimension does not apply, mark that explicitly with a reason rather than silently skipping it.

| # | Dimension | Key question | Charter placement |
|---:|---|---|---|
| 1 | Motivation | Why now? What prompted the research? | Rationale |
| 2 | Objectives | What understanding or decision must it enable? | Objectives |
| 3 | Existing knowledge | What is already known, believed or disputed? | Prior knowledge |
| 4 | Subject boundaries | Which entities, users, periods, regions, products and events? | Scope |
| 5 | Depth | How exhaustive, granular or causal must the inquiry be? | Depth |
| 6 | Critical questions | Which questions must be answered or responsibly bounded? | Mandatory questions |
| 7 | Assumptions | What provisional beliefs require tests or alternatives? | Assumptions |
| 8 | Evidence standards | Which kinds and quality of evidence can justify claims? | Evidence rules |
| 9 | Constraints | Budget, access, resources, legal/ethical limitations? | Constraints |
| 10 | Outputs | Book structure, evidence records, analysis, learner outputs? | Deliverables |
| 11 | Human involvement | What learning, review and escalation are desired? | Participation |
| 12 | Completion criteria | What objectively makes the research sufficiently finished? | Completion |
| 13 | Exclusions | Which tempting questions are explicitly out of scope? | Non-goals |

Do not treat the user's inability to answer a historical fact as a reason to stop intake: mark it as a research question. Do not assign an invented numerical budget when none was supplied.

## 4. Apply adaptive and rigorous goal-grilling

Challenge ambiguities that could affect the investigation:

- “First customer” may mean first registrant, activated user, first paying person, first signed contract, or first revenue collected. Ask which matters; if multiple matter, distinguish them.
- “What worked” may reflect an outcome without proving a causal contribution. Ask whether the objective is chronology, mechanism, or a decision-ready comparison.
- “First 100” may be unobservable in public evidence. Agree whether evidence-exhausted, explicitly qualified outcomes can count toward completion and which facts remain critical.
- Apparent success may reflect timing, selection bias, founder network, underlying market growth, funding or competitive changes. Propose alternative hypotheses rather than assuming an attractive success story.
- Company-wide and product-specific GTM may diverge. Confirm boundaries and units of analysis.

Ask targeted follow-up rounds until consequential ambiguities are resolved **or explicitly accepted as uncertainty**. Preserve human choice: Codex proposes alternatives and challenges weak assumptions; it does not dictate the desired conclusion.

## 5. Propose optional GTM-specific extensions

The thirteen-dimension core is mandatory. Codex may propose subject-specific discovery extensions, with a clear relevance and effort rationale, such as:

- Pre-inception market conditions and competitor alternatives.
- Founder distribution advantage, network and earliest audience.
- User → active user → paying customer conversion.
- First 1/10/100 paying customers (where supportable), deal dynamics and source access.
- Pricing, sales cycles, contracts, channel economics and revenue quality.
- Failed experiments, partnerships, pivots, retention, and growth constraints.
- Distinguishing temporally close evidence from founder retrospective stories.

Consequential additions to approved scope, depth or effort **require human approval**; no silent expansion of the discovery framework. This is a GTM skill, but not every project needs every extension.

## 6. Draft the charter

Use [the research-charter template](../templates/research-charter.md). State objectives, questions, scope, evidence standards, assumptions, outputs, constraints, human participation, exclusions and completion criteria. Keep confidence in the *plan* separate from confidence in *historical claims*. Distinguish:

- **Approved requirements:** what the human authorized.
- **Research questions:** what Codex must try to establish.
- **Provisional hypotheses:** not yet established facts.
- **Unknowns / accepted limitations:** unresolved issues with explicit handling.
- **Proposals:** extensions or changes not yet approved.

The charter is a versioned governance artifact. Material amendments must identify what changed, consequences for plans/budgets/dependencies, and the actual human approval. Do not silently overwrite the previous approved version or mark a proposed version as current.

## 7. Obtain and persist charter approval

Present the complete charter in human-readable form, summarize consequential choices, identify open issues, and ask explicit approval of its version. Goal/charter approval **does not** approve the high-level plan or immediate detailed plan.

In an approved, ready OKF workspace, issue an unused `DEC` ID, persist actual authorization evidence in `decisions.md`, and link the approved charter version. Follow durable write ordering and checkpoint-last rules. If there is no authorized persistent workspace, do not assert approval has been durably recorded; an approval can be discussed in conversation but the prerequisite record must be reconciled before dependent writes/execution.

## 8. Charter acceptance checklist

- [ ] Research request classified appropriately and reconnaissance bounded.
- [ ] All 13 discovery dimensions addressed or explicitly marked not applicable.
- [ ] Important GTM units/definitions distinguished where necessary.
- [ ] Consequential ambiguities challenged, resolved or accepted as uncertainty.
- [ ] Extensions justified and approved when material.
- [ ] Charter separates factual assertions from questions and hypotheses.
- [ ] Evidence expectations are claim-specific and uncertainty-aware.
- [ ] Constraints, outputs, approvals and objective completion criteria are stated.
- [ ] Explicit human decision identifies the approved charter version.
- [ ] Durable decision recorded in a ready, authorized OKF workspace before dependent stateful work.

**Next:** [Progressive planning and research contracts](progressive-planning-and-contracts.md), then [authorized evidence investigation](investigation-execution.md) only when every start gate is satisfied. Actual major-conclusion red-team outcomes may be recorded under [independent review](red-team-and-adjudication.md). Research closure requires the separate [completion audit](completion-and-acceptance.md).
