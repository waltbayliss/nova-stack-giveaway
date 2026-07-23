# Self Building, Self Improving Agent Stack — the real kit

This is not a set of hand-written templates. It's the real file and folder structure of 11 agents from
a live 98-agent stack — same names, same layout, same code — with all real content redacted. Secrets,
credentials, logs, and anything personal have been stripped or replaced with a placeholder explaining
what normally lives there. The shape is real. The history in it is not.

Verified with `gitleaks` and `trufflehog` before publishing — zero findings on both.

## What's in here

Eleven agents, each with the same shape:

- **nova-assistant** — the orchestrator. One voice, routes everything else.
- **agent-builder** — turns an approved idea into a working agent.
- **agent-quick-searcher** — checks if someone's already built this before I do.
- **agent-prd-reviewer** — 9-point review before a single line of code.
- **agent-code-reviewer** — the 2-pass gate. Nothing ships without independent sign-off.
- **agent-security** — PASS / WARN / BLOCK on anything new touching the stack.
- **agent-security-sweeper** — daily autonomous scan across the whole fleet.
- **agent-self-improve** — the weekly report card. Judges, ranks, proposes fixes.
- **agent-auditor** — weekly health check of the entire registry.
- **agent-health-check** — daily — is everything actually still running?
- **agent-openrouter-optimizer** — picks the right model for the job, logs every call's cost.

Every agent follows the same 8-doc structure: `CLAUDE.md` (the operating system), `docs/PRD.md`,
`ARCHITECTURE.md`, `SOUL.md`, `SECURITY.md`, `ROADMAP.md`, `DECISIONS.md`, `SPRINT_LOG.md`, and
`agent-memory.md`. Real code lives in `src/`, real playbooks in `skills/`.

## What was removed

- Every credential, API key, and hardcoded ID
- Real session logs, decision history, and memory entries (each file exists with a one-line note on
  what it's for — the log content itself is gone)
- Anything naming a real person other than me, or specific to my employer/business beyond what's
  already public in this talk

## How to use it

Pick any agent folder as a starting skeleton, or read `nova-assistant/CLAUDE.md` first — it's the root
operating system every session boots from. Fill in the bracketed placeholders. Start a session with an
AI coding assistant that reads a root memory file (Claude Code, Cursor, etc.) and it becomes your
orchestrator.

Take it. Build better agents.

— Walt Bayliss
