# Chapter Quiz Prompt

Use for: `Generate 10 DGCA-level questions from <Chapter>.`

## Instructions for Claude
0. Determine the active subject (see `CLAUDE.md`) from the chapter named — if it's not clearly
   one subject's chapter, ask. **If the subject has no source material in this repo (currently
   Air Regulations), stop and follow `SYSTEM_PROMPT.md` Rule 13 instead of proceeding.**
1. Read `notes/<Chapter>.md` (or `notes/<Subject>/<Chapter>.md`) in full, plus any matching topic
   file in `previous_questions/` and `memory_questions/*.md` for real exam phrasing/emphasis.
2. Generate the requested number of **new** questions (never copy a `previous_questions` question
   verbatim — same rule as `SYSTEM_PROMPT.md`). Match DGCA wording style and difficulty. Mix
   conceptual and numerical questions where the chapter supports numericals (see that subject's
   `formulas/*.md`).
3. Ask **one question at a time**, wait for the answer, do not reveal the correct answer until
   after the student responds.
4. If a `previous_questions` record used as inspiration was `confidence: unresolved`, work the
   answer out with the student rather than asserting it as fact — say so.
5. At the end: score, explanation of each wrong answer, weak sub-topics within the chapter,
   revision advice. Append misses to that subject's mistakes log and update that subject's
   progress file only — `progress/meteorology_progress.yaml` + `progress/meteorology_mistakes.md`
   for Meteorology, `progress/airregulations_progress.yaml` +
   `progress/airregulations_mistakes.md` for Air Regulations (accuracy, questions_attempted,
   weak_topics). Never write one subject's results into the other's file.
