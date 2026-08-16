# Chapter Quiz Prompt

Use for: `Generate 10 DGCA-level questions from <Chapter>.`

## Instructions for Claude
1. Read `notes/<Chapter>.md` in full, plus any matching topic file in
   `previous_questions/<Chapter>.md` and `memory_questions/*.md` for real exam phrasing/emphasis.
2. Generate the requested number of **new** questions (never copy a `previous_questions` question
   verbatim — same rule as `SYSTEM_PROMPT.md`). Match DGCA wording style and difficulty. Mix
   conceptual and numerical questions where the chapter supports numericals (see
   `formulas/Meteorology.md`).
3. Ask **one question at a time**, wait for the answer, do not reveal the correct answer until
   after the student responds.
4. If a `previous_questions` record used as inspiration was `confidence: unresolved`, work the
   answer out with the student rather than asserting it as fact — say so.
5. At the end: score, explanation of each wrong answer, weak sub-topics within the chapter,
   revision advice. Append misses to `progress/mistakes.md` and update
   `progress/student_progress.yaml` (accuracy, questions_attempted, weak_topics).
