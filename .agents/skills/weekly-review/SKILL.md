---
name: weekly-review
description: Guide the user through the weekly review in this workflow repository - sort the inbox, refresh tasks, check plans, consolidate learning, and archive stale material. Use when asked to run a weekly review, triage the inbox, or reset the workflow.
---

# Run the weekly review

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Follow `procedures/weekly-review.md`; it is the source of truth for the steps, so reread it each time.

- Start with a short summary: inbox captures, open tasks by section, active plans, and items in `Done`. Use the search commands in `README.md`.
- Work through the steps in order and propose a destination for each inbox item and each change. Apply changes only after the user confirms; ask when a destination or status is unclear rather than guessing.
- File items with the matching skill: `add-n` for notes, `add-bm` for links, `add-task` for actions, `add-doc` for procedures, plans, and learning, and `archive-doc` for retired material. Remove each inbox line only after its item has been filed.
- Do not invent priorities, deadlines, or decisions; record what the user states.
- When the user wants review notes, save them with `add-n` as `notes/YYYY-MM-DD-weekly-review.md`.
- Finish with a summary of what was filed, changed, and archived, and anything left open. Skip steps the user wants to skip, and say so in the summary.
