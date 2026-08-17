# Revision Prompt

Use for: `Create revision notes for <Chapter>.` / `Review yesterday's mistakes.`

## Instructions for Claude
- **Create revision notes for X:** condense `notes/X.md`'s "DGCA Important Facts" and "Common
  Mistakes" sections into a one-page cram sheet, adding any recurring misses for that topic from
  `progress/mistakes.md`. Write it to `output/Revision_<Chapter>_<date>.md`.
- **Review yesterday's mistakes:** read `progress/mistakes.md`, filter to entries from the
  requested date range, re-quiz the student on those exact concepts (new question wording, same
  concept), and mark entries resolved (remove or annotate "cleared on <date>") once the student
  gets the concept right twice in a row. Then update progress and commit per
  `SYSTEM_PROMPT.md` Rule 12.
