# DGCA-CPL Study Repo (multi-subject)

@SYSTEM_PROMPT.md

Act as described in `SYSTEM_PROMPT.md` for every session in this repo — you are the exam engine,
the student is preparing for DGCA CPL written papers.

## Active subject

**DGCA CPL — Air Regulations** is the active subject as of 2026-11-03 (set via explicit project
directive). All new question generation, quizzes, mock exams, revision notes, and progress
tracking default to Air Regulations unless the student explicitly asks for Meteorology or another
subject by name. Do not mix subjects within a single quiz/exam.

**Air Regulations currently has no source material in this repo** (no syllabus, notes, formulas,
or previous-questions bank). Do not generate Air Regulations quiz questions from memory and
present them as grounded DGCA content — see Rule 11 in `SYSTEM_PROMPT.md` and the Air Regulations
section below for what's needed and how to proceed in the meantime.

Meteorology is fully built and preserved below; switch back to it on request.

## Repo map

### Meteorology (built, has full source material)
- `syllabus/Meteorology.md` — official DGCA/CAR syllabus, §1.1–1.10
- `notes/*.md` — 16 chapter files (Atmosphere, Pressure, Wind, Thermodynamics, Clouds, Fog,
  Precipitation, Stability, Thunderstorms, Fronts, PressureSystems, JetStreams, Icing, Visibility,
  Climatology, MetInformation), each following: Definition → Classification → Formation → DGCA
  Important Facts → Frequently Tested Concepts → Numerical Problems → Memory Questions → Common
  Mistakes → Revision Summary
- `formulas/Meteorology.md` — every numeric fact/formula used across the notes, one page
- `dgca_documents/METAR_TAF.md` — METAR/TAF/SIGMET/AIRMET decode reference
- `previous_questions/*.md` (+ `INDEX.md`) — 2,167 deduped questions extracted from source PDFs,
  grouped by topic, each tagged `Confidence: verified|unresolved` (see `SYSTEM_PROMPT.md` rule 11
  — only ~14% carry a confirmed answer)
- `memory_questions/YYYY-MM.md` — dated exam-recall compilations from Telegram study groups
  (topic hints, not verified questions/wording)
- `progress/meteorology_progress.yaml`, `progress/meteorology_mistakes.md` — Meteorology's
  progress history (421 questions attempted as of 2026-08-16), preserved and untouched

### Air Regulations (active subject, source material NOT yet present)
- `syllabus/AirRegulations.md` — placeholder only; needs the official DGCA CAR Section 1/syllabus
  content this paper covers
- `notes/AirRegulations/` — placeholder folder; needs chapter files once source material exists
  (likely topics: Aircraft Rules 1937, relevant CARs, ICAO Annexes 1/2/6/8/13 as applicable,
  Chicago Convention 1944 articles — to be confirmed against the actual DGCA syllabus, not assumed)
- `previous_questions/AirRegulations/` — placeholder folder; needs a real question bank the same
  way Meteorology's was extracted from source PDFs
- `progress/airregulations_progress.yaml`, `progress/airregulations_mistakes.md` — fresh, empty,
  separate from Meteorology's progress files (see `progress/README.md`)

### Shared
- `quiz_history/` — mock-exam run logs (any subject)
- `prompts/chapter_quiz.md`, `prompts/mock_exam.md`, `prompts/revision.md` — detailed instructions
  for the three quiz modes below, subject-agnostic
- `output/` — generated revision sheets land here
- `progress/README.md` — explains the per-subject progress-file split

## Daily commands
- `Generate 10 DGCA-level questions from <Chapter>.` → `prompts/chapter_quiz.md`
- `Generate 20 mixed <Subject> questions.`
- `Start a timed 100-question DGCA mock.` → `prompts/mock_exam.md`
- `Review yesterday's mistakes.` / `Create revision notes for <Chapter>.` → `prompts/revision.md`
- `Ask only numerical questions from <Chapter>.`
- `Explain every incorrect answer in detail.`
- `Update my progress after this quiz.`
- `Switch to Meteorology.` / `Switch to Air Regulations.` — changes the active subject for this
  session; always confirm which subject a quiz command applies to if it's ambiguous.

## Provenance
Meteorology was built from `Source/` (60 PDFs, 7 exact duplicates). Extraction/parsing pipeline
lives in `../build/` (scripts + intermediate JSONL) — not part of the study repo itself, kept for
re-running if more source PDFs are added later. See `../build/PIPELINE.md` for how to extend it.
Air Regulations has no equivalent source corpus yet — the same build process should be used once
source PDFs/material are supplied, rather than hand-writing unverified content.
