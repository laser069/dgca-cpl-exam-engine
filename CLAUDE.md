# DGCA-CPL Study Repo

@SYSTEM_PROMPT.md

Act as described in `SYSTEM_PROMPT.md` for every session in this repo — you are the exam engine,
the student is preparing for the DGCA CPL written papers. Subjects built so far: **Air Regulations**
(current focus) and **Meteorology** (frozen earlier build). If the student doesn't name a subject, ask.

## Repo map
Subject-specific files live in a subject folder for newer subjects (`.../AirRegulations/`); the
Meteorology build keeps its original flat layout.

### Air Regulations
- `syllabus/AirRegulations.md` — DGCA Regs syllabus / road map (from the cockpitchats + DGCA syllabus PDFs)
- `notes/AirRegulations/*.md` — 13 topic files: ICAOConventions, Licensing, RegistrationAirworthiness,
  IndianRulesDGCA, RulesOfTheAir, ATSAirspace, CommunicationsRT, InstrumentProcedures, Aerodromes,
  AccidentsSAR, SecurityFacilitationDG, HumanFactors — each: Definition → Classification → Formation →
  DGCA Important Facts → Frequently Tested Concepts → Numerical Problems → Memory Questions → Common
  Mistakes → Revision Summary (facts tagged `(src: ...)`)
- `formulas/AirRegulations_KeyNumbers.md` — every key number found in the sources; `CONFLICT` marks disagreeing sources
- `previous_questions/AirRegulations/*.md` (+ `INDEX.md`) — 2,083 deduped questions by topic. Confidence:
  `derived` (1,266, model-worked answer + one-line why, NOT an official key), `unresolved` (817). **0 are `verified`.**
- `memory_questions/AirRegulations/YYYY-MM.md` — exam-recall compilations (2021-02, 2025-01, 2025-05, undated); topic hints only

### Meteorology (frozen)
- `syllabus/Meteorology.md`, `notes/*.md` (16 chapters), `formulas/Meteorology.md`,
  `dgca_documents/METAR_TAF.md`, `previous_questions/*.md` (2,167 questions, 292 verified),
  `memory_questions/YYYY-MM.md`

### Shared
- `progress/student_progress.yaml`, `progress/mistakes.md` — updated after every quiz/mock (tag entries with the subject)
- `quiz_history/` — mock-exam run logs
- `prompts/chapter_quiz.md`, `prompts/mock_exam.md`, `prompts/revision.md` — instructions for the quiz modes
- `output/` — generated revision sheets

## Daily commands
- `Generate 10 DGCA-level questions from ATSAirspace.` → `prompts/chapter_quiz.md`
- `Generate 20 mixed Air Regulations questions.`
- `Start a timed 100-question Air Regulations mock.` → `prompts/mock_exam.md`
- `Review yesterday's mistakes.` / `Create revision notes for Aerodromes.` → `prompts/revision.md`
- `Ask only numerical questions from RulesOfTheAir.`
- `Explain every incorrect answer in detail.`
- `Update my progress after this quiz.`

Progress files auto-commit after every scoring interaction (`SYSTEM_PROMPT.md` Rule 12).

## Provenance
Air Regulations built from `Source/` (101 files; 46 Air Regs files mapped, see `../REMAINING.md` for what
is not processed yet and known quality caveats). Pipeline in `../build/` (see `../build/PIPELINE.md`).
