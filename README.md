# DGCA CPL Meteorology — Study Repo

A markdown knowledge base for Claude Code to run as a DGCA CPL Meteorology examiner: chapter
quizzes, timed mocks, mistake tracking, revision sheets. See `CLAUDE.md` for the repo map and
`SYSTEM_PROMPT.md` for the examiner behaviour rules.

## Quick start
Open Claude Code in this folder (`DGCA-CPL/`) and type a command, e.g.:
```
Generate 10 DGCA-level questions from Clouds.
```
`CLAUDE.md` auto-loads `SYSTEM_PROMPT.md`, so no manual setup is needed each session.

## Where this came from
Built from `../Source/` — 60 DGCA Meteorology PDFs (IC Joshi, Aviator's Library, cockpitchats,
ria mam, ECQB dumps, exam-recall lists, ~295 MB). Pipeline and provenance details:
`../build/PIPELINE.md`.

## Answer-key coverage — read this before trusting a number
Of the **2,167** deduped previous-exam questions in `previous_questions/`, only **292 (~13%)**
carry a confirmed answer, matched from two real answer keys found in the source material
(`METEOROLOGY EXAM 265 04.pdf`'s inline `Answer : X` key, and `METEOROLOGY previous DGCA QUES.pdf`
+ `SK Met Answers.pdf`'s `Ans. x` key). The remaining ~87% are tagged `Confidence: unresolved` —
**no answer key exists for them anywhere in Source/**. They are real, correctly-transcribed
*questions*; their listed correctness is not verified.

This was a deliberate scope call, not an oversight: cross-matching real keys was done in full;
mass-generating ~1,875 answers by LLM guess was **not** done upfront, to avoid quietly shipping a
large batch of unverified "facts" with no way to tell them apart from the real ones. `notes/*.md`
chapter content was written from grounded aviation-meteorology knowledge, not from the unresolved
question pool, so it does not inherit this risk — but any `previous_questions`/`memory_questions`
entry without a `verified` tag should be treated as a study prompt, not an answer key, until you
work it out (`SYSTEM_PROMPT.md` rule 11 tells Claude to do this openly, not silently).

To resolve more: ask Claude to work through a topic's `unresolved` questions with you directly
(cheapest — happens naturally during a chapter quiz), or re-run `build/scripts/05_answers.py`
(not yet written — see `build/PIPELINE.md`) for a batch LLM pass if you want the whole bank
answered up front.

## Known gaps
- `Source/Nav Feb 2025 @cockpitchats.pdf` is Navigation, not Meteorology — left unprocessed.
- Two low-quality scanned/garbled sources (`Met_Question_Bank.pdf`, `Meteorology 818
  questions.pdf`) were excluded from structured parsing (space-stripped/OCR-garbled text, too
  error-prone to auto-parse reliably) — raw text still sits in `../build/raw_text/` if you want to
  hand-clean them later.
- `Latest Meteorology IC JOSHI (1).pdf` (309-page scanned textbook) was OCR'd for its notes prose;
  its printed answer-key tables came out column-scrambled by OCR and were not usable as an answer
  source.
