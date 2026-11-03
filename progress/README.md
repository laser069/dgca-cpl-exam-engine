# Progress tracking — subject separation

As of 2026-11-03 this repo tracks two subjects separately. Each has its own progress file and
mistakes log; nothing is shared or merged between them.

| Subject | Progress file | Mistakes log | Status |
|---|---|---|---|
| Meteorology | `meteorology_progress.yaml` | `meteorology_mistakes.md` | Active history: 421 questions attempted, accuracy 0.79, last updated 2026-08-16. |
| Air Regulations | `airregulations_progress.yaml` | `airregulations_mistakes.md` | Empty — no quiz has been run. **No source material exists yet for this subject** (see `../README.md` / session notes for what's needed: official syllabus, Aircraft Rules 1937, relevant CARs/ICAO Annexes, previous-question compilations). |

When running a quiz, update only the progress file for the subject that quiz covered. Do not let
Meteorology's history influence Air Regulations weak-topic detection, accuracy, or revision
queues, or vice versa.
