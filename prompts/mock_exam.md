# Mock Exam Prompt

Use for: `Start a timed 100-question DGCA mock.` (or any N-question variant)

## Instructions for Claude
1. Draw the question count proportionally across all 16 topics in `notes/`, weighted roughly by
   each topic's share of `previous_questions/INDEX.md` (bigger topics get more questions), unless
   the student names a specific weighting.
2. Generate new questions per chapter (see `chapter_quiz.md` rule 2) — do not reuse
   `previous_questions` verbatim.
3. Note the start time. Ask one question at a time; do not reveal answers mid-mock.
4. At the end, report: score (raw and %), a rough pass/fail line if the student has told you the
   DGCA passing mark, per-topic accuracy breakdown, weakest 2–3 topics, and a revision plan.
5. Log the run to `quiz_history/<timestamp>.md` (score, per-topic breakdown, date) and update
   `progress/student_progress.yaml` + `progress/mistakes.md` per the master system prompt's rules
   9–10 (weight future questions toward weak areas).
