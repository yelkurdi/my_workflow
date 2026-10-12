---
name: archive-doc
description: Move a completed or retired document, or completed tasks, into the archive of this workflow repository and repair links and indexes. Use when asked to archive, retire, or put away finished material.
---

# Archive a document

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Read `archive/README.md` and the document to archive before changing anything.

- Archive only what the user named. Ask before archiving anything inferred to be stale. Do not delete content.
- Move the file to `archive/<original-section>/<filename>` (for example `notes/2026-01-05-topic.md` → `archive/notes/2026-01-05-topic.md`), using `git mv` when the file is tracked. Create the subfolder if needed.
- Fix relative links inside the moved file for its new depth, including its navigation line (for example `../README.md` becomes `../../README.md`).
- Search the repository for links to the old path (`rg -n -F '<filename>' -g '*.md'`). Remove the entry from the original section index, and update other links to point to the archived path.
- Add an entry under Documents in `archive/README.md`, newest first: `- [<Title>](<original-section>/<filename>) — archived YYYY-MM-DD; <reason, when supplied>`. Use the current local date. Remove the empty-state sentence on the first entry.
- For completed tasks, move the `- [x]` lines from `Done` in `tasks/README.md` to a `## Tasks` heading in `archive/README.md`, keeping their wording and links (adjusted to resolve from `archive/`).
- Check that all changed links resolve. Return a link to the archived document and list the indexes and links updated.
