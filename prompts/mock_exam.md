# Mock Exam Prompt

Use for: `Start a timed 100-question DGCA mock.` (or any N-question variant)

## Instructions for Claude
0. Confirm the active subject (see `CLAUDE.md`) before drawing any questions — a mock must cover
   one subject only, never a mix. **If that subject has no source material in this repo
   (currently Air Regulations), stop and follow `SYSTEM_PROMPT.md` Rule 13 instead of proceeding.**
1. Draw the question count proportionally across that subject's chapters in `notes/` (or
   `notes/<Subject>/`), weighted roughly by each topic's share of that subject's
   `previous_questions/INDEX.md` (bigger topics get more questions), unless the student names a
   specific weighting.
2. Generate new questions per chapter (see `chapter_quiz.md` rule 2) — do not reuse
   `previous_questions` verbatim.
3. Note the start time. Ask one question at a time; do not reveal answers mid-mock.
4. At the end, report: score (raw and %), a rough pass/fail line if the student has told you the
   DGCA passing mark, per-topic accuracy breakdown, weakest 2–3 topics, and a revision plan.
5. Log the run to `quiz_history/<timestamp>.md` (score, per-topic breakdown, date, subject) and
   update that subject's own progress file + mistakes log only
   (`progress/meteorology_progress.yaml`/`meteorology_mistakes.md` or
   `progress/airregulations_progress.yaml`/`airregulations_mistakes.md`) per the master system
   prompt's rules 9–10 (weight future questions toward weak areas, using only that subject's
   history).
