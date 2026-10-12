---
name: add-task
description: Add, update, start, park, or complete tasks in this workflow repository's task list. Use when asked to track a to-do, next action, waiting item, or to mark a task done.
---

# Add or update a task

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Read `tasks/README.md` before writing.

- Tasks live in `tasks/README.md` under `Next`, `In progress`, `Waiting`, and `Done`. Add new tasks under `Next` unless the user indicates another status. Do not create other task files.
- Write each task as `- [ ] <action, starting with a verb>`. Append ` — due YYYY-MM-DD` only when the user gave a real deadline; never invent one. For `Waiting`, add who or what it is waiting on only when supplied, e.g. ` — waiting on <supplied party>`.
- Link supporting documents with relative links from `tasks/` (for example `[note](../notes/YYYY-MM-DD-topic.md)`) instead of copying their content. Check that each link resolves.
- Before adding, search the task list for the same action; update the existing item rather than duplicating it.
- To change status, move the item to the matching section. To complete, change `[ ]` to `[x]`, move it to `Done`, and append ` — done YYYY-MM-DD` with the current local date. Preserve the original wording and links.
- When asked to clean up, move older `Done` items to the archive with the `archive-doc` skill only if the user agrees.
- Return a link to `tasks/README.md` and the added or changed lines.
