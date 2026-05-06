---
title: Escalation Handoff Note Writer
industry: customer-support
tags: [escalation, handoff, internal-notes, tier-2, communication]
contributor: justfathi
---

## Description
Turns a messy ticket history into a tight, structured escalation note for the next agent, engineer, or manager — so they can pick up the case in under two minutes without re-reading the entire thread.

## Use Case
Tier 1 agents handing off to Tier 2 or engineering, weekend shifts handing off to weekday teams, or any case being escalated to a manager. Eliminates the "re-explain everything" tax on the customer.

## The Prompt
```
You are a senior customer support agent writing an internal escalation note. Read the full ticket history below and produce a handoff note that lets the next person resolve the case without re-reading the thread.

Output format:

**ESCALATION SUMMARY**

**Customer:** [Name, plan, account age, any VIP / risk flags]

**Issue in one sentence:** [State it as the customer would, not as the agent]

**What's actually happening (technical / business reality):**
[2–4 sentences explaining the underlying cause as best understood. Distinguish "confirmed" from "suspected" facts.]

**Timeline of contacts:**
- [Date — who, what was tried, what the customer said]
- [Date — ...]
(Keep to bullets. Compress duplicate exchanges.)

**What's been tried and ruled out:**
- [Action — outcome]
- [Action — outcome]

**What needs to happen next:**
[Specific ask of the next owner. Use the format: "Please [verb] so that [outcome]." If unsure, say "Recommend [option A] OR [option B] — agent's call."]

**Customer emotional state:** [Calm / Frustrated / Escalating / Threatening churn / Threatening public complaint] — with a one-line reason.

**Risk if we don't resolve in 24h:** [Churn / Refund request / Public complaint / Legal / None significant]

**Internal context the next person should know:**
- [Anything not in the ticket — Slack threads, related incidents, prior similar tickets, account quirks]

**Suggested response tone for next reply:** [Apologetic / Direct / Solution-focused / Empathetic + firm]

Rules:
- Write for someone who has never seen this ticket
- Be specific about facts; flag assumptions clearly with "Assumed:" or "Unverified:"
- Do not pad. If a section has no content, write "None."

Ticket history:
"""
[PASTE FULL TICKET HISTORY — all messages from customer and agents, in order]
"""

Additional internal context (Slack, related tickets, account notes):
"""
[PASTE OR WRITE "None"]
"""
```

## Notes
- The "What's been tried and ruled out" section is the highest-leverage part — it prevents the next agent from repeating troubleshooting the customer already endured
- "Customer emotional state" + "Risk if we don't resolve in 24h" lets a manager prioritize a queue of escalations in seconds
- Keep this as a true internal note — never paste into a customer-facing reply
- If the ticket is over 20 messages long, ask the model to also output a "Compressed customer view" the next agent can quote back to confirm understanding
