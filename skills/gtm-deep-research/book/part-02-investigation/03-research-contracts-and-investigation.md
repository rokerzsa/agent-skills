# Chapter 03 — Research Contracts and Investigation

[Previous: Chapter 02](../part-01-foundations/02-governance-and-planning.md) · [Part II](index.md) · [Book home](../index.md) · [Next: Chapter 04](04-evidence-and-source-integrity.md)

**Purpose:** Establish a rigorous, auditable method of executing authorized subphase research and managing material evidence gaps without mistaking search activity or budget exhaustion for actual understanding.

**Governing decisions:** DR-012, DR-013, DR-018, DR-023.  
**Implementation status:** Authorized investigation, gap/journal recording, independent [red-team review](05-independent-red-team-review.md) and [adaptive budgets](06-research-budgets.md) are operationally specified. Autonomous subphase/project closure is a **separate verified procedure** under [Chapter 13](../part-04-outputs-lifecycle/13-completion-and-acceptance.md), not an automatic result of investigation.  
**Operational references:** [Investigation execution](../../references/investigation-execution.md) · [Gaps and journal](../../references/gaps-and-journal.md) · [Contracts and planning](../../references/progressive-planning-and-contracts.md).

## 3.1 Research contract as the execution boundary

Every executable subphase must have a versioned, structured research contract derived from an approved charter and plan. A contract makes the immediate investigation's scope and success requirements explicit. It must not silently add objectives, costs, evidence avenues outside authorization, or reinterpret plan approval.

Its required fields are:

| Field | Requirement |
|---|---|
| Identity | Stable scoped `RC` ID, version and title |
| Authorization | Actual approved charter, high-level plan and detailed-plan references; exact attached contract approval where applicable |
| Objective and scope | Specific question, subject/time bounds, inclusions and exclusions |
| Mandatory questions | Identifiable questions with evidence-based acceptable outcomes and priorities |
| Dependencies and assumptions | Prior work and assumptions whose invalidation affects this investigation |
| Investigation strategy | Claim-specific source avenues, approaches and falsification possibilities |
| Evidence expectations | Provenance, independence, corroboration and known access limits |
| Review expectations | Major-conclusion red-team triggers and consequential escalations |
| Resource authorization | Budget references, allowed discretion, hard ceilings and extension allowances |
| Required OKF outputs | Sources, claims, concepts, journal, gap records and other contract deliverables |
| Completion criteria | Objective research adequacy, permitted qualified gaps, critical blockers |
| Execution state | Current status, dependencies, next authorized action, revisions |

The authorized immediate detailed plan must **explicitly cover** the contract. One human decision may approve that plan with its named attached contract, but charter and high-level plan approvals are separate. Mere existence of a template or a `status: proposed` field authorizes nothing.

See the [research contract template](../../templates/research-contract.md) and [approval rules](../../references/activation-and-approval-gates.md).

## 3.2 Question-driven investigation

Codex must investigate **research questions and what would count as evidence**—not simply accumulate URLs. For each material question, it should:

1. Specify the possible defensible answer and relevant GTM definitions.
2. Identify observations, reported assertions and rival hypotheses that bear on the question.
3. Find and inspect accessible primary, contemporary, retrospective, independent and contradictory material as appropriate.
4. Evaluate what each inspected source actually establishes, not what its title suggests.
5. Link support and counterevidence to narrow claim records; assess independence and confidence.
6. Update provisional concepts and record meaningful actions, uncertainties and unresolved gaps.
7. Reconsider expected information gain and remaining leads within authorized resources.
8. Continue, close a defensibly exhausted **noncritical gap**, or escalate a critical/material issue.

Adaptive methods are allowed within approved scope. Material changes to objectives, approaches, spending or plan dependencies require corresponding human approval.

**Illustration:** To research a company's first ten *paying* enterprise customers, first define paid (signed contract? invoiced? cash collected?), period and organization-level identity. An archived pricing page establishes advertised pricing, not actual transaction values; a logo or founder interview may provide a lead, but does not necessarily establish payment. The narrowest supported claim is preferable to fabricated completeness.

## 3.3 Depth-first execution and limited parallelism

Codex should investigate an active subphase deeply before moving to dependent subphases, including consequential contradictions, alternative explanations, archived material and gaps.

Depth-first work does not prohibit parallel source searches that assist the **same** authorized subphase. It also does not demand infinite search: evidence exhaustion and justified qualified outcomes are possible.

No arbitrary mandatory source count substitutes for adequacy. A research question requiring one authenticated contract and one requiring multiple competing causal analyses need different evidence approaches.

## 3.4 Evidence exhaustion

Evidence exhaustion is a reasoned assessment that further **reasonable and authorized** investigation avenues are unlikely to yield material new information for the specified question at the current time.

It is **not** shown by any of these alone:

- A planned source count or tool-call limit has been reached.
- Several pages repeat the same original narrative.
- One search engine finds nothing.
- The original source is behind access restrictions.
- The approved budget has been consumed.
- A polished narrative seems plausible.

Codex must document relevant distinct avenues tried, actual accessible evidence, missing originals, failed recovery, residual uncertainty, expected marginal value, and conditions that could make renewed investigation worthwhile. Limited access may indicate a **blocked** avenue rather than an exhausted question.

## 3.5 Impact-based gap assessment

A consequential unanswered question requires a scoped `GAP` record. Gap criticality is independently assessed on potential effect on:

- a mandatory charter objective or completion requirement;
- the reliability of major conclusions and causal mechanisms;
- downstream questions, dependencies and strategic interpretations;
- provenance, independence and contradiction handling;
- approved scope and assumptions.

A difficult or expensive gap is not automatically minor. Criticality must not be downgraded to satisfy an execution schedule or budget.

A **critical gap** can undermine a major conclusion, required research answer or dependency. A **noncritical gap** can remain an explicit limitation without materially compromising the approved objective.

## 3.6 Autonomous noncritical gap closure

After justified evidence exhaustion, Codex may close a genuinely noncritical gap without a separate human approval, recording:

1. Exact question and contract relationship.
2. Why the gap matters, and why its impact is noncritical.
3. Searched and inspected avenues plus meaningful failed attempts.
4. Recovered/inaccessible evidence and provenance restrictions.
5. What remains unknown and why further investigation is presently unlikely to help.
6. Effects on dependent claims, concepts or interpretations.
7. Conditions for revisiting the gap.
8. Related source, claim, journal and budget records.

This is **gap closure**, not verification of the unknown answer and **not** subphase completion. A critical unresolved gap is escalated, blocked or given an authorized qualified disposition under the [completion rules](../part-04-outputs-lifecycle/13-completion-and-acceptance.md); it cannot be silently labeled `exhausted-noncritical`.

## 3.7 Independent criticality and selective pause

Codex assesses gap criticality itself using the objective impact rules and makes that judgment auditable. If material new evidence invalidates an approved charter assumption, document the specific dependency and pause only work that relies on it. Continue unrelated authorized investigation. Propose a human-approved amendment when required; no autonomous charter rewrite.

If a critical gap or red-team trigger prevents defensible final conclusions, record it rather than forcing agreement. Chapter 05's independent reviews and Chapter 13's closure checks govern completion.

## 3.8 Investigation journal

Codex must maintain a meaningful chronological journal of material research activities, including source discovery/inspection, failed avenues, source recovery, hypothesis changes, contradictions, gaps, reviews, resource events, and consequential decisions. Each entry should reference durable authoritative records where available.

Repeated low-value search calls may be summarized. The journal is not a duplicate source register or transcript of every tool call. Do not fabricate timestamps for events whose time is unknown or infer evidence of an original document merely from a secondhand description.

Example journal entry fields: ordered entry marker; contract question; action **actually performed**; source/claim/gap/concept references; result/failure; relevant hypothesis change; impact/dependencies; budget authorization; next authorized action.

See the [journal template](../../templates/investigation-journal.md) and [gap register](../../templates/gap-register.md).

## 3.9 Durable integration while investigating

Evidence must be recorded progressively in the standalone authoritative OKF workspace, with distinct source, claim and semantic concept layers (Chapter 04). Records can remain provisional; persistence is **not** acceptance.

Scoped identities must be issued by the project ledger and workspace-wide `K` identities by the workspace counter. Persist identity issuance before record creation; persist material records before indexes and journal references, validate, then advance the active checkpoint last. Interrupted writes must not cause ID reuse or lost evidence. See [standalone OKF conventions](../../references/standalone-okf-conventions.md).

## 3.10 Investigation reporting and separate completion audit

Investigation may report contract-question progress, linked evidence and limitations, noncritical gap closures, pending or completed genuine `RT` reviews, and authorized budget consumption. It must not misrepresent any unperformed red-team review as passed.

**Investigative progress is not itself subphase or project completion.** To close work, follow the separate [Chapter 13 criterion-by-criterion audit](../part-04-outputs-lifecycle/13-completion-and-acceptance.md) and write the required [completion dossiers](../../references/completion-and-acceptance.md). Critical blockers, mandatory review dispositions and charter conditions remain binding. A draft book becomes a completed deliverable only after all applicable completion checks pass.

## Chapter navigation

- **Previous:** [Chapter 02 — Governance and Planning](../part-01-foundations/02-governance-and-planning.md)
- **Next:** [Chapter 04 — Evidence and Source Integrity](04-evidence-and-source-integrity.md)
- **Procedures:** [Authorized investigation](../../references/investigation-execution.md) · [Gaps and journal](../../references/gaps-and-journal.md)
- **Templates:** [Contract](../../templates/research-contract.md) · [Gap registry](../../templates/gap-register.md) · [Investigation journal](../../templates/investigation-journal.md)
