# Chapter 07 — Standalone OKF Workspace and Research State

[Part III index](index.md) · [Book home](../index.md) · [Previous: Chapter 06](../part-02-investigation/06-research-budgets.md) · [Next: Chapter 08](08-research-records-and-identity.md) · [Implementation conventions](../../references/standalone-okf-conventions.md)

**Scope:** Approved standalone architecture, maintained across all six implementation increments. This chapter supersedes the former generic OKF / Goal Memory integration assumptions in the initial draft.

**Governing decisions:** DR-024, DR-025, DR-040-R, DR-041-R, DR-042-R.

## 7.1 Architectural authority

GTM Deep Research is independently usable. It owns research charters, phase plans, consequential decisions, approved contracts, provenance, claims, red-team reviews, budgets, concepts, semantic indexes, project state, research books, completion and recovery. Goal Memory, `memory temp/`, its allocator and its approval records are **not** required or inherited. OKF means a single semantic, Markdown-first, linked and auditable research knowledge environment.

## 7.2 One authoritative workspace

An approved research root contains navigation, workspace controls, reusable knowledge and project-specific research records. No shadow source of truth may be silently created. The physical layout should be minimal and adaptable, with actual folders created only when needed. See the [proposed directory structure](../../references/standalone-okf-conventions.md#proposed-logical-layout).

## 7.3 Initialization and compatibility

Before live initialization, establish explicit human authorization for the root and scope. If the workspace is missing, follow approved initialization. If an existing workspace is inconsistent, do not overwrite it: diagnose, preserve valid records, halt affected writes and reconcile. Full stateful research must not proceed without durable evidence and recovery guarantees.

## 7.4 Minimal internal OKF contract

The internal contract guarantees stable creation, workspace-wide concepts, scoped project records, semantic links, evidence provenance, human approval records, indexes, active checkpoints and recoverable writes. It is **not** an external API or a dependency on another skill.

## 7.5 Research governance

The skill records actual human approval for charter, plan, consequential scope and budget changes, without inferring authorization from proposals. The approval ledger belongs to the research project. Reopening does not authorize new scope or spending.

## 7.6 Compact active checkpoint

Each active project has one authoritative checkpoint referencing approved charter version, active phase/subphase and contract, open leads, dependencies, reviews, budgets, blocked decisions, next authorized action and recovery marker. It does not duplicate source or concept contents.

## 7.7 Ordered durable writes

Issue an ID durably before its record is created, preserve source/claim/concept/approval records, update indexes and journal references, validate and **only then** advance the active checkpoint. Issued identities must never be reused, even following failure. Prefer straightforward single-writer Markdown conventions; no speculative database-grade transaction guarantee.

## 7.8 Recovery

Inspect the checkpoint and durable files after interruption. Preserve valid content, reconcile incomplete indexes and references, and protect issuance counters. Never fabricate evidence or approvals or roll an ID counter backward. Escalate inconsistencies that cannot be safely repaired.

## 7.9 Missing workspace and optional interoperability

Read-only diagnosis may continue without the workspace, but not substantial unsaved stateful research. External imports may be authorized separately and must preserve provenance; no external goal-management system is required.

## 7.10 Acceptance of foundational architecture

The reviewed foundation must demonstrate a self-contained workspace model, non-destructive initialization policy, distinct identity namespaces, safe write order, compact recoverable state, and explicit human authority boundaries. The full research lifecycle uses [autonomous criterion-based completion](../../references/completion-and-acceptance.md), [selective reopening/dependencies](../../references/dependency-impact-and-reopening.md) and [explicit interruption recovery](../../references/recovery-and-consistency.md). Each requires its own evidence, checkpoint and authorization checks.
