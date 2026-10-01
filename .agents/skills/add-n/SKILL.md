---
name: add-n
description: Capture or update a Markdown note in this workflow repository and maintain the notes index. Use when asked to add or save notes, ideas, observations, or meeting notes.
---

# Add a note

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Read `notes/README.md` and `templates/note.md` before writing.

- Use the user's content and requested title, date, and tags. Derive a concise title when omitted. Ask for the content if none was supplied; do not create an empty note.
- Create `notes/YYYY-MM-DD-topic.md` with a lowercase, hyphenated topic. Use the current local date unless another date was specified. If the filename exists, update it only when the request concerns that note; otherwise choose a distinct descriptive suffix.
- Adapt the template to the content, omitting unused headings and optional fields. Preserve uncertainties and distinguish proposals from decisions. Add source links when supplied.
- Add a relative link and a short description under Documents in `notes/README.md`, newest date first. Remove the initial empty-state sentence when adding the first note. Avoid duplicate index entries.
- Keep follow-up ideas in the note. Add items to `tasks/README.md` when the user asks to track them, linking back to the note.
- Check that the index link resolves. Return a link to the saved note and briefly describe any other updates.
