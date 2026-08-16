# DGCA CPL Meteorology Exam Engine — User Manual
*Generated 2026-08-16*

## What this is
A self-contained study repo that turns Claude into a personal DGCA CPL Meteorology examiner. It
generates fresh, DGCA-style questions (never copy-pasted from memory banks), quizzes you one
question at a time, tracks your accuracy and weak topics across sessions, and produces revision
sheets on demand — all backed by 16 chapter note files, a formula sheet, 2,167 deduped past
questions, and dated exam-recall compilations.

## How Claude behaves in this repo (the rules)
Set once in `SYSTEM_PROMPT.md`, applied every session:
1. Questions are newly written, never copied verbatim from `previous_questions/` or
   `memory_questions/`.
2. Wording and difficulty match real DGCA style.
3. Conceptual understanding is prioritised; numericals included where the topic supports them.
4. **One question at a time** — you answer before the next is shown.
5. Answers are withheld until the quiz ends.
6. Every quiz ends with: score, explanations for wrong answers, weak topics, revision advice,
   difficulty analysis.
7. Your performance is written back to `progress/student_progress.yaml` after every quiz.
8. Weak areas get proportionally more questions in future quizzes.
9. **Confidence honesty (Rule 11):** `previous_questions/` and `memory_questions/` entries are
   tagged `verified` (matched to a real DGCA answer key) or `unresolved` (~86% of the bank — no
   confirmed answer exists). When an `unresolved` question inspires a new quiz question, the
   answer is worked out from first principles and flagged as such — never presented as an
   official DGCA key.

## The three quiz modes

| You say | Claude does | Instructions in |
|---|---|---|
| `Generate 10 DGCA-level questions from <Chapter>.` | Reads that chapter's notes + past questions, asks N new questions on it | `prompts/chapter_quiz.md` |
| `Generate 20 mixed Meteorology questions.` | Same, but draws across all 16 chapters | (chapter_quiz logic, mixed scope) |
| `Start a timed 100-question DGCA mock.` | Full mock exam, questions weighted by each topic's real-world share of the question bank, logged with a timestamp | `prompts/mock_exam.md` |
| `Create revision notes for <Chapter>.` | One-page cram sheet from that chapter's key facts + your own recurring mistakes, saved to `output/` | `prompts/revision.md` |
| `Review yesterday's mistakes.` | Re-quizzes you on exactly the concepts you got wrong recently (new wording), clears them once you get each right twice in a row | `prompts/revision.md` |

You can also narrow any of these: *"Ask only numerical questions from Pressure,"* *"Explain every
incorrect answer in detail,"* *"Update my progress after this quiz."*

## Repo map — where things live

| Path | Contents |
|---|---|
| `syllabus/Meteorology.md` | Official DGCA/CAR syllabus (§1.1–1.10) |
| `notes/*.md` | 16 chapter files — Atmosphere, Pressure, Wind, Thermodynamics, Clouds, Fog, Precipitation, Stability, Thunderstorms, Fronts, PressureSystems, JetStreams, Icing, Visibility, Climatology, MetInformation. Each follows: Definition → Classification → Formation → DGCA Important Facts → Frequently Tested Concepts → Numerical Problems → Memory Questions → Common Mistakes → Revision Summary |
| `formulas/Meteorology.md` | Every numeric fact/formula used across the notes, one page |
| `dgca_documents/METAR_TAF.md` | METAR/TAF/SIGMET/AIRMET decode reference |
| `previous_questions/*.md` (+ `INDEX.md`) | 2,167 deduped real questions, grouped by topic, each tagged `verified`/`unresolved` |
| `memory_questions/YYYY-MM.md` | Dated exam-recall compilations from Telegram study groups (topic hints, not verified wording) |
| `progress/student_progress.yaml` | Your running accuracy, strong/weak topics, per-session history |
| `progress/mistakes.md` | Every wrong answer, with the question, your answer, correct answer, why, and a recurrence counter |
| `quiz_history/` | Timestamped mock-exam run logs |
| `prompts/*.md` | The instructions above, in full |
| `output/` | Generated revision sheets and this manual land here |

## How progress tracking works
- After every quiz, `progress/student_progress.yaml` is updated: cumulative accuracy, a running
  list of strong/weak topics, and a per-session history entry.
- Every wrong answer also gets an entry in `progress/mistakes.md` — if the same concept is missed
  again later, the entry is marked as recurring with a count, so persistent gaps stand out.
- Weak topics feed back into future quizzes: chapters/concepts you've missed more than once get
  weighted more heavily when you ask for new questions.

## Typical session flow
```
1. "Generate 10 DGCA-level questions from Clouds."
   → Claude asks Q1, you answer, Q2, you answer... through Q10.
   → Claude reveals score, per-question explanations, weak sub-topics, revision advice.
   → progress/student_progress.yaml and progress/mistakes.md are updated automatically.

2. "Create revision notes for Clouds."
   → One-page cram sheet written to output/Revision_Clouds_<date>.md, including your
     personal recurring misses on that chapter.

3. Next day: "Review yesterday's mistakes."
   → Re-quizzed only on what you got wrong, with new wording.
```

## Notes on the source material
Built from 60 source PDFs (7 exact duplicates removed). The extraction/parsing pipeline lives
outside this repo in `../build/` (kept only for re-running if more PDFs are added) — see
`../build/PIPELINE.md`. Only about 14% of `previous_questions/` entries carry a confirmed DGCA
answer key (`verified`); the rest are `unresolved`, meaning Claude reasons out the answer from
`notes/` and `formulas/Meteorology.md` rather than asserting a source-confirmed value — see Rule 11
above.
