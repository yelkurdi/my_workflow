---
name: add-doc
description: Create or update a procedure, plan, or learning document in this workflow repository from its template and maintain the section index. Use when asked to write down how to do something, document a checklist, start a project plan, or track a learning topic.
---

# Add a procedure, plan, or learning document

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root.

| Type | Folder | Template | Use for |
| --- | --- | --- | --- |
| Procedure | `procedures/` | `templates/procedure.md` | Repeatable instructions and checklists |
| Plan | `plans/` | `templates/plan.md` | Goals, milestones, and project approaches |
| Learning | `learning/` | `templates/learning.md` | Topics to study, resources, takeaways |

- Choose the type from the request; ask if it is ambiguous. Use the `add-n` skill instead for one-off observations, meetings, or decisions.
- Read the section's `README.md`, its template, and any existing document on the same topic before writing. Update an existing document rather than creating a near-duplicate.
- Ask for the content if none was supplied; do not create a document containing only placeholders. Use the user's facts; do not invent steps, milestones, deadlines, or resources. Record unknowns under `Open questions` (plans) or leave them out.
- Name the file `<folder>/<topic>.md` with a stable, lowercase, hyphenated topic and no date. Add a navigation line under the title, as in `procedures/weekly-review.md`: `[<Section>](README.md) · [Home](../README.md)`.
- Adapt the template: set `Updated` to the current local date, keep `Status` values supplied by the user (defaults: `draft` for plans, `exploring` for learning), and omit unused headings. Link bookmarks, notes, and tasks with relative links rather than copying them.
- Add a relative link and a short description under Documents in the section `README.md`, keeping entries alphabetical. Remove the initial empty-state sentence on the first addition. Avoid duplicate index entries.
- Add concrete next actions to `tasks/README.md` only when the user asks to track them, linking back to the document.
- Check that all relative links resolve. Return a link to the document and briefly describe any other updates.
