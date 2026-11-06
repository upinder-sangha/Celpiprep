# celpiprep — instructions for Claude

An app for practicing the CELPIP test (Canadian English proficiency exam).

## The repo is the only source of truth

The owner works on this project from several Claude accounts and sessions.
Nothing about the project may live only in a session, a Claude account or the cloud environment.

- **Don't** keep project knowledge in Claude memory, claude.ai Artifacts, Claude Docs, or chat history.
  If it matters, write it into this repo.
- **Don't** rely on account-specific environment settings (secrets, setup scripts, env vars) without
  documenting them here. Required env vars go in `.env.example` (names and descriptions, never real values).
- Real secrets never get committed. List them in `.env.example` and say in `docs/STATUS.md` where to get them.

## Autonomy

The owner has given standing permission to act without asking: run any command, install packages,
edit or create any file, commit and push to `main`, and make reasonable technical choices
(record them in `docs/DECISIONS.md`). Just do the work and report what was done.
Only stop to ask before actions that destroy work and can't be undone, such as force-pushing,
rewriting git history, deleting the repo or its branches, or wiping data.

## Start of every session

1. Read `docs/STATUS.md`: where things stand and what's next.
2. Read `docs/SPEC.md` for what the app should do, and `docs/DECISIONS.md` before changing anything already decided.
3. Run `git pull` first, since another session or account may have pushed.

## End of every chunk of work

1. Update `docs/STATUS.md`: what was done, what's in progress, next steps, open questions.
2. Record any new decision (stack, structure, product choices) in `docs/DECISIONS.md`.
3. Commit and push. Work that isn't pushed is lost when the session ends.

## Docs

| File | Purpose |
|------|---------|
| `docs/STATUS.md` | Current state + next steps (the handoff note) |
| `docs/SPEC.md` | Product requirements: features, CELPIP sections, UX |
| `docs/DECISIONS.md` | Dated log of decisions and why |
