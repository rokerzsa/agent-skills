---
type: Reference
title: Goal memory operating guide
description: Adaptive discussion, private memory initialization, review and recovery.
tags: [collaboration, goals, workflow]
status: draft
---

# Operating guide

## Discuss and adapt

Start with the request and what the project already shows. For a large or unclear goal, explain the relevant situation and a provisional direction. Separate current behavior from proposed design. A concrete flow or scenario can expose missing responsibilities and failure paths. Select the smallest unresolved question that changes the next decision and ask it plainly. Multiple questions are appropriate only when closely related and easy to answer together.

After each answer, acknowledge the result, update relevant memory and adapt. If the user says the whole system is confusing, inspect it and suggest a useful starting area instead of requiring them to choose a feature. Challenge material assumptions without a fixed questionnaire or repeated approval rituals. Discuss credible alternatives and trade-offs when the choice matters. Reopen affected decisions when evidence invalidates them. Preserve explicit constraints, including restrictions on tests.

Example: “The runner mixes startup and recording. I suggest starting with recording because it is a distinct block. Does that sound useful?” After agreement, inspect that block, explain a simple change and ask the next relevant question. This example's design is not a universal rule.

## Plan, implement and review

Outline the goal, major phases, dependencies and important risks. Detail the next slice: intended result, scope, approach, expected affected areas, verification and review point. Later phases are provisional. Only seek clarification or agreement that is needed and not already provided; clear instructions can authorize multiple steps.

Carry out the authorized slice, then explain the change, files, actual checks and limitations. Show the diff or a scenario if helpful. Respond to review questions, revise if requested, and document important understanding. By default wait for review before the next slice; honor explicit authorization to proceed across slices. Commit only on instruction or an explicitly authorized alternative policy. Record implementation, verification, review, approval and commit independently and truthfully.

If a material assumption fails, inspect evidence, explain the effect and discuss a recommendation before changing agreed design. Continue independent authorized work where possible. When switching goals, checkpoint current state and next action.

## Initialize and recover memory

For substantial work when the project location is known, initialize automatically if memory is absent. Preserve existing files. Where Git applies, add /memory temp/ to the root .gitignore if needed and check tracked paths. If memory is already tracked, report it; ignore rules do not untrack files.

Create memory temp/index.md and date-grouped log.md; copy references/SPEC.md and references/HOW-TO-USE.md into memory under those names; copy the three skill templates as 001-working-agreement.md, 002-active-state.md and 003-working-patterns.md. Link them from the root index and record initialization with the actual date. Do not invent project facts or approvals. Start a goal concept when useful.

At restart, read the index, agreement, active state, patterns and relevant linked documents. Check the detailed checkpoint and current evidence before resuming. Reconcile stale summaries from the detailed record. Existing project reference copies are snapshots; propose a migration and preserve local agreements rather than overwriting them automatically.

## Keep context useful

Record concise decisions, reasons, constraints, open questions, changes and verified results, not a transcript. A goal, plan and decisions may share a concept. Split only when independent retrieval or maintenance helps. Update the detailed record first, then active state and affected indexes/log. Record actual evidence when important, including what was not verified. Follow the [OKF profile](SPEC.md) for metadata, IDs and navigation.
