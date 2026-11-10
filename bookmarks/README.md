# Bookmarks

[Home](../README.md)

Store links in the most specific category. Each entry has a linked title, a short description when known, and an added date. Tags are optional. Search for an existing URL before adding it again.

## Categories

- [IBM](IBM/README.md)
  - [Internal](IBM/internal/README.md)
    - [Computing](IBM/internal/computing/README.md) — infrastructure, development environments, and technical tools.
    - [Processes](IBM/internal/processes/README.md) — organizational workflows and administrative procedures.
    - [Coding agents](IBM/internal/coding_agents/README.md)
      - [Claude](IBM/internal/coding_agents/claude/README.md)
    - [IT](IBM/internal/IT/README.md)
    - [Research](IBM/internal/research/README.md)
- [Media](media/README.md)
  - [YouTube](media/youtube/README.md)
    - [Commentary](media/youtube/commentary/README.md)
    - [Education](media/youtube/education/README.md)
    - [News](media/youtube/news/README.md)
- [News](news/README.md)
  - [Tech](news/tech/README.md)

## Structure

Each category is a folder whose `README.md` holds its links.

```
bookmarks/
├── README.md
├── IBM/
│   ├── README.md
│   └── internal/
│       ├── README.md
│       ├── computing/
│       ├── processes/
│       ├── coding_agents/
│       │   └── claude/
│       ├── IT/
│       └── research/
├── media/
│   ├── README.md
│   └── youtube/
│       ├── commentary/
│       ├── education/
│       └── news/
└── news/
    ├── README.md
    └── tech/
```

Use the [bookmark template](../templates/bookmark.md) for new entries. Add new category links here and in their parent indexes.
