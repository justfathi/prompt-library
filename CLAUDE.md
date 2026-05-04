# Open Prompt Library — Project Documentation

**Repo:** github.com/justfathi/prompt-library  
**Live site:** justfathi.github.io/prompt-library  

---

## Project Overview

A free, community-driven library of specialized AI prompts organized by industry. Prompts are stored as markdown files, indexed in `index.json`, and served via GitHub Pages with a searchable frontend.

---

## Folder Structure

```
prompt-library/
├── index.html              # GitHub Pages frontend
├── index.json              # Search index — must stay in sync
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
└── prompts/
    ├── healthcare/
    ├── marketing/
    ├── coding/
    ├── finance/
    ├── education/
    ├── legal/
    └── real-estate/
```

---

## Adding a Prompt

1. Create a `.md` file in the correct `/prompts/{industry}/` folder
2. Use this format:

```markdown
---
title: Prompt Title
industry: healthcare
tags: [tag1, tag2]
contributor: contributor-name
---

## Description
What this prompt does.

## Use Case
When to use it.

## The Prompt
\```
The full prompt goes here.
\```

## Notes
Any tips or limitations.
```

3. Add a corresponding entry to `index.json`

---

## index.json Format

```json
{
  "title": "Prompt Title",
  "industry": "healthcare",
  "tags": ["tag1", "tag2"],
  "description": "One sentence description.",
  "file": "prompts/healthcare/filename.md"
}
```

---

## Quality Rules

- Prompts must be specific, useful, and tested — no filler
- No duplicates
- Every prompt must have an industry tag
- Credit the original source if not original content
- Prefer prompts that work across multiple AI models

---

## Commit Conventions

- `add: {industry} — {prompt title}` for new prompts
- `fix: {what was fixed}` for corrections
- `update: index.json` when updating the search index
- `update: README` for documentation changes

---

## Communication Rules

- Commits, PR comments, and contributions must be neutral and human-readable
- No references to AI models or tools in any public-facing content
