---
title: Canned Response Macro Generator
industry: customer-support
tags: [macros, canned-responses, templates, efficiency, helpdesk]
contributor: justfathi
---

## Description
Generates a clean, reusable canned response (macro) for a recurring support issue — with placeholder variables, tone variants, and a recommended trigger condition.

## Use Case
Support leads building or refreshing a macro library in Zendesk, Intercom, Help Scout, Freshdesk, or any helpdesk — especially when the team is repeatedly answering the same question with inconsistent quality.

## The Prompt
```
You are a customer support operations lead. Build a reusable canned response (macro) for the recurring issue below.

Output format:

**Macro name:** [Short, search-friendly internal name]

**Trigger condition:** [When an agent should reach for this macro — be specific about ticket signals: subject keywords, customer plan, ticket category, etc.]

**Variables used:**
- {{customer.first_name}}
- {{any other variables — list each with what it should resolve to}}

**Macro body — Standard tone:**
[The full reply, ready to paste into the helpdesk. Use the variable syntax above. Include a short greeting, the answer, and a clear closing. Keep under 150 words unless the topic requires more.]

**Macro body — Apologetic tone:**
[Same content but for cases where the customer has had a bad experience or has been waiting. Soften the opener, acknowledge the wait, keep the answer identical.]

**Macro body — Quick / informal tone:**
[Same content but trimmed for chat or simple how-to questions. Friendly, no formal greeting, under 60 words.]

**Do NOT use this macro when:**
- [Specific edge cases where a custom response is required — list 2–4]

**Linked resources:**
- [Help center articles, internal docs, or related macros worth attaching]

Quality rules:
- Sound human — no "Dear valued customer" or "Per our records"
- Always end with a clear next step or invitation, never a dead-end
- The three tone variants must communicate the same information — only the wrapper changes
- If the answer depends on plan, account state, or product version, surface that in the trigger condition AND remind the agent in a small italicized note at the top of the macro

Recurring issue: [DESCRIBE THE ISSUE THE MACRO SHOULD ANSWER]
Product context: [PRODUCT / FEATURE THE ISSUE RELATES TO]
Brand voice: [WARM / NEUTRAL / PLAYFUL / FORMAL — describe in 3–5 words]
Helpdesk platform: [ZENDESK / INTERCOM / HELP SCOUT / FRESHDESK / OTHER]
```

## Notes
- The three tone variants are the secret — agents pick the closest one and tweak, instead of writing from scratch
- Always include "Do NOT use this macro when" — without it, agents over-apply macros and customers feel processed
- Variables should match the syntax of the helpdesk platform (e.g. Zendesk uses `{{ticket.requester.first_name}}`, Intercom uses `{{ first_name }}` — adjust accordingly)
- Review macros every 90 days — product changes silently invalidate them
