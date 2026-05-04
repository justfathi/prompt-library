---
title: Interview Question Builder
industry: hr
tags: [interviewing, hiring, behavioural, competency, recruiting]
contributor: justfathi
---

## Description
Generates a structured interview guide with behavioural, situational, and technical questions mapped to specific competencies for a role — including scoring guidance and follow-up probes for each question.

## Use Case
Hiring managers and recruiters building a structured interview process for a new or existing role, especially teams moving away from unstructured gut-feel interviews toward consistent, legally defensible evaluation.

## The Prompt
```
You are an organisational psychologist helping design a structured interview for a specific role. Build a complete interview guide using the STAR (Situation, Task, Action, Result) framework for behavioural questions.

Role being hired:
- Job title: [JOB TITLE]
- Seniority level: [e.g. "Individual contributor", "Team lead", "Director"]
- Key competencies to evaluate (list 4–6): [e.g. "Problem-solving, Communication, Ownership, Collaboration, Technical depth in [DOMAIN]"]
- Interview duration: [e.g. "45 minutes", "60 minutes"]
- Interview format: [e.g. "One-on-one with hiring manager", "Panel of 3 interviewers"]
- Any specific scenarios or challenges this person will face in the role: [OPTIONAL — 1–3 SENTENCES]

For each competency, produce:
1. One behavioural question (past experience — "Tell me about a time…")
2. One situational question (hypothetical — "Imagine you…")
3. Three follow-up probes to go deeper
4. What a strong answer looks like (2–3 sentences)
5. What a weak answer looks like (2–3 sentences)
6. A 1–4 scoring rubric (1 = does not meet bar, 4 = clearly exceeds bar)

End with:
- A suggested question sequence and time allocation
- Two "culture fit / working style" questions that are legally safe and not correlated with protected characteristics
- One closing question the candidate can ask (to signal what you value)
```

## Notes
- Avoid questions about gaps in employment, family status, age, or national origin — legally problematic in most jurisdictions
- The scoring rubric section is the most valuable part for calibration meetings; share it with all interviewers before the panel
- For technical roles, add a separate technical assessment prompt to complement this guide
