# Decision Log

Record durable project decisions here. Keep entries concise and link to related task/handoff files when useful.

## Template

```md
### YYYY-MM-DD — Decision Title

**Decision:** What was decided.

**Rationale:** Why this choice was made.

**Alternatives considered:** Optional.

**Affected files/areas:** Optional.

**Related:** Optional links to tasks, handoffs, commits, issues, or design references.
```

## Decisions

### 2026-06-06 — Use repo-based context as shared agent memory

**Decision:** Shared project context, task state, handoffs, and decisions will live as Markdown/JSON files in the repository.

**Rationale:** Raw agent sessions are local, noisy, and tool-specific. Distilled repo context is portable across devices, humans, and agent instances.

**Affected files/areas:** `AGENTS.md`, `context/`, `tasks/`, `handoffs/`, `agents/`.
