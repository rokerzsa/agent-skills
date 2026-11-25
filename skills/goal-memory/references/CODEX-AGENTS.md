# Goal Memory roles for Codex

The canonical TOML profiles live in this repository's top-level `agents/` directory. Copy them into the target project's `.codex/agents/` or your personal `~/.codex/agents/`. These are optional Codex definitions. [Model availability](https://learn.chatgpt.com/docs/models) depends on the account and client.

## Choose the role for the current step

The main Codex session that runs `$goal-memory` is the coordinator and uses its selected model. The skill defines its coordination duties. In authorized Auto work, the coordinator invokes the installed specialists by name and relays their results and questions. Use the [mode guide](HOW-TO-USE.md#work-modes) to check authority.

| Step | Role and default | When to use it |
| --- | --- | --- |
| Coordinate the goal | Main agent | Own the conversation, scope and authority, dispatch, checkpoints, private memory and decisions on advancement. |
| Inspect and answer factual questions | Optional `goal_memory_inspector` from `agents/goal_memory_inspector.toml`, using Codex's default subagent model and effort | Trace current behavior and open questions. Reuse its evidence when answering follow-ups. |
| Challenge assumptions and review the plan | `goal_memory_reviewer` from `agents/goal_memory_reviewer.toml`, on GPT-6.2 Sol at high effort | Probe consequential assumptions during discovery when useful, then complete the independent plan review before edits in Auto. |
| Answer design questions and plan | Coordinator, with optional `goal_memory_planner` from `agents/goal_memory_planner.toml`, on GPT-6.2 Sol at medium effort | Use the inspector's findings and reviewer's questions to compare options, then propose a reviewable plan. |
| Implement and verify | `goal_memory_worker` from `agents/goal_memory_worker.toml`, on GPT-6 Luna at max effort | Use for a settled, bounded change with clear checks. |
| Implement and verify complex work | `goal_memory_complex_worker` from `agents/goal_memory_complex_worker.toml`, on GPT-6.2 Sol at medium effort | Use instead of the routine worker when diagnosis, cross-component changes or difficult integration is expected. |
| Review results and revisions | Same independent reviewer where possible | Inspect the diff and actual checks, then verify corrections. |

## How the coordinator hands off work

Give each specialist the current phase, the exact question or task, its read or write scope, relevant source and memory paths, and the expected output. Specialists return their work to the coordinator, which passes relevant results onward. Reuse the same specialist for follow-ups when practical.

1. **Discovery and planning.** The coordinator collects factual findings from the inspector when needed and uses them to shape the plan with the planner. It sends the plan and its evidence to the reviewer. Route reviewer questions about facts to the inspector and design trade-offs to the planner. The coordinator sends the answers back to the reviewer and pauses affected work if a question requires the user's judgment or approval.
2. **Implementation.** Once material plan findings are resolved and the work is authorized, the coordinator gives one worker the reviewed plan, write scope and agreed checks. The worker returns its changed paths or diff, actual check results and any unresolved issues.
3. **Review and checkpoint.** The coordinator presents the uncommitted diff and check results to the user. Obtain the user's approval to begin result review before giving the reviewer that evidence, unless the user has explicitly authorized a different review sequence for the phase. Route findings to the worker and send revisions back for re-review. Once blockers are resolved, record the evidence and apply the commit and advancement rules. On resume, use the recorded checkpoint to pick up the next pending handoff.

For example, the inspector finds that a service starts before its audit log opens. The reviewer asks what should happen if the log fails to open. The inspector can confirm current behavior and the planner can explain the trade-off. The coordinator checks the recorded requirements and delegated authority. If the desired behavior requires the user's judgment, it asks the user and pauses that change.

Choose one implementation worker per phase. If a routine change uncovers a coupled failure, have the outgoing worker finish or confirm that it has stopped editing and released the scope being transferred. Then capture the handoff diff and check results. Reassess any material plan change with the reviewer, and give the complex worker the captured diff, evidence and revised scope once authorized.

GPT-6.1 Terra is an optional fit when browser interaction or visual evidence dominates a step. If you use it regularly, set `model = "gpt-6.1-terra"` and `model_reasoning_effort = "medium"` in a copy of the appropriate role, giving the copy a distinct `name` and filename if you keep both. Codex gives a named role's pinned model and effort precedence over spawn-time values. [Model selection guide](https://learn.chatgpt.com/docs/model-selection) · [Custom agent configuration](https://learn.chatgpt.com/docs/agent-configuration/subagents#custom-agents)

If a named role or its model is unavailable, use the same role brief with an available model through the harness. Favor a stronger available model for independent review. If delegation itself is unavailable, follow the [mode guide's fallback](HOW-TO-USE.md#work-modes).
