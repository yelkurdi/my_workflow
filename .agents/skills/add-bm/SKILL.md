---
name: add-bm
description: Save or organize bookmark URLs in this workflow repository using categorized Markdown pages. Use when asked to add, save, or categorize a bookmark or web link.
---

# Add a bookmark

Locate the repository through its root `AGENTS.md` and `README.md`; all paths below are relative to that root. Read `bookmarks/README.md`, the relevant category page, and `templates/bookmark.md` before writing.

- Require a supplied URL. Use the user's title and description; when absent, use a descriptive title inferable from the URL, or the hostname as a fallback. Omit unknown descriptions rather than claiming to have read the page. Fetching a page is optional and is not needed to save an internal link.
- Follow an explicit category. Existing categories start with `IBM/internal/computing` for infrastructure, developer environments, and technical tools, and `IBM/internal/processes` for organizational workflows and administrative procedures. Preserve this capitalization in paths. Do not infer that a link is IBM-internal solely because these categories exist.
- Infer a category only when the supplied context makes it clear. Otherwise ask which category to use. For a requested new category, create `bookmarks/<category>/README.md` and any missing parent indexes, with relative navigation links. Add the category to `bookmarks/README.md` and its parent indexes.
- Search existing bookmark files for the URL before adding it. Preserve query strings and fragments, since they can identify different resources. If already present, enrich the existing entry with supplied information; move it and remove the old entry if recategorization was requested. Do not silently create duplicates across categories.
- Append the adapted bookmark template under Links on the category page. Use the current local date for Added unless specified otherwise; preserve the original date when updating an entry. Omit unused fields. Remove the initial empty-state sentence on the first addition.
- Check relative navigation links and preserve the exact supplied URL. Return a link to the category page and state whether the bookmark was added, updated, moved, or already present.
