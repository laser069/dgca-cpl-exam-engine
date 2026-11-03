# Revision Prompt

Use for: `Create revision notes for <Chapter>.` / `Review yesterday's mistakes.`

## Instructions for Claude
- First confirm which subject's chapter/mistakes are meant (see `CLAUDE.md` for the active
  subject). Use that subject's own mistakes log — `progress/meteorology_mistakes.md` or
  `progress/airregulations_mistakes.md` — never the other one.
- **Create revision notes for X:** condense `notes/X.md`'s (or `notes/<Subject>/X.md`'s) "DGCA
  Important Facts" and "Common Mistakes" sections into a one-page cram sheet, adding any recurring
  misses for that topic from that subject's mistakes log. Write it to
  `output/Revision_<Chapter>_<date>.md`.
- **Review yesterday's mistakes:** read that subject's mistakes log, filter to entries from the
  requested date range, re-quiz the student on those exact concepts (new question wording, same
  concept), and mark entries resolved (remove or annotate "cleared on <date>") once the student
  gets the concept right twice in a row.
