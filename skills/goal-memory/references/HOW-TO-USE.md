---
type: Reference
title: Goal memory operating guide
description: Adaptive discussion, private memory initialization, review and recovery.
tags: [collaboration, goals, workflow]
status: draft
---

# Operating guide

## Discuss and adapt

Act as a design partner. Start from the request, relevant files and settled decisions. Before asking, identify what the answer would change about the outcome, scope, design or checks. Resolve factual questions by inspecting the project. Ask the user about unresolved intent, constraints or trade-offs that need their judgment.

Before a consequential question or recommendation, follow relevant memory indexes to the goal, phase, decisions and evidence, then inspect affected source files. Recheck context when an answer or finding changes the next step. State what inspection established, any material mismatch or uncertainty, and how it affects the decision.

Give just enough context to answer. Name the relevant behavior or file, explain the consequence of the choice and recommend a default when the evidence supports one. For architecture, trace one concrete scenario through the affected components and probe the first unclear boundary, such as who owns state or what happens on failure. Keep the question short. Group questions only when they are closely related and easy to answer together.

After each answer, acknowledge the result, update relevant memory and adapt. If the user says the whole system is confusing, inspect it and suggest a useful starting area instead of requiring them to choose a feature. Challenge material assumptions without a fixed questionnaire or repeated approval rituals. Discuss credible alternatives and trade-offs when the choice matters. Reopen affected decisions when evidence invalidates them. Preserve explicit constraints, including restrictions on tests.

Example: “The runner currently starts recording after startup. If recording fails, should startup still succeed?” If the user says yes, record that constraint and check how recording failures are reported. Ask a follow-up only if the existing behavior and the answer leave a material choice unresolved. Once the next step is clear, summarize the agreed scope and proceed within the authorization already given.

## Plan, implement and review

Outline the goal, major phases, dependencies and important risks. Detail the next slice: intended result, scope, approach, expected affected areas, verification and review point. Later phases are provisional. Only seek clarification or agreement that is needed and not already provided; clear instructions can authorize multiple steps.

For a substantial goal, create a separate numbered phase concept when preparing each independently reviewable phase. Link it from the goal and current state; add a phase index when several phases need navigation. Record the outcome, scope, participating repositories, dependencies, open questions, agreed decisions and reasons, implementation, verification, review, approval and commit when they occur. Update it during discussion and review. Link shared decisions instead of duplicating them. Retain earlier scope and evidence when later changes supersede them, and link the newer record.

For example, an Agent and API goal can have one phase for each side and a later integration phase. The integration record links the two dependencies and states what was actually verified together. Phase progress is separate from OKF knowledge status.

Carry out the authorized slice, then explain the change, files, actual checks and limitations. Show the diff or a scenario if helpful. Respond to review questions, revise if requested, and document important understanding. By default wait for review before the next slice; honor explicit authorization to proceed across slices. Commit only on instruction or an explicitly authorized alternative policy. Record implementation, verification, review, approval and commit independently and truthfully.

If a material assumption fails, inspect evidence and its effect. Decide within explicit delegated authority; otherwise pause affected work and discuss a recommendation. Continue independent authorized work where possible. When switching goals, checkpoint current state and next action.

## Learn and apply working patterns

At meaningful checkpoints and before handoff, consider the available conversation, decisions, reviews and work for durable patterns in how the human answers, which questions help, and how the team plans, implements and reviews. Record an explicitly stated enduring preference as confirmed with its stated scope. Keep instructions limited to a task or phase in that work's record; do not generalize them into durable preferences. Record an inferred pattern as provisional only when it recurs in comparable situations, with brief evidence and context. Ask for confirmation before treating it as binding. Do not invent evidence or inspect unavailable history. Update the pattern register and log material additions or corrections; preserve a concise amendment when a confirmed pattern changes. Continue observing a mature profile, but change it only when new evidence or a correction warrants it.

Read applicable confirmed patterns when planning, questioning and reviewing. Determine the current mode from the user's instructions, available harness state and working agreement; an active goal alone does not authorize unattended decisions or bypass review. In an explicitly authorized unattended run, use patterns to frame the questions the human typically asks, investigate answers using available evidence, and choose within delegated authority. Implement, verify, review and checkpoint each slice, then continue within that authorization. Record the rationale, evidence and agent review; never describe it as human approval. If a consequential choice exceeds delegated authority or lacks evidence, record it as open and pause affected work while continuing independent authorized work. Current instructions and the working agreement take precedence over inferred preferences.

## Initialize and recover memory

For substantial work when the project location is known, initialize automatically if memory is absent. Preserve existing files. Where Git applies, add /memory temp/ to the root .gitignore if needed and check tracked paths. If memory is already tracked, report it; ignore rules do not untrack files.

Create memory temp/index.md and date-grouped log.md; copy references/SPEC.md and references/HOW-TO-USE.md into memory under those names; copy the three skill templates as 001-working-agreement.md, 002-active-state.md and 003-working-patterns.md. Link them from the root index and record initialization with the actual date. Do not invent project facts or approvals.

When a substantial goal or coherent discussion begins, create a descriptively named folder inside memory temp/ with its own index.md and a numbered goal or discussion concept. Link the folder from the root index and the current concept from active state. Keep related phase and decision concepts in that folder, adding subfolders only when helpful. Capture understanding and open questions even when no implementation is planned. Reuse the existing folder when the work belongs to the same goal; keep shared concepts at a location accessible to all relevant goals and link them. Allocate numbered concepts using the bundle-wide counter in active state.

For an existing bundle, preserve existing files and links. Continue an existing goal in its current location unless reorganizing is appropriate; if moving concepts, preserve their numeric IDs and history and update affected links and indexes. Respect locally agreed rules and the migration guidance below.

For work across repositories, keep the shared goal, phases, decisions and indexes in the primary project's memory temp/. Record the participating repository locations and responsibilities in the goal, and identify affected repositories in each phase. Check existing memory in participating projects for relevant agreements before proceeding; preserve and link to it without silently copying private content. If the primary project is unclear, ask the human. Apply ignore and tracked-file checks to the repository containing the shared bundle.

At restart, read the index, agreement, active state, patterns and relevant linked documents. Check the detailed checkpoint and current evidence before resuming. Reconcile stale summaries from the detailed record. Existing project reference copies are snapshots; propose a migration and preserve local agreements rather than overwriting them automatically.

## Keep context useful

Record concise decisions, reasons, constraints, open questions, changes and verified results, not a transcript. Keep the overall goal and provisional plan together; use phase concepts for substantial reviewable work and separate shared decisions when independent retrieval or maintenance helps. Update the detailed record first, then active state and affected indexes/log. Record actual evidence when important, including what was not verified. Follow the [OKF profile](SPEC.md) for metadata, IDs and navigation.
