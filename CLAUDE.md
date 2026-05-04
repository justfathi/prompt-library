# Open Prompt Library — Project Documentation

**Repo:** github.com/justfathi/prompt-library  
**Live site:** justfathi.github.io/prompt-library

---

## Project Overview

A free, community-driven library of specialized AI prompts organized by industry. Prompts are stored as markdown files, indexed in `index.json`, and served via GitHub Pages with a searchable frontend. Clicking a prompt opens a modal showing the full description, use case, prompt text, and notes — with a one-click copy button.

---

## Folder Structure

```
prompt-library/
├── index.html              # GitHub Pages frontend — search, filter, modal
├── index.json              # Search index — must stay in sync with prompts/
├── LIBRARY_SUMMARY.md      # Auto-updated snapshot of all prompts — update after every session
├── CONTRIBUTING.md         # Contributor guide
├── README.md
├── LICENSE
├── .nojekyll               # Prevents GitHub Pages from running Jekyll (required for raw .md serving)
├── grow.md                 # (gitignored) Agent prompt for growing the library
└── prompts/
    ├── healthcare/
    ├── marketing/
    ├── coding/
    ├── finance/
    ├── education/
    ├── legal/
    ├── real-estate/
    └── {new-industry}/     # Add new folders as new industries are introduced
```

---

## Current State

Check `LIBRARY_SUMMARY.md` for the up-to-date list of all industries and prompts. Always read it before adding anything to avoid duplicates.

**Current industries:** healthcare, marketing, coding, finance, education, legal, real-estate  
**Current prompt count:** 35 (5 per industry)

---

## Adding a Prompt

1. Check `LIBRARY_SUMMARY.md` — confirm it doesn't already exist
2. Create a `.md` file in `/prompts/{industry}/{descriptive-filename}.md`
3. Use this exact format:

```markdown
---
title: Prompt Title
industry: healthcare
tags: [tag1, tag2, tag3]
contributor: justfathi
---

## Description
One or two sentences on what this prompt does.

## Use Case
Who uses it and when.

## The Prompt
\```
The full prompt goes here. Use [PLACEHOLDERS] for anything the user fills in.
\```

## Notes
- Tip or limitation
- Another tip
```

4. Add a matching entry to `index.json` immediately
5. Validate JSON is still valid
6. Commit
7. Update `LIBRARY_SUMMARY.md`

---

## index.json Format

```json
{
  "title": "Prompt Title",
  "industry": "healthcare",
  "tags": ["tag1", "tag2"],
  "description": "One sentence shown on the search card — make it specific.",
  "file": "prompts/healthcare/filename.md"
}
```

`index.json` is the source of truth for the frontend. If a prompt isn't in `index.json` it won't appear on the site.

---

## Adding a New Industry

When adding a prompt for an industry that doesn't exist yet:

1. Create the folder: `prompts/{new-industry}/`
2. Add the industry to the `meta` object in `index.html`:
```javascript
'new-industry': { label: 'Industry Name', e: '🔧' }
```
3. Add a badge color in the `<style>` block of `index.html`:
```css
.badge-new-industry { background: #f0f9ff; color: #0284c7; }
```
4. Proceed with writing prompts and updating `index.json` as normal

---

## How the Frontend Works

- `index.html` fetches `index.json` on load and renders all prompt cards
- Clicking a card opens a modal that fetches the `.md` file directly
- The modal parses the markdown to extract: Description, Use Case, The Prompt (from inside the code block), and Notes
- The Copy button copies only the prompt text (the code block content)
- `.nojekyll` is required — without it GitHub Pages runs Jekyll and the `.md` files are not served as raw text, breaking the modal fetch

**Do not modify `index.html`** unless you are:
- Adding a new industry to the `meta` object and badge styles
- Fixing a clear bug

---

## Quality Rules

- Every prompt must be specific and immediately usable — no generic filler
- Use `[PLACEHOLDERS]` for anything the user needs to supply
- No duplicates — check `LIBRARY_SUMMARY.md` first
- Prompts must work in any capable LLM, not just one model
- The `## The Prompt` section must contain the prompt inside a fenced code block — the frontend parser depends on this

---

## Commit Conventions

- `add: {industry} — {prompt title}` for new prompts
- `fix: {what was fixed}` for bug fixes
- `update: LIBRARY_SUMMARY` when updating the summary
- `update: {filename}` for documentation changes

**Never mention authors, tools, AI models, or any name in commit messages.**

---

## After Every Session

Always end a session by updating `LIBRARY_SUMMARY.md` with the new prompt count, any new industries, and all new prompt titles. Commit it as the final step. This keeps the next session from having to scan the whole repo.
