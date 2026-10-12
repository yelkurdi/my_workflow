---
name: add-inbox
description: Quickly capture a rough thought, link, or reminder in the inbox of this workflow repository for later sorting. Use when asked to jot down, capture, or "inbox" something whose destination is unclear.
---

# Add an inbox capture

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Read `inbox/README.md` before writing.

- Ask for the content if none was supplied. Keep the user's wording; shorten only to fit one line, and do not add interpretation.
- When the destination is clear, such as a URL to save, a note, or a task, suggest the matching skill (`add-bm`, `add-n`, `add-task`) instead, unless the user explicitly asked for the inbox.
- Append one line per capture at the end of the file using the format in the file's comment: `- YYYY-MM-DD — item`. Use the current local date unless another date was specified. Keep supplied URLs exact.
- Remove the `No captures yet.` sentence on the first capture. Keep the format comment.
- Return a link to `inbox/README.md` and the captured line.
