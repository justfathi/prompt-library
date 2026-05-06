---
title: Customer Persona Builder
industry: marketing
tags: [persona, segmentation, positioning, messaging, research]
contributor: justfathi
---

## Description
Builds a research-grounded customer persona from a mix of qualitative inputs — interviews, reviews, support tickets, sales call notes — with the depth needed for messaging, product, and GTM decisions, not just a poster on the wall.

## Use Case
Marketers or product teams developing positioning for a new launch, refreshing stale personas, or aligning sales and marketing around a single ICP definition before a campaign or quarterly plan.

## The Prompt
```
You are a B2B/B2C marketing strategist. Build a customer persona from the inputs below. The persona should be specific enough to drive copy decisions, channel selection, and product roadmap conversations — not a generic "Marketing Mary".

Output format:

**PERSONA NAME**
[Memorable, role-anchored. Format: "[Adjective] [Role]" — e.g. "Pragmatic Ops Manager", "Skeptical First-Time Founder". Avoid alliterative cuteness if it doesn't fit.]

**ONE-LINE SUMMARY**
[Who they are + the single problem they care most about, in one sentence.]

**DEMOGRAPHICS / FIRMOGRAPHICS**
- Role / title: [Specific titles, not categories]
- Company size: [Specific range]
- Industry: [Specific verticals]
- Geography: [Where they are]
- Tools they currently use: [Adjacent and competing tools]

**DAY IN THE LIFE**
[3–5 sentences in their voice. What does their workday look like? What's stressful? What's invisible to outsiders?]

**JOBS TO BE DONE (functional, emotional, social)**
- Functional: [What are they trying to accomplish?]
- Emotional: [What do they want to feel — or stop feeling?]
- Social: [How do they want to be perceived by their team / boss / customers?]

**BUYING TRIGGERS**
[The 2–4 events that make this persona start actively shopping for a solution. Be specific — "growing team" is not a trigger; "first hire that isn't a founder" is.]

**OBJECTIONS & CONCERNS** (ranked)
1. [Top objection — what they actually say, not the corporate version]
2. [...]

**WHERE THEY GET INFORMATION**
- Trusted sources: [Specific publications, podcasts, communities, individuals — name them]
- Channels they ignore: [Where NOT to spend marketing $]

**MESSAGING THAT WORKS**
- Words and phrases they use for their problem: [Verbatim from inputs]
- Words and phrases they reject: [Jargon, buzzwords, claims that ring false]
- Proof points they trust: [Case studies / data / peer reviews / free trial / demo]

**WHO THIS PERSONA IS NOT**
[Equally important — describe the adjacent persona this is often confused with, and the 1–2 attributes that distinguish them.]

**EVIDENCE**
For each major claim above, cite which input source supports it (e.g. "Interview #3", "Review batch #7"). Flag anything that is inference vs. direct evidence.

**CONFIDENCE LEVEL**
[High / Medium / Low] — with a 1-sentence reason. Note any gaps in the input that would meaningfully sharpen the persona.

Rules:
- Use the customer's actual language, not marketing translation
- Every section must be specific enough that a copywriter could write a headline from it
- If a section can't be supported by the input data, write "Insufficient evidence" — never invent
- Do not include made-up names, photos, or fictional bios; the persona is a research artifact, not a character

Inputs:
"""
[PASTE OR LIST INPUTS — interview notes, review excerpts, support ticket samples, sales call summaries, survey results, etc.]
"""

Product context: [WHAT YOUR PRODUCT DOES IN ONE SENTENCE]
Use of this persona: [WHO WILL USE IT AND FOR WHAT — e.g. "Sales team for cold outreach", "PMM for landing page rewrite"]
```

## Notes
- The "Who this persona is NOT" section is what makes personas usable in real decisions — without it, every decision becomes "well, it could apply to them too"
- Demand evidence citations — personas without traceable sources get ignored by sales and product
- Re-run this prompt every 6–12 months with fresh inputs; personas drift as the product and market change
- For GTM use, pair this persona with a separate "buying committee" map if selling B2B above SMB
