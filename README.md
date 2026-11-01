# DGCA CPL — Study Repo (Air Regulations + Meteorology)

A markdown knowledge base for Claude Code to run as a DGCA CPL examiner: chapter quizzes, timed
mocks, mistake tracking, revision sheets. See `CLAUDE.md` for the repo map and `SYSTEM_PROMPT.md`
for the examiner rules.

## Quick start
Open Claude Code in this folder (`DGCA-CPL/`) and type a command, e.g.:
```
Generate 10 DGCA-level questions from ATSAirspace.
```
`CLAUDE.md` auto-loads `SYSTEM_PROMPT.md`.

## Subjects
- **Air Regulations** (rebuilt 2026-11-01 from the new `Source/`): 13 topics, 2,083 deduped questions.
- **Meteorology** (earlier build, frozen — its question PDFs are no longer in `Source/`).
- Other subjects: not built yet. See `../REMAINING.md` for the backlog and the onboarding checklist.

## Answer-key coverage — read before trusting a number (Air Regulations)
| Confidence | Count | Meaning |
|---|---|---|
| verified / matched | 0 | no parsed source carries a printed answer key |
| derived | 1,266 | answer worked out by a model; mostly from its own ICAO/DGCA knowledge, only lightly checked against the textbooks; one-line `Why` |
| unresolved | 817 | no answer yet (model wasn't ≥~85% sure, or the question is garbled) |

`derived` ≠ official key. Some source banks are non-Indian (JAR/EASA, Malaysian), so a few answers may
differ from DGCA CAR / Aircraft Rules 1937 — the notes + CAR win. Real keys may exist in the scanned
`SK Reg QB Solved` / `Air Reg Solved Bali 2021` PDFs (OCR running; not parsed yet).

## Known gaps
See `../REMAINING.md` (unprocessed files, OCR backlog, topic-tag quality, `images/` empty, no end-to-end session test).
