# DGCA-CPL Meteorology Study Repo

@SYSTEM_PROMPT.md

Act as described in `SYSTEM_PROMPT.md` for every session in this repo — you are the exam engine,
the student is preparing for the DGCA CPL Meteorology written paper.

## Repo map
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
- `progress/student_progress.yaml`, `progress/mistakes.md` — updated after every quiz/mock
- `quiz_history/` — mock-exam run logs
- `prompts/chapter_quiz.md`, `prompts/mock_exam.md`, `prompts/revision.md` — detailed instructions
  for the three quiz modes below
- `output/` — generated revision sheets land here

## Daily commands
- `Generate 10 DGCA-level questions from Clouds.` → `prompts/chapter_quiz.md`
- `Generate 20 mixed Meteorology questions.`
- `Start a timed 100-question DGCA mock.` → `prompts/mock_exam.md`
- `Review yesterday's mistakes.` / `Create revision notes for Fog.` → `prompts/revision.md`
- `Ask only numerical questions from Pressure.`
- `Explain every incorrect answer in detail.`
- `Update my progress after this quiz.`

Progress files auto-commit after every scoring interaction (`SYSTEM_PROMPT.md` Rule 12) — expect
a git commit per quiz/mock/revision session, not just on request.

## Provenance
Built from `Source/` (60 PDFs, 7 exact duplicates). Extraction/parsing pipeline lives in
`../build/` (scripts + intermediate JSONL) — not part of the study repo itself, kept for
re-running if more source PDFs are added later. See `../build/PIPELINE.md` for how to extend it.
