# Chapter 10 — Research Synthesis and Lessons

[Book home](../index.md) · [Part IV](index.md) · [Previous: Part III](../part-03-okf-architecture/index.md) · [Next: Chapter 11](11-book-architecture-and-navigation.md)

**Status:** Approved consolidated specification, operationally specified for evidence-linked synthesis and revisions. **Governing decisions:** DR-033, DR-034, DR-036. See [synthesis procedure](../../references/research-synthesis-and-lessons.md), [revision procedure](../../references/synthesis-revisions.md) and [draft chapter template](../../templates/research-book-chapter.md).

**Purpose:** Transform authoritative researched evidence into coherent GTM explanations and appropriately conditional lessons without confusing reported accounts, verified events, causal interpretation and prospectively applicable advice.

## 10.1 Authoritative research and derived synthesis

The standalone OKF workspace is authoritative for source provenance, claims, evidence states, red-team outcomes, semantic `K` concepts and consequential research decisions. The charter-defined research book is a **derived reader-facing synthesis**, not a parallel evidence store. A materially supported book claim must point back to existing `K` and qualified project `CLM`/`SRC`/`RT` records. Recording a sentence in a book is not independent corroboration of that sentence.

The research book may itself reside within the OKF workspace; its readable presentation role does not displace the original records. If evidence or review state changes, the related prose must be reviewed and selectively revised.

## 10.2 Charter-defined synthesis scope

The approved charter determines audience, format, depth, required questions and completion criteria. Depending on the GTM investigation, narrative coverage may include market preconditions, founders, product positioning, early user acquisition, first paying customers, marketing, sales, pricing, partnerships, failed experiments, competitive responses, revenue trajectories, retention, causal mechanisms and transferable implications.

No such chapter's existence is proof that underlying data were found. When a mandatory question cannot be answered from legitimate evidence, the book must document that gap instead of inventing a satisfying narrative. Other research domains may use different structures if charter scope warrants.

## 10.3 Three analytical layers

**Observation:** What was directly observed in an inspected artifact, or that a person/source made a particular *reported* assertion. Distinguish archived advertised pricing from realized customer revenue, and founder statements from verified historical transactions.

**Causal interpretation:** What likely contributed to the outcome, how, under what temporal and contextual conditions, and what rival explanations remain. Showing that two events occurred together does not establish one caused the other.

**Transferable lesson:** What the researched company's experience teaches, why that insight follows, and which general business conditions and failure modes limit it. Lessons may stay within the researched company's type of business. Apply them to the user's business only when separately requested; never import that business from conversation history.

The synthesis must label these layers in substance, though it need not mechanically repeat a three-part form for every paragraph.

## 10.4 Evidence-calibrated lessons

When extracting a consequential GTM lesson, Codex must identify: (a) the supporting historical observations and their scope; (b) proposed causal mechanism and mandatory `RT` review if major; (c) plausible alternative explanations; (d) transfer/applicability conditions; (e) important differences in market, buyer, timing, channel access and product economics; (f) plausible failure modes; (g) qualitative confidence and validation opportunity.

If the causal mechanism is unverified, the lesson may be a **conditional hypothesis to test**, not a proven recommendation. A red-team-qualified causal model cannot silently turn into a certain strategic prescription in a later chapter.

## 10.5 Rival models and disclosed uncertainty

The synthesis must distinguish strongly supported, meaningfully supported but qualified, plausible/unverified, disputed and refuted interpretations. It must make material disagreements and unresolved critical gaps visible in the chapter they affect, as well as link to the appropriate indexes/appendices.

A source supporting that a founder **said** something does not by itself verify that the historical assertion is true. Multiple copies of one original account do not constitute independent confirmation. Do not manufacture numerical probabilities from qualitative confidence labels.

Major conclusions with `review: pending` can be explored in a clearly labeled **draft hypothesis** but cannot be presented as independently reviewed. `qualified` and `unresolved` review states must be reflected in the narrative. Neither human agreement nor elegant prose resolves the evidentiary issue.

## 10.6 Traceable synthesis workflow

Before outlining, reconstruct the company journey from the records: customer problem and alternatives, actual product workflow, user/buyer/payer, acquisition, economics, outcome and reason for change. Use this as an internal thinking aid. Organize the prose around how the business evolved, not the order of source discovery.

For a general reader, introduce the company and industry before disputes about dates. Explain each material transition through the prior situation, pressure or opportunity, company response and result. Distinguish founders' stated reasons from supported author interpretation in ordinary language. Do not invent motives or force overlapping products into a single pivot.

Select details by whether they change understanding of a decision, customer, business model, outcome or lesson. Use readable citations with detailed source comparisons in notes. Keep material uncertainty near the affected conclusion, without repeating access caveats after every paragraph. Internal IDs, review badges and approval mechanics belong in notes or project records.

The detailed authoring and two-pass editorial/evidence review are defined in the [synthesis procedure](../../references/research-synthesis-and-lessons.md). Review an introduction and one material transition before applying substantial writing changes to the affected chapter.


1. Validate approved charter, reader audience and current contract/authorization limits.
2. Read current `K` concept records and linked qualified `CLM`, `SRC` and `RT` records, including counterevidence, access mode and review status.
3. Map mandatory questions and material conclusions to sections; identify missing evidence or unresolved review needs.
4. Draft substantive explanations in clear chronological/thematic order, citing the source/evidence chain where materially relevant.
5. Present significant rival explanations and limitations faithfully.
6. Derive scoped transferable implications only when justified by reviewed evidence, noting conditions for application.
7. Check navigation and citation links using [Chapter 11](11-book-architecture-and-navigation.md), then persist substantive edits and indexes before checkpoint advancement.
8. Leave lifecycle status `draft` or `revision-pending` during synthesis; [Chapter 13](13-completion-and-acceptance.md) separately verifies charter/contract criteria before any completed status can be assigned. A generated chapter never closes research by itself.

## 10.7 Versioned selective maintenance

On new evidence, Codex must reassess impacted source/claim/concept/review records **before** revising derived book text. Identify affected chapters, preserve previous consequential wording or version references, record trigger evidence and its effect on conclusions, then integrate the evidence into the relevant historical stage and resynthesize affected sections and transitions. Consolidate duplicate explanations rather than appending successive source summaries. Preserve stable IDs and repair indexes/links.

Minor typographic changes need not cause full book regeneration. Material evidence revisions must not be suppressed to protect the previous narrative. A newer book version is not automatically a more certain conclusion.

Use a [local revision ledger](../../templates/synthesis-revision-log.md) with stable entry anchors, **not** a competing evidence registry or new global ID counter. Consequential top-level structural changes require the human approval prescribed by Chapter 11. Materially invalidated completed research follows the separate [Chapter 09 reopening procedure](../part-03-okf-architecture/09-shared-knowledge-and-dependencies.md), preserving old dossiers and new authorization gates.

## 10.8 Illustrative GTM interpretation (not a finding)

Suppose a hypothetical company ran a campus contest. An archived site may support the observation *a competition was advertised*. It does not alone prove there were paying enterprise customers or that the contest caused growth. A lesson from this case might distinguish attracting candidates from acquiring paying employers. Its usefulness depends on whether the contest actually produced each outcome and on what other channels were operating. A comparison to the reader's own business is not presumed.

## 10.9 Integrity and scope gate

Before using a chapter as a substantive research output, check approved scope, true accessed sources, specific claim definitions, contradictory evidence, confidence, red-team review, evidence links and version history. A reader-facing draft deliverable is not evidence of research completion, which requires [Chapter 13](13-completion-and-acceptance.md) verification and a durable dossier.

**Next:** [Chapter 11 — Book Architecture and Navigation](11-book-architecture-and-navigation.md) · [Detailed synthesis procedure](../../references/research-synthesis-and-lessons.md).
