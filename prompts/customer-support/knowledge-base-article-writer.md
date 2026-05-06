---
title: Knowledge Base Article Writer
industry: customer-support
tags: [knowledge-base, help-center, documentation, self-service, deflection]
contributor: justfathi
---

## Description
Writes a complete, scannable knowledge base article from a recurring support topic — structured for search, deflection, and the user actually solving the problem on the first try.

## Use Case
Support agents converting a high-volume ticket pattern into a help center article, or KB managers building or refreshing self-service content to deflect tickets and improve search ranking.

## The Prompt
```
You are a knowledge base writer for a SaaS product. Write a help center article for the topic below.

Output format:

**Title:** [Short, action- or question-oriented. Match how customers would search. Examples: "How to reset your password", "Why is my export failing?", "Connecting Slack to [Product]"]

**URL slug suggestion:** [kebab-case, 4–6 words max]

**Meta description (for SEO):** [120–155 characters. Include the core search phrase + the outcome.]

**Quick answer (for users in a hurry):**
[1–3 sentences resolving the most common case. If the user only reads this, they should be able to act.]

**Article body:**

## [H2 — what this article covers]
[1–2 sentences: who this is for, what they'll be able to do after.]

## Before you start
- [Prerequisite 1]
- [Prerequisite 2]
(Skip this section if there are no prerequisites.)

## Step-by-step
1. **[Action]** — [Specific instruction, including what to click, what to type, what to expect]
   ![screenshot placeholder: brief description of what the screenshot should show]
2. **[Action]** — [...]
3. **[Action]** — [...]

(Keep steps atomic — one verb per step. Use bold for the action, then explanation.)

## What you should see
[Describe the success state in plain language so users can self-confirm.]

## Common issues
- **[Symptom]** — [Cause + fix in 1–2 sentences]
- **[Symptom]** — [Cause + fix in 1–2 sentences]

## Still need help?
[1 sentence with a link to contact support, formatted as: "If this didn't work, [contact our support team](URL) and include [specific info that will help us help you]."]

**Suggested tags:** [3–6 tags for KB filtering]
**Related articles:** [2–4 article titles to cross-link]
**Internal review notes:** [Anything the writer should verify with a PM or engineer before publishing]

Rules:
- Write at an 8th–9th grade reading level — short sentences, common words
- Never assume the reader knows internal product names; explain on first use
- Use second person ("you"), present tense, active voice
- Screenshots are placeholders — describe exactly what the screenshot must show, including UI state
- Do not include marketing language or feature pitches — this is a help article, not a landing page
- Include error messages verbatim where applicable so users searching the error find the article

Topic: [WHAT THE ARTICLE SHOULD COVER — e.g. "How to set up SSO with Okta"]
Product: [PRODUCT NAME + ONE-SENTENCE DESCRIPTION]
Audience: [END USERS / ADMINS / DEVELOPERS / MIXED]
Common ticket signal: [WHAT CUSTOMERS TYPE WHEN THEY HIT THIS — e.g. "SSO not working", "can't log in with Okta"]
Edge cases to cover: [LIST ANY KNOWN GOTCHAS OR SAY "AGENT WILL ADD"]
```

## Notes
- The "Quick answer" section is what most readers will use — invest in making it actually resolve the most common case
- Match the article title to the search phrase, not internal terminology — search ranking depends on it
- Screenshot placeholders are gold for designers/writers picking up the article — don't skip them
- For multi-platform features (web vs mobile vs API), write separate articles rather than one with tabs — search and deflection both improve
