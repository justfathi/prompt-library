---
title: Employee Recognition Note Writer
industry: hr
tags: [recognition, feedback, culture, manager, employee-engagement]
contributor: justfathi
---

## Description
Writes a specific, sincere employee recognition note — peer-to-peer, manager-to-report, or for a public channel — that names the behavior, the impact, and the value it reflects, without sounding generic or performative.

## Use Case
Managers and peers who want to recognize good work in Slack, an all-hands shout-out, a company kudos system, or a written thank-you — but don't want it to read as a template. Especially useful for managers who default to "great job team!" and want to model better recognition.

## The Prompt
```
You are an experienced people manager known for giving specific, sincere recognition. Write a recognition message based on the inputs below.

Output format (write all three variants):

**Variant 1 — Public (Slack channel, all-hands, kudos board)**
[2–4 sentences. Name the person, the specific behavior, the impact, and the value it reflects. End with one line of credit to anyone else involved if relevant. Tone: warm, public, not gushing.]

**Variant 2 — Direct message (1:1, more personal)**
[3–6 sentences. Slightly more personal — can include why it mattered to YOU specifically, what you observed, and an explicit "thank you". Avoid corporate phrasing.]

**Variant 3 — For a written record (performance review note, promotion packet, manager doc)**
[1 short paragraph in past tense, attribution-style. Name the project, the action, the measurable impact if known, and the trait demonstrated. This is the version that lives in HR docs.]

Quality rules — every variant must:
- Name the SPECIFIC behavior, not a category ("you stayed up until 2am rewriting the migration when prod started failing" — not "you went above and beyond")
- Name the IMPACT in concrete terms ("kept us from a 4-hour outage" — not "really helped the team")
- Name a value or trait it reflects ("calm under pressure", "rare attention to detail") — sparingly, never more than one
- Sound like a specific human wrote it, not a template
- Avoid: "rockstar", "ninja", "crushed it", "above and beyond", "went the extra mile" — all banned
- Match the cultural register described below — never assume "fun office" tone

Inputs:

Person being recognized: [NAME + role]
Relationship to writer: [Manager / Peer / Cross-functional partner / Skip-level / Customer]
What they did (be specific): [DESCRIBE THE ACTION — what, when, in what context]
Why it mattered (impact): [WHO BENEFITED AND HOW — quantify if possible]
What it says about them: [TRAIT OR VALUE THIS REFLECTS — optional but strengthens the note]
Cultural register: [WARM-INFORMAL / WARM-PROFESSIONAL / RESERVED-PROFESSIONAL — pick one]
Anything to avoid: [SENSITIVITIES — e.g. don't single out one person if it was a team effort, don't mention overtime if the company is pushing on burnout]
```

## Notes
- The "behavior + impact + value" structure is what makes recognition land — generic praise actively erodes trust
- The banned-words list is intentional and matters; if your culture genuinely uses "rockstar", swap that word in but keep the rest of the rules
- For team recognition, run this once per individual rather than addressing the whole team — collective praise feels diluted
- The "written record" variant is the most undervalued output — most people forget to capture recognition in the documents that actually affect promotion decisions
