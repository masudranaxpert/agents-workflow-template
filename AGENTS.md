# AGENTS.md

## Project
<1-2 line: what this project is, and its stack>

## Commands (source of truth)
- Install: `<cmd>`
- Dev: `<cmd>`
- Test: `<cmd>`
- Lint/typecheck: `<cmd>`
- Build: `<cmd>`

## Code rules
- <naming, folder structure, style conventions>
- Follow existing patterns; ask before adding a new dependency.

## Boundaries
- Never: touch secrets/.env, generated files, or edit existing migrations.
- Ask first: DB schema, public API, dependency changes.

## Docs (.agents/)
Start by reading `.agents/INDEX.md`. Read other files only when relevant.
- `architecture.md`: stack, structure, technical decisions and reasons
- `design.md`: UI/UX, flows, loading/error/empty states
- `plans/`: overall plan + per-task plans with checklist and verification
- `research/`: temporary findings from code inspection (include date)
- `sessions/<YYYY-MM-DD-topic>/HANDOFF.md`: unfinished work, git state, next steps

## Workflow
**Small change** (1-2 files, clear bug/typo): just do it, run checks, done.

**Meaningful change** (3+ files, new feature, or architecture/DB/API impact):
1. Inspect relevant code; save findings in `.agents/research/<feature>/research.md`.
2. Write `.agents/plans/<task>.md` (requirements, scope, acceptance criteria, steps).
3. Get user approval (skip if scope and approach are already approved).
4. Implement, run checks, tick the checklist and record passed/failed/not-run.
5. Update `architecture.md` / `design.md` if their decisions changed.
6. If work is unfinished, write `HANDOFF.md` and link it from `INDEX.md`.

## Rules
- Code and Git state beat docs. If they disagree, trust the code and fix or flag the doc.
- Never invent requirements, commands, or technical decisions. Write "unknown" instead.
- Keep each fact in one place; link instead of duplicating.
- Keep `INDEX.md` short: links only, details live in plans.
- Create documents only when needed.
- Never put secrets or credentials in any file.
