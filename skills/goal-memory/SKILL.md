---
name: goal-memory
description: Guide substantial project goals through adaptive discussion, private OKF context, and small reviewable steps. Use for substantial project goals, goal-memory work, or when memory temp/index.md exists.
---

# Goal memory

Help the human understand and accomplish a goal while preserving context. Apply to new projects, features, fixes, refactoring and understanding-only work. Scale the process: make and verify a clear small correction directly; discuss substantial or ambiguous work. Explicit instructions override defaults.

## Understand together

Inspect the request, existing work and relevant memory before asking. Distinguish facts, assumptions and proposals. Explain the situation plainly; use responsibilities, state, actions and relationships when helpful. Use a short example, snippet, diagram or scenario when it clarifies a choice.

Keep the whole goal in view while focusing on one manageable part. Ask one short, focused question at a time by default. Offer a simple recommendation and reason when useful. Do not ask for answers already provided or discoverable in the project. If an answer is broad, investigate and suggest a concrete focus. Adapt to each answer and revisit affected assumptions when necessary. Continue until material uncertainty is resolved or explicitly accepted; do not infer agreement from silence.

Record meaningful answers, decisions, reasons and open questions in their memory document during discussion. Summarize understanding and scope when agreement matters. A request to understand or plan alone does not authorize implementation.

## Plan and work in small pieces

Map the outcome, major phases and known dependencies for substantial goals. Keep later phases provisional; discuss the next cohesive, reviewable slice in detail: purpose, scope, approach, affected areas and verification. Anticipate consequential risks without inventing complexity. Respect prior authorization; do not ask again for an authorized step.

Implement the authorized slice, verify what is practical and permitted, and explain why, what changed, how it works and what checks show. Use a diff or scenario when helpful. Answer review questions, make requested corrections and preserve new understanding in memory or useful code comments. By default offer the slice for human review before the next; explicit instructions may authorize continuous progression. Commit only when instructed, unless explicitly authorized otherwise for the goal or phase.

Distinguish proposed, implemented, verified, reviewed, approved and committed; never invent evidence or approval. A commit does not establish approval. If evidence materially changes agreed behavior, architecture, scope or risk, pause affected work, investigate and discuss the choice; continue unaffected authorized work. Routine choices remain within the agreed slice.

## Private context

For substantial work with an established project location, initialize private memory temp/ automatically if absent. Do not initialize for a small self-contained task. Reuse existing memory without overwriting it. Where Git applies, protect it with a root-anchored /memory temp/ ignore rule and check whether files are tracked. An ignore rule does not untrack files. Do not commit, delete or export memory without explicit authorization. Without a project location, continue discussing and establish the location before creating memory.

On subsequent work, read the root index, working agreement, active state and working patterns, then selectively follow relevant links. Reconcile inconsistencies from evidence; never invent past approval. Update the detailed goal or decision first, then active state, indexes and log as affected. Preserve earlier decisions and reasons when changed. Read [the operating guide](references/HOW-TO-USE.md) for discussion, execution and initialization, and [the OKF profile](references/SPEC.md) when maintaining memory. Installed references are templates; project copies are local snapshots and must not be silently overwritten.
