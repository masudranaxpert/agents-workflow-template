# agents-workflow-template

A lightweight, drop-in documentation workflow for coding agents (Codex, Cursor, Claude Code, etc.).

## What's inside

```
AGENTS.md              # agent instructions (commands, rules, workflow)
.agents/
├── INDEX.md           # short entry point: links + active task
├── architecture.md    # stack, structure, decisions
├── design.md          # UI/UX and states
├── plans/             # overall plan + per-task plans
├── research/          # temporary code-inspection findings
└── sessions/          # local handoffs (gitignored)
```

## Use it

1. Copy `AGENTS.md`, the `.gitignore` entries and `.agents/` into your project.
2. Fill in the **Commands**, **Code rules** and **Boundaries** sections of `AGENTS.md`.
3. Let the agent create docs only when needed.

## Principles

- Progressive disclosure: start at `INDEX.md`, read more only when relevant.
- Code is the source of truth; docs are verified against it.
- Small changes skip the ceremony; meaningful changes get research, a plan and approval.
