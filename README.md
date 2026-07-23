# Self Building, Self Improving Agent Stack — Starter Kit

Everything from the talk. Real structure, redacted of anything specific to my own stack (paths, credentials, business specifics) — but the mechanism is exactly what runs a live 98-agent fleet today.

## What's in here

- `CLAUDE.md` — the root operating-system template. Drop this at the root of any AI-coding-assistant project and it becomes the orchestrator.
- `docs/` — the 8-doc structure every agent in the fleet uses. Copy this folder into any agent's directory as a starting skeleton.
- `agent-memory.md` — cross-session memory template.
- `skills/build-pipeline-skill/` — the full 4-stage build pipeline (prior-art research → PRD review → security pre-check → 2-pass code review), self-contained, no external dependencies. This is the real thing — install instructions are inside.
- `skills/security-bouncer.md` — the PASS/WARN/BLOCK gate for anything new touching the stack.
- `skills/self-improve.md` — the protocol every agent runs after every task.
- `skills/self-improve-loop-real-example.md` — the real weekly self-improvement architecture (adversarial judge, ELO ranking, human approval gate, auto-revert on regression), redacted but structurally faithful.

## How to use it

1. Pick any AI coding assistant that reads a root memory file (Claude Code, Cursor, etc.).
2. Drop `CLAUDE.md` and `docs/` into a new project.
3. Fill in the bracketed placeholders — your north star, your first agent's purpose.
4. Start a session. The AI reads the file and becomes your orchestrator.
5. When you want to build your first specialist agent, run the build pipeline skill.

Take it. Build better agents.

— Walt Bayliss
