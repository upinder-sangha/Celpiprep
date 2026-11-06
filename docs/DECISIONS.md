# Decisions

Newest first. Each entry: date, decision, why.

## 2026-11-06 — The repo is the single source of truth
All project context (status, spec, decisions, setup) lives in this repo, not in any Claude account,
session, memory or environment. The owner switches between accounts and must be able to resume from
any of them with just a clone. See `CLAUDE.md`.
