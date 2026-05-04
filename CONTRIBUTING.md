# Contributing to Open Prompt Library

Thanks for wanting to add a prompt. Here's how.

---

## Quick steps

1. Fork the repo
2. Create your prompt file in the right folder
3. Add an entry to `index.json`
4. Open a pull request

---

## Folder structure

Put your file in the matching industry folder:

```
prompts/
├── healthcare/
├── marketing/
├── coding/
├── finance/
├── education/
├── legal/
└── real-estate/
```

---

## Prompt file format

Create a `.md` file with a descriptive name, e.g. `prompts/coding/regex-explainer.md`.

```markdown
---
title: Your Prompt Title
industry: coding
tags: [tag1, tag2, tag3]
contributor: your-github-username
---

## Description
One or two sentences on what this prompt does.

## Use Case
When and why someone would use it.

## The Prompt
\```
The full prompt goes here. Use [PLACEHOLDERS] for anything the user needs to fill in.
\```

## Notes
Tips, limitations, or variations worth knowing.
```

---

## index.json entry

After adding your file, add a matching entry to `index.json`:

```json
{
  "title": "Your Prompt Title",
  "industry": "coding",
  "tags": ["tag1", "tag2", "tag3"],
  "description": "One sentence shown on the card.",
  "file": "prompts/coding/your-filename.md"
}
```

The `description` is what appears on the search card — make it specific and useful.

---

## Quality bar

- The prompt must be specific and immediately usable — not a generic template
- Use `[PLACEHOLDERS]` for anything the user needs to supply
- One prompt per file
- No duplicates — search the library before submitting
- `index.json` must be updated in the same PR as the prompt file

---

## Commit format

```
add: {industry} — {prompt title}
```

Example: `add: coding — Regex Explainer`
