# Chapter 14 — Standalone GTM Research Skill Implementation and Review

[Previous: Chapter 13](../part-04-outputs-lifecycle/13-completion-and-acceptance.md) · [Part V](index.md) · [Book home](../index.md) · [Final static audit](../../references/final-static-audit.md)

**Governing decisions:** DR-048, DR-049, DR-052 and standalone amendments DR-040-R–042-R, DR-044-R. **Purpose:** Implement the approved research skill faithfully, reviewably and independently of Goal Memory, validating its specification without overclaiming proven runtime reliability.

## 14.1 Scope of the standalone skill

GTM Deep Research is a reusable Codex skill for historical and analytical GTM research: market before formation, founding/product, initial users and paying customers, acquisition, sales, positioning, pricing, revenue, growth, failures, competitive responses, causal interpretation and conditional strategic lessons. It independently owns its Markdown-first OKF research workspace and its research lifecycle. There is **no Goal Memory dependency**, inherited `memory temp/` workspace, global external allocator, separate required service or Docusaurus build. General-purpose evidence rigor survives domain specialization.

## 14.2 Authoritative documentation layers

The approved **five-part, fourteen-chapter** Markdown OKF specification book governs *skill behavior*. Root `SKILL.md` is the concise operational entry point, linking to focused procedures and templates. The *research workspace* is independently initialized under a user-approved root and holds authoritative provenance, claims, concepts, decisions and state. Its generated *research book* is derived reader-facing synthesis, not a competing historical evidence authority. These three layers have distinct roles and must not be conflated.

## 14.3 Architecture and approval boundaries

The skill uses one workspace-wide `K` allocator and project-scoped `PRJ:SRC/CLM/RC/RT/GAP/DEC` ledgers; `DR-###` labels are design decisions only. Human approval is required for live workspace root initialization, goal/charter, high-level phase plan, immediate detailed plans/contracts, material changes and unauthorized budget extensions. Routine evidence investigation, major-conclusion red-team, eligible noncritical gap closure and contract-verified subphase/project completion may operate autonomously *within approved boundaries*. Reopening may be autonomous when material evidence is encountered, but new scope/spending/plan execution remains separately gated.

## 14.4 Incremental delivery history and scope

Implementation proceeds in independently reviewed increments:

| Increment | Capability |
|---|---|
| 1 | Standalone skill foundation, OKF conventions, navigation and identities |
| 2 | Research activation, bounded reconnaissance, charter, plans and contracts |
| 3 | Authorized investigation, source/claim/confidence, gaps and journal |
| 4 | Major-conclusion independent `RT`, adjudication and adaptive budgets |
| 5 | Evidence-linked draft research books, transferable lessons, selective revisions and learning |
| 6 | Autonomous completion, selective reopening, dependencies, recovery and final static audit |

A newer package does not retroactively make historical increment review records describe features that did not then exist. Each increment has its own approval, review and authorization trace. The complete original specification and subsequent standalone amendment were approved before implementation; material later changes require approved amendments with version history.

## 14.5 Minimal skill file structure

`SKILL.md` should state triggers, stop conditions, main workflow, human authorization, evidence integrity, red-team, budget, book, completion and reopening constraints, and links to focused references. Operational references implement concrete procedures. Templates illustrate empty records, **not** true evidence, an initialized workspace or obtained human approval. The canonical specification book has part indexes, full chapter navigation and audit appendices. Prefer Markdown and light indexing to redundant scripts, databases or a giant duplicated prompt.

## 14.6 Static validation method

DR-048 selected specification and static inspection, **not** a mandatory automated integration test framework. The final audit must inspect frontmatter and activation instructions; all 14 materialized chapters; DR-001–DR-052 mapping without duplication; R-01–R-08 and standalone supersession; internal link resolution; record/ID and write/recovery consistency; role/authority and budget gates; major/aggregate red-team rules; allowed critical-gap disposition; book provenance/revisions; and completion/reopening limits. The [static review procedure](../../references/final-static-audit.md) sets reportable methods and honest limitations.

These checks can establish that particular Markdown instructions and links are present and internally consistent. They do **not** establish that Codex will obey them perfectly in all runtime environments, that live research will be accurate, that files can be recovered in all crash cases, or that a Docusaurus site builds successfully.

## 14.7 Workflow examples and quality review

The supporting documentation should illustrate lightweight questions that avoid full protocol; substantial charter/plan approval; early paying-customer uncertainty; actual accessed sources and contradictory claims; separate adversarial red-team evidence search; justified budget extension; consequential assumption invalidation; an evidence-linked reader-facing book; autonomous criterion-based completion; material reopening with old completion preserved; and interruption recovery with nonreused IDs. Examples must remain clearly hypothetical unless supported by actual inspected research evidence.

A final static review must distinguish **pass**, **fail** and **not verifiable statically**. Known limitations, incompatible external conditions and open consequential defects must be disclosed. Fix consequential static failures and rerun relevant checks before proposing release.

## 14.8 Release readiness and final human gate

The packaged skill requires explicit human release authorization before distribution as released. It must not be silently installed, initialized in a repository, or used for paid research. Release requires explicit final human approval separate from completion of the implementation increment. Even after approval, live workspace creation requires authorization of its target root, and research remains subject to charter/plan and expenditure gates.

If implementation reveals a consequential specification incompatibility, record it with affected DR mappings and tradeoffs, seek an amendment, preserve revision history and do not quietly downgrade an approved requirement. Editorial improvements may follow normal authorized maintenance.

## 14.9 Future evolution

Actual use may reveal improvements to source discovery, evidence indexing, GTM specialization, versioned books or optional runtime testing. Changes must remain minimal and traceable. A future integration with an external goal-management system, automated monitor or Docusaurus publisher is optional and requires separate approval; none is implicit in this release.

**Static validation:** [Static audit procedure](../../references/final-static-audit.md) · [Decision coverage](../appendices/decision-coverage.md) · [Reconciliations](../appendices/audit-reconciliations.md).
