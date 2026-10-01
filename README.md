# My workflow

A home for workflow documentation, useful links, and work in progress. Start here to find or capture information.

## Sections

| Section | What belongs here |
| --- | --- |
| [Inbox](inbox/README.md) | Quick captures to sort later |
| [Tasks](tasks/README.md) | Next actions, work in progress, and waiting items |
| [Notes](notes/README.md) | Observations, meeting notes, ideas, and decisions |
| [Bookmarks](bookmarks/README.md) | Useful links organized by category |
| [Procedures](procedures/README.md) | Repeatable instructions and checklists |
| [Plans](plans/README.md) | Goals, milestones, and project approaches |
| [Learning](learning/README.md) | Topics to study, resources, and takeaways |
| [Archive](archive/README.md) | Completed or retired material worth keeping |

## Everyday use

- Capture quickly in the inbox when the destination is unclear.
- Keep next actions in Tasks and link to the relevant note, procedure, or plan.
- Use a [template](templates/README.md) when creating a longer document, then add a link to its section index.
- Use the [weekly review](procedures/weekly-review.md) to sort captures, refresh tasks, and archive completed work.

## Finding information

Use your editor's repository-wide search, or run these commands from the repository root if ripgrep (`rg`) is installed:

```bash
# Search all Markdown content, ignoring case.
rg -n -i 'search phrase' -g '*.md'

# Find a saved bookmark by hostname or part of its URL.
rg -n -F 'example.com' bookmarks/

# Find open tasks.
rg -n -- '- \[ \]' tasks/
```

## Conventions

Use Markdown and relative links between files. Use lowercase, hyphenated filenames; date notes as `YYYY-MM-DD-topic.md`. Give procedures, plans, and learning documents stable topic names. Dates use `YYYY-MM-DD`. Optional tags are plain text, such as `ibm, computing`.

Bookmark categories follow folders, starting with [IBM/internal/computing](bookmarks/IBM/internal/computing/README.md) and [IBM/internal/processes](bookmarks/IBM/internal/processes/README.md). Add categories as needed.

## Assistant shortcuts

Repository skills are in [.agents/skills](.agents/skills). Example requests:

- `$add-n Capture a note about today's planning discussion: …`
- `$add-bm Save https://example.com in IBM/internal/computing with the title Example resource.`

The examples are prompts, not saved content. See [add-n](.agents/skills/add-n/SKILL.md) and [add-bm](.agents/skills/add-bm/SKILL.md) for their conventions. Repository skill placement follows the [official Codex documentation](https://developers.openai.com/codex/skills/).
