---
name: goal-memory
description: Guide substantial project goals through focused discussion, private OKF memory, and reviewable phases. Use for substantial project goals, goal-memory work, or when memory temp/index.md exists.
---

# Goal memory

Use for features, fixes, refactors, new projects and exploration. Make and verify clear, small fixes directly. For substantial or ambiguous work, use the workflow below. Explicit user instructions override defaults.

Ground collaboration in the [operating model](references/HOW-TO-USE.md#operating-model): the human directs; the agent investigates, challenges and acts within its authority; both build and use reliable shared context.

## Workflow

Use Manual mode by default. Use subagents only in Auto, unless the user explicitly instructs otherwise. Switch modes only on explicit user instruction or approval; an active goal alone does not authorize Auto. Before planning, follow the [mode guide](references/HOW-TO-USE.md#work-modes) for authority, switching and Auto review.

1. **Understand.** Read relevant files and memory first. Separate facts, assumptions and proposals. Use the [probing guide](references/HOW-TO-USE.md#discuss-and-adapt) to ask one focused question at a time about a choice that changes the next step. Adapt to answers and record decisions, reasons and open questions as they arise. A request to understand or plan does not authorize implementation.
2. **Plan.** Map the outcome, phases and dependencies. Keep later phases provisional. Give each independently reviewable phase its own numbered concept when preparing it. Agree on the next phase's scope, approach and checks where needed. Reuse prior authorization.
3. **Implement and verify.** Work within the granted scope. When evidence materially changes behavior, architecture, scope or risk, decide within delegated authority or pause affected work for human direction. Continue unaffected authorized work.
4. **Review and learn.** Explain what changed, why and what the checks showed, including limitations. Apply feedback and update memory. At meaningful checkpoints, use the [learning loop](references/HOW-TO-USE.md#learn-and-apply-working-patterns) to review available conversation and work for durable patterns. In Manual, offer each phase for human review by default; in Auto, follow the authorized review loop. Continue across phases or commit only when authorized. Record implementation, verification, review, approval and commits separately as they occur.

## Private memory

- For substantial work, follow the [initialization guide](references/HOW-TO-USE.md#initialize-and-recover-memory) to create or reuse the primary project's private, Git-ignored `memory temp/` bundle. Give each substantial goal or coherent discussion a named folder and local index when it begins, and link it from the root index and active state. Use the bundle for shared context across repositories and record each repository's location and role. Ask if the primary project is unclear. Keep memory private unless explicitly authorized to share it.
- On resume, read the index, working agreement, active state and working patterns. Follow relevant links and reconcile stale summaries against evidence.
- Update the detailed goal, phase or decision first, then active state, affected indexes and log. Preserve earlier decisions and reasons. Keep existing local reference copies unless migration is agreed.

## File references

Link relevant source files, phase records and evidence in plans, decisions and review notes. Use relative Markdown links within the bundle. For code across repositories, identify the repository and use a repository-relative path, adding a symbol or line when helpful. Find references before asking the user. If a necessary file cannot be located or accessed, ask for its path or link.

## References

- [Operating guide](references/HOW-TO-USE.md) — Initialize memory, work across repositories and maintain phase records.
- [OKF profile](references/SPEC.md) — Read before creating or updating memory. Follow its format, ID reservation, provenance and recovery rules.
- Starter templates — [working agreement](templates/001-working-agreement.md), [active state](templates/002-active-state.md), [working patterns](templates/003-working-patterns.md).
