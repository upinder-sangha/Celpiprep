# Status

_Last updated: 2026-11-06_

## Done
- Repo created: https://github.com/upinder-sangha/Celpiprep
- Project-continuity setup: `CLAUDE.md` plus `docs/` (STATUS, SPEC, DECISIONS)
- Permissions: `.claude/settings.json` allows all tools

## Proposed plan (awaiting owner's go-ahead)
Focus: Listening + Reading. Content must be official (Paragon) and obtained legitimately:
the free official practice tests, or tests/study material the owner buys.
Scraped or pirated dumps are out of scope (Claude won't search for or process them).

1. **Pilot:** start with the free official tests on celpip.ca. While taking each one, the owner keeps a
   private copy: screen recording with audio, plus screenshots of questions and the answer-review screen.
   This goes in the owner's private storage, never in this repo.
2. **Importer:** scripts turn those captures into structured JSON per test: audio clips cut per part
   (ffmpeg), question/option text via OCR, transcripts via local Whisper, and the answer key.
3. **App:** retake tests in a clean UI; every attempt saved; review wrong answers with transcript and
   notes; weak spots by part; score trends; mistake re-review queue.
4. **Scale up:** buy official practice-test packs and run them through the same importer.

## Next steps
- Owner confirms the plan and describes the app requirements
- Define the data model (tests → sections → parts → questions, media, transcripts, answers, attempts)

## Open questions
- Web, mobile, or both?
- Where the owner's private content library lives (Google Drive, Dropbox, local folder)
