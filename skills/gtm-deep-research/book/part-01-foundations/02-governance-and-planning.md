# Chapter 02 — Governance and Planning

[Previous: Chapter 01](01-research-modes-and-charters.md) · [Part I index](index.md) · [Book home](../index.md) · [Next: Part II](../part-02-investigation/index.md)

**Purpose:** Balance independent, depth-first research with explicit human authority over consequential research direction, planning and resource authorization.

**Governing decisions:** DR-003, DR-005, DR-006, DR-011, DR-017.  
**Operational scope:** The full protocol includes contract/charter-verified completion, selective reopening and recovery. Installing the skill and beginning a project remain separately authorized activities.  
**Operational procedure:** [Progressive planning and contracts](../../references/progressive-planning-and-contracts.md).

## 2.1 Governing principle

GTM Deep Research must exercise **high autonomy within approved limits**, not silently expand those limits. Codex independently handles routine planning refinements and routine investigation, evidence verification and bounded exploration. The human controls consequential decisions about goals, approved research scope, plans, important assumptions and resources beyond established allowances.

The skill maintains its own versioned charter, plans, project decisions and active-state checkpoint within the standalone OKF workspace. It must not delegate approvals or execution authority to Goal Memory.

## 2.2 Distinct human authorization gates

The following are distinct authorization objects; approval of one is not blanket permission for another:

| Decision or action | Human authorization | Why |
|---|---|---|
| Research goal and versioned charter | **Required** | Defines objectives, boundaries and completion criteria |
| Full high-level phase outline | **Required, separately** | Authorizes the research strategy and phase boundaries |
| Immediate detailed phase/subphase plan | **Required** | Authorizes a specific next execution block |
| Attached contract fitting the approved detailed plan | Can be approved **in the same explicit decision** as the detailed plan | Avoids duplicate gates but requires exact contract identification |
| Routine plan wording and tactical choice within approved boundaries | Not separately required | Does not materially change authorization |
| Consequential charter, scope or plan amendment | **Required before taking effect** | Changes approved research direction |
| New spending or hard ceiling increase beyond allowance | **Required before action** | Protects explicit resource authorization |
| Autonomous noncritical gap closure or objective subphase/project completion | Not an extra human acceptance by default | Requires specified evidence/review/contract checks |
| Significant unresolved review or invalidated assumption | Escalate under applicable rules | Cannot be silently resolved by convenience |

Required learning checkpoints are distinct from research approvals. Understanding an interpretation does not establish its evidentiary validity or approve an amended research plan.

The live decision ledger must record **actual human decisions** and the versions/objects they authorize; a proposed record or implied assent is not an approval.

## 2.3 Hierarchical progressive planning

Planning proceeds through linked but separately authorized levels:

1. **Approved charter:** What/why/boundaries/evidence and completion rules.
2. **Approved high-level phase plan:** Complete outline of major phases, their objectives, order, dependencies, milestone outputs and approximate allocations.
3. **Approved immediate detailed phase/subphase plan:** Enough method, scope, questions, evidence requirements, budget and review triggers to execute the next block.
4. **Approved contract within that plan:** Explicit research question set, strategy, required OKF outputs, reviews and completion conditions.
5. **Later elaboration:** After evidence is obtained, detailed planning of subsequent phases is proposed and approved when required.

The full high-level phase outline should be approved before substantive execution. Detailed distant-phase contracts should **not** be locked prematurely when current findings might change their design. Detailed plans and contracts must stay within the authorized charter.

Use the [plan template](../../templates/research-plan.md) and [research contract template](../../templates/research-contract.md). A plan with an attached contract may be jointly reviewed under one explicit detailed-plan decision if the exact versions and scope are clear. This does not collapse the charter and high-level plan gates.

## 2.4 Depth-first investigation principle

When execution capabilities are implemented and authorized, Codex must thoroughly investigate an active subphase before proceeding to dependent work. Investigation considers consequential evidence avenues, corroboration, competing explanations, contradictions and gap closure conditions.

**Depth-first is not infinite research.** A subphase may close after objective contract satisfaction, mandatory reviews, and permitted qualified outcomes supported by justified evidence exhaustion. Budget or source-count exhaustion alone does not prove evidentiary completion.

Parallel discovery may support the active subphase where useful, provided it does not bypass dependency, review, approval or resource rules.

**Completion boundary:** Investigation, noncritical gap exhaustion, journaling and genuine red-team/adjudication may proceed within authorized scope and budget. **Closing** a subphase/project requires a separate [contract/charter audit and versioned dossier](../../references/completion-and-acceptance.md); having research and review records alone does not satisfy completion.

## 2.5 Bounded researcher discretion

Codex may propose and investigate promising leads within the approved charter and any explicitly granted discretionary allowance. Routine tactics can evolve without repeated interruptions.

Codex must not:

- Rewrite an approved charter or plan because it discovers a compelling alternative.
- Elevate an exploratory hypothesis to historical fact without appropriate evidence.
- Exceed a hard budget or incur paid-service charges without approval.
- Treat an adjacent subject as included merely because it appears relevant.
- Treat acceptance of a learning explanation as authorization for a consequential change.

A material change proposal should identify the discovered evidence, proposed amendment, reason, likely benefits, dependent work and resource effect. Obtain explicit human authorization before it takes effect.

Approved in-scope leads may be investigated under the exact authorized contract. Adjacent material leads outside charter/plan discretion must be proposed, not silently investigated.

## 2.6 Adaptive human collaboration

Human participation should occur at meaningful decision points: consequential discoveries, competing interpretations, significant unexpected outcomes, scope or plan changes, strategic decisions, unresolved red-team disputes, and phase boundaries. Codex should avoid blocking every routine action with unnecessary approvals.

Learning discussions are configurable and generally nonblocking for unrelated authorized work. The detailed teaching and checkpoint procedure is [Chapter 12](../part-04-outputs-lifecycle/12-human-learning.md); learning cannot override evidence assessment or required governance gates.

## 2.7 Invalidated assumptions and selective pausing

Codex must detect when new evidence materially undermines an assumption on which the approved charter or plan depends. It should:

1. Identify the exact assumption and the evidence or observation challenging it.
2. Assess consequences for objectives, causal explanations, dependencies and planned questions.
3. **Pause only work that materially depends on the invalidated assumption.**
4. Continue unaffected work within existing authorization.
5. Draft an amendment with alternatives, scope/budget effects and justification.
6. Obtain the necessary human approval and preserve the former state and decision history.

**Illustration:** A plan assumes early paying customers were universities, while newly found information credibly suggests enterprise recruiters were the first revenue source. Codex should flag dependent early-customer hypotheses and commercial analysis, but need not discard unrelated market history. It must not automatically rewrite the charter based on incomplete information.

If prior completion or red-team results are materially affected, [Chapter 09](../part-03-okf-architecture/09-shared-knowledge-and-dependencies.md) governs known downstream dependencies and selective reopening. Codex may flag/reopen affected completed work after material evidence, but must obtain authorization for any new spending, charter scope or detailed plan.

## 2.8 Authorization records and safe checkpoints

Research governance is only durable when it is recorded within a safely initialized standalone OKF workspace:

- Issue decision/contract IDs through the authoritative scoped ledger, never by reusing a number.
- Record exact objects, versions and the actual human authorization before marking them approved.
- Persist approved content and consequential decision history.
- Update links/indexes, validate essential consistency, then advance the active-state checkpoint.
- Stop affected writes when authorization or recovery state is ambiguous.

The charter and plan are distinct; no duplicate active-state authority is created. See [standalone OKF conventions](../../references/standalone-okf-conventions.md).

## 2.9 Chapter completion and lifecycle handoff

This chapter's governance design is satisfied when the goal/charter, high-level phase plan, and immediate detailed plan/contract have appropriate explicit approval and durable records, and the next proposed action is bounded and unambiguous.

**Full workflow:** Execute a contract only after the [authorized research start gate](../../references/investigation-execution.md) passes; capture evidence, close only justified noncritical **gaps**, conduct [red-team adjudication](../../references/red-team-and-adjudication.md), respect [budgets](../../references/research-budget-management.md), build [evidence-linked books](../../references/research-book-architecture.md) and optional [learning checkpoints](../../references/human-learning.md). Subphase and project completion require the separate [criterion-by-criterion audit](../../references/completion-and-acceptance.md). Material new evidence can trigger [selective reopening](../../references/dependency-impact-and-reopening.md) without granting new spending or scope. No activity may bypass plan or budget authorization.

## Chapter navigation

- **Previous:** [Chapter 01 — Research Modes and Charters](01-research-modes-and-charters.md)
- **Next:** [Chapter 03 — Research Contracts and Investigation](../part-02-investigation/03-research-contracts-and-investigation.md)
- **Procedures:** [Planning and contracts](../../references/progressive-planning-and-contracts.md) · [Plan template](../../templates/research-plan.md) · [Contract template](../../templates/research-contract.md)
- **Decision index:** [DR-001–DR-052 map](../appendices/decision-coverage.md)
