# Chapter 05 — Independent Red-Team Review

[Book home](../index.md) · [Part II](index.md) · [Previous: Chapter 04](04-evidence-and-source-integrity.md) · [Next: Chapter 06](06-research-budgets.md)

**Status:** Approved consolidated specification, operationally specified. **Governing decisions:** DR-014, DR-015, DR-016. See [red-team and adjudication procedure](../../references/red-team-and-adjudication.md) and [review record template](../../templates/red-team-review.md).

**Purpose:** Subject major GTM conclusions to a genuinely separate adversarial research investigation, document counterevidence and competing causal models, and adjudicate disagreements without fabricating certainty.

## 5.1 Mandatory independent review

Every major research conclusion **must** receive a substantive independent red-team pass before the conclusion is relied on as reviewed. A red-team pass is not merely editing prose, restating the researcher's argument or asking for generic objections; it actively investigates **how the exact conclusion could be wrong**.

The procedure must retain source provenance, uncertainty, independent information lineage and distinct claim evidence/review states. It must not manufacture consensus or assert a source was read when only a summary was available.

## 5.2 Impact-based major-conclusion classification

Classify each material conclusion with respect to:

- Importance to approved charter questions and completion basis.
- Causal or strategic significance; early customer acquisition, pricing drivers and GTM success mechanisms are presumptively consequential.
- Dependencies on which subsequent interpretations or projects rely.
- Consequences of error, including strategic decisions informed by the conclusion.
- Current uncertainty, contradictions and alternative explanations.
- The effect a changed conclusion would have on the overall research narrative.

A compound or aggregate conclusion may be **major** even if no constituent observation independently qualifies. Codex must not avoid mandatory review by dividing one consequential conclusion into numerous innocuous claims.

Record the classification and rationale, with the relevant `CLM` and semantic `K` targets. Non-major material interpretations may carry an auditable `not-required` rationale; classification must be reevaluated if usage or dependency impact changes.

## 5.3 Substantively independent adversarial investigation

The red-team investigation is a distinct authorized pass, with its own search work and record.

1. **Freeze target:** Identify precise original proposition, scope, timeframe, definitions, cited sources, evidence state and confidence *before* the challenge.
2. **Generate countermodels:** Form rival explanations, confounders, disconfirming predictions and falsification criteria without assuming the original hypothesis is correct.
3. **Discover counterevidence independently:** Search contemporary, primary, archival and relevant independent sources specifically for disconfirmation; inspect legitimate accessible originals and record source lineage.
4. **Interrogate the inference:** Test evidence relevance, bias, timing, source interdependence, survivorship/selection effects, missing variables and narrowness of observed facts.
5. **State strongest objections:** Distinguish what is refuted, what is qualified and what remains uncertain.
6. **Persist the record:** Use a distinct project-scoped `RT` identifier and link new source/claim records and meaningful journal actions.

A different model or person is permitted, not required. If one model performs both passes, a separate adversarial evidence-discovery step and transparent record remain mandatory. Do not falsely claim a second agent participated.

A review lacking the adversarial investigation must remain `pending`.

## 5.4 Red-team review record

A consequential review must record:

| Element | Required content |
|---|---|
| Identity | Stable `PRJ:RT` reference and review version/history |
| Target | Exact original and aggregate claims/concepts under challenge |
| Reason for review | Impact classification and causal/strategic/dependency rationale |
| Original case | Researcher's argument, evidence, confidence and limitations |
| Independent research | New avenues actually attempted, accessed evidence and shared lineage |
| Disconfirmation | Counterevidence, source quality, strongest criticisms and falsifiers |
| Alternatives | Competing GTM mechanisms and confounders |
| Adjudication | Evidence comparison, bounded further work and outstanding disagreement |
| Disposition | Procedural review state and reason; evidence/confidence separately |
| Follow-up | Qualified wording, escalation, dependency pauses, revisit triggers and audit |

Records may be grouped, but logical `RT` identities must remain stable across file moves. Reviews can target a meaningful aggregate conclusion instead of creating one review per trivial claim.

## 5.5 Bounded evidence-based adjudication

If original research and red-team reach materially different positions, Codex must:

- Compare exact propositions and definitions, timeframes and scope.
- Compare source directness, quality, independence, incentives and historical proximity.
- Seek decisive additional evidence **only within authorized contract, budget and access boundaries**.
- Preserve differences between observation, founder-reported statement, inferred causality and generalizable GTM lesson.
- Update claim confidence/evidence states only on evidence, not because the review completed.
- Document unresolved ambiguity and its effect on dependent conclusions and research plans.
- Escalate consequential unresolved disputes without treating them as administratively resolved.

Human approval may authorize proceeding with a qualified outcome when charter rules permit it, but it cannot establish a disputed historical proposition as fact. If adjudication requires material scope/budget changes, obtain the separate applicable approval first.

## 5.6 Independent review states and outcomes

Evidence state, qualitative confidence and independent review state are distinct:

| Review state | Meaning and required evidence |
|---|---|
| `not-required` | Substantively non-major by documented impact rationale; reevaluate on changed use |
| `pending` | Major review due, not yet substantively completed, or missing independent search |
| `passed` | Independent pass completed; no material unresolved challenge to the *exact appropriately scoped* conclusion |
| `qualified` | Completed pass requires narrower proposition, conditions or explicit limitations |
| `unresolved` | Consequential dispute remains after bounded adjudication; escalate and block dependent completion as applicable |

`refuted` is an **evidence state**, not a review state. `passed` means the challenge process was completed satisfactorily, **not** that underlying evidence automatically becomes high confidence. A formerly passed review may later become stale; preserve the prior version and set affected conclusion review `pending` for new applicable red-team work.

A red-team `RT` record can additionally track workflow progress (`investigating`, `adjudicating`), separate from the target claim's review state.

## 5.7 Consequences of review

A completed red-team pass may produce narrower conclusions, changed claim confidence, new gaps, dependencies, previously missing source avenues, or a proposed charter amendment. Material invalidation may selectively pause dependent work while unrelated research continues.

Critical unresolved discrepancies must receive an explicit disposition before their affected contract can satisfy its completion criterion. Neither a favorable review nor exhausted authorized budget alone is permission to close an entire subphase. Completion requires the separate [Chapter 13 audit](../part-04-outputs-lifecycle/13-completion-and-acceptance.md).

## 5.8 GTM example (illustrative, not a factual finding)

**Original hypothesis:** “Campus competitions were the primary cause of Company X's early growth.”

**Adversarial alternatives:** Competitions correlated with, but did not cause, acquisition; university partnerships provided distribution; founder networks recruited early institutions; market timing or other product advantages affected growth.

**Evidence tests:** Dated distribution agreements, attributable referrals, customer acquisition sequences, historical channel attribution, contemporaneous feedback, contradictory participant accounts, and definitions of *users* vs *paying customers*.

**Possible outcome:** “Competitions formed part of an early acquisition program; their relative causal contribution remains unverified.” Record it as qualified if the actual reviewed evidence warrants that narrowing. Do not assert this outcome about a real company without sources.

## 5.9 Operational handoff and stop

Before marking review disposition complete, verify: target frozen; major classification reason; truly separate evidence search; alternative models/falsification; independent source attribution; bounded adjudication and budget authorization; review state distinct from evidence/confidence; stable `RT` references; consequential unresolved conflicts escalated; OKF write/checkpoint ordering respected.

**Operational handoff:** Independent review outcomes feed [criterion-based completion](../../references/completion-and-acceptance.md) and [impact-based reopening](../../references/dependency-impact-and-reopening.md); those processes must independently verify their requirements and authorizations.

**Next:** [Chapter 06 — Research Budgets](06-research-budgets.md) · [Budget procedure](../../references/research-budget-management.md).
