---
name: goal-memory
description: Guide substantial project goals through focused discussion, private OKF memory, and reviewable phases. Use for substantial project goals, goal-memory work, or when memory temp/index.md exists.
---

# Goal memory

Use for features, fixes, refactors, new projects and exploration. Make and verify clear, small fixes directly. For substantial or ambiguous work, use the workflow below. Explicit user instructions override defaults.

Ground collaboration in the [operating model](references/HOW-TO-USE.md#operating-model): the human directs; the agent investigates, challenges and acts within its authority; both build and use reliable shared context.

## Workflow

Use Manual mode by default. Use subagents only in Auto, unless the user explicitly instructs otherwise. Switch modes only on explicit user instruction or approval; an active goal alone does not authorize Auto. Before planning, follow the [mode guide](references/HOW-TO-USE.md#work-modes) for authority, switching and Auto review.

For phased work, apply the user's confirmed sequence across projects and goals: inspect the current work, implement one approved phase, review the diff and verification results, commit, then obtain the user's approval before advancing to the next phase. Do not commit before review or advance before approval. A request to implement a phase authorizes that phase, not later phases. Follow a more specific user instruction if it changes this sequence.

1. **Understand.** Read relevant files and memory first. Separate facts, assumptions and proposals. Use the [probing guide](references/HOW-TO-USE.md#discuss-and-adapt) to ask one focused question at a time about a choice that changes the next step. Adapt to answers and record decisions, reasons and open questions as they arise. A request to understand or plan does not authorize implementation.
2. **Plan.** Map the outcome, phases and dependencies. Keep later phases provisional. Give each independently reviewable phase its own numbered concept when preparing it. Agree on the next phase's scope, approach and checks where needed. Reuse prior authorization.
3. **Implement and verify.** Work within the granted scope. When evidence materially changes behavior, architecture, scope or risk, decide within delegated authority or pause affected work for human direction. Continue unaffected authorized work.
4. **Review and learn.** Explain what changed, why and what the checks showed, including limitations. Apply feedback and update memory. At meaningful checkpoints, use the [learning loop](references/HOW-TO-USE.md#learn-and-apply-working-patterns) to review available conversation and work for durable patterns. In Manual, follow the phased-work sequence above and wait for approval before advancing; in Auto, follow the authorized review loop. Record implementation, verification, review, approval and commits separately as they occur.

## Private memory

- For substantial work, follow the [initialization guide](references/HOW-TO-USE.md#initialize-and-recover-memory) to create or reuse the primary project's private, Git-ignored `memory temp/` bundle. Give each substantial goal or coherent discussion a named folder and local index when it begins, and link it from the root index and active state. Use the bundle for shared context across repositories and record each repository's location and role. Ask if the primary project is unclear. Keep memory private unless explicitly authorized to share it.
- On a fresh session or after context loss, start with active state and the applicable working agreement and patterns. Confirm the current goal's mode, authority and phase checkpoint before acting. Consult the index and linked records as needed and reconcile stale summaries against relevant evidence. In an ongoing conversation, reuse loaded context and reread when freshness or missing evidence matters.
- Search the log for specific historical evidence rather than reading it in full by default. Read relevant sections first and expand as needed for a complete answer or review. Limit repeated or truncated tool output; updating the log does not require loading its full contents. For repeated mechanical work, follow the [context efficiency guidance](references/HOW-TO-USE.md#keep-context-useful) to reuse tools or local scripts.
- Update the detailed goal, phase or decision first, then active state, affected indexes and log. Preserve earlier decisions and reasons. Keep existing local reference copies unless migration is agreed.

## File references

Keep indexes navigational, following the [OKF profile](references/SPEC.md#private-okf-profile). Link relevant source files, phase records and evidence in plans, decisions and review notes. Use relative Markdown links within the bundle. For code across repositories, identify the repository and use a repository-relative path, adding a symbol or line when helpful. Find references before asking the user. If a necessary file cannot be located or accessed, ask for its path or link.

## References

- [Operating guide](references/HOW-TO-USE.md) — Initialize memory, work across repositories and maintain phase records.
- [OKF profile](references/SPEC.md) — Consult when format, ID reservation, provenance or recovery rules are needed.
- Starter templates — [working agreement](templates/001-working-agreement.md), [active state](templates/002-active-state.md), [working patterns](templates/003-working-patterns.md).
