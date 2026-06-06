# Agentic Collaboration Template

A lightweight repository template for human + AI-agent collaboration across multiple PCs and optional mobile review.

The core idea: **raw agent sessions are local working memory; repo files are shared durable memory.** Agents should distill their progress, decisions, task state, and handoffs into this repository so another human or agent can resume from any device.

## What This Template Provides

```text
AGENTS.md                 # Operating protocol for agents
context/                  # Durable project context and decision logs
tasks/                    # Backlog, active, blocked, review, and done task files
handoffs/                 # End-of-session handoff summaries
agents/                   # Agent registry, status, and inboxes
design/                   # Design tokens and component notes
scripts/                  # Copy/paste agent startup and shutdown prompts
```

## How to Start a New Project From This Template

1. Create a fresh repository from this template.
2. Open the new repository locally.
3. Start an agent session and paste `scripts/agent-startup.md`.
4. Fill in:
   - `context/PROJECT.md`
   - `context/CURRENT.md`
   - `context/DESIGN.md`
   - `context/ARCHITECTURE.md`
   - `agents/registry.md`
5. Create the first real task from `tasks/TEMPLATE.md`.
6. Have every agent follow `AGENTS.md`.

## Daily / Session Loop

```text
Read shared context
→ Claim one task
→ Work on one branch/worktree
→ Update task progress
→ Record durable decisions
→ Write handoff before stopping
```

## Source-of-Truth Hierarchy

1. Code, tests, design tokens, schemas, and committed artifacts
2. `context/DECISIONS.md`, `context/CONVENTIONS.md`, `context/ARCHITECTURE.md`, `context/DESIGN.md`
3. Task files in `tasks/`
4. Handoffs in `handoffs/`
5. Local agent session history

## Notes

This template is intentionally tool-agnostic. It works with Hermes, Claude Code, Codex, Cursor, Copilot, or any other agentic coding/design assistant as long as each agent writes distilled state back into the repo.
