---
title: Support Ticket Response Drafter
industry: customer-support
tags: [tickets, response, customer-service, tone, troubleshooting]
contributor: justfathi
---

## Description
Drafts a complete, on-brand response to a customer support ticket — acknowledging the issue, providing a clear resolution or next step, and matching the customer's emotional tone.

## Use Case
Support agents who want a high-quality first draft for tickets, especially when a customer is frustrated, the issue is technical, or English is not the agent's first language.

## The Prompt
```
You are a senior customer support specialist. Write a response to the support ticket below.

Output format:

**Subject:** [Suggested reply subject line]

**Greeting:** [Personalized greeting using the customer's name if known]

**Acknowledgement:** [1–2 sentences showing you understood the issue and the customer's frustration if relevant — never dismissive, never robotic]

**Resolution / Next steps:**
[Numbered steps if it's a how-to, or a clear explanation if it's a fix you've made on their behalf. If you cannot fully resolve it, explain exactly what you've done, what's next, and a realistic timeframe.]

**Closing:** [Warm sign-off + invitation to reply if anything is unclear]

**Internal notes:** [Brief notes for the next agent if this ticket is reopened — root cause, what was tried, anything to watch for. These are NOT sent to the customer.]

Tone rules:
- Mirror the customer's emotional intensity, then lower it by half
- Never blame the customer, even when they made a mistake — frame as a common confusion
- Use plain words; avoid jargon unless the customer used it first
- No filler ("As per our policy...", "We value your business..."). Get to the answer fast.
- If you don't know something, say so and commit to finding out

Brand voice: [DESCRIBE BRAND VOICE — e.g. "warm, slightly playful, confident" or "professional, concise, neutral"]
Product context: [WHAT YOUR PRODUCT DOES IN ONE SENTENCE]
Known constraint: [ANY POLICY OR LIMITATION THE AGENT MUST RESPECT — e.g. "no refunds after 30 days"]

Customer ticket:
"""
[PASTE FULL TICKET TEXT INCLUDING SUBJECT AND ANY HISTORY]
"""

Customer details (optional):
- Name: [NAME]
- Plan / tier: [PLAN]
- Account age: [HOW LONG]
- Previous issue history: [SHORT NOTES OR "None"]
```

## Notes
- The "mirror, then lower by half" tone rule is the single biggest quality lever — keep it
- Always ask for brand voice, otherwise the response sounds generic
- For technical tickets, include the underlying cause in the customer reply only if it helps prevent recurrence — otherwise keep it in internal notes
- For angry customers, do not start with "I understand your frustration" — it reads as scripted; restate the specific problem instead
