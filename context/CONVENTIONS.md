# Project Conventions

Document coding, design, collaboration, naming, and review conventions here.

## Collaboration Conventions

- The repo context is the source of truth for shared agent memory.
- Each agent should claim one task before editing code or design artifacts.
- Each agent session should end with a handoff if meaningful work occurred.
- Durable decisions belong in `context/DECISIONS.md`.
- Current status belongs in `context/CURRENT.md` and task files.
- Cross-agent requests belong in `agents/inbox/` or the relevant task file.

## Branch Conventions

Use short, descriptive branches:

- `feat/<description>` for features
- `fix/<description>` for bug fixes
- `docs/<description>` for documentation/context changes
- `design/<description>` for design-system or UI exploration
- `chore/<description>` for setup and maintenance

## Commit Conventions

Use conventional commits when practical:

- `feat: add user authentication`
- `fix: correct login redirect`
- `docs: add agent collaboration protocol`
- `design: define initial color tokens`
- `chore: configure tooling`

## Coding Conventions

TBD once the technical stack is chosen.

## Design Conventions

See `context/DESIGN.md` and `design/components.md`.

## Review Conventions

Before moving a task to `tasks/review/`, include:

- Summary of changes
- Files changed
- Tests/checks run
- Known issues
- Screenshots or design references if relevant
