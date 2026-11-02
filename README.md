# Agent Skills

Reusable skills for AI coding agents.

## Skills

- [goal-memory](skills/goal-memory/SKILL.md) — Work through substantial goals with focused questions, private project context, and small reviewable steps.

## Install

Copy the entire `skills/goal-memory` directory into your agent's skills directory. For Codex, use `~/.codex/skills/goal-memory/` for a personal installation, or the project's `.agents/skills/goal-memory/` for a project installation. Keep `SKILL.md`, `references/`, and `templates/` together.

Invoke the skill as `$goal-memory` in a supported agent. The skill can also be selected automatically when appropriate; selection depends on the agent and its configuration.

For substantial goals, the skill creates a private `memory temp/` directory in the project. Its Git ignore rule does not remove already tracked files or protect against deletion. Review the skill before using it in your own workflow.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Contributions are accepted under the [MIT License](LICENSE).
