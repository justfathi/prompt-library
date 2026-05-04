---
title: Job Description Writer
industry: hr
tags: [recruiting, job-description, hiring, bias-reduction, talent]
contributor: justfathi
---

## Description
Writes a structured, inclusive job description from role requirements — covering responsibilities, qualifications, and compensation range — while flagging language likely to reduce applicant diversity.

## Use Case
Recruiters and hiring managers who need to post a new role quickly without spending hours wordsmithing, or who want a second pass on existing JDs to reduce unintentional bias.

## The Prompt
```
You are a senior recruiter writing a job description. Use the details below to produce a complete, well-structured job description. Flag any language or requirement you include that research shows reduces applicant diversity (e.g. unnecessary degree requirements, gendered phrasing, excessive "must-haves").

Role details:
- Job title: [JOB TITLE]
- Team / department: [TEAM OR DEPARTMENT]
- Reporting to: [MANAGER TITLE]
- Employment type: [FULL-TIME / PART-TIME / CONTRACT]
- Location / remote policy: [ON-SITE / REMOTE / HYBRID — LOCATION]
- Compensation range: [SALARY OR RATE RANGE, or "competitive / to be disclosed"]
- Core responsibilities (bullet points): [LIST 4–6 KEY RESPONSIBILITIES]
- Must-have qualifications: [LIST 3–5 REQUIRED SKILLS OR EXPERIENCE]
- Nice-to-have qualifications: [LIST 2–3 PREFERRED SKILLS]
- Team culture / working style: [1–2 SENTENCES DESCRIBING THE TEAM]
- Key performance indicators for this role in year one: [LIST 2–3 SUCCESS METRICS]

Produce the following sections:
1. About the role (2–3 sentences, energising but honest)
2. What you'll do (bulleted responsibilities)
3. What we're looking for (split clearly into "Required" and "Preferred")
4. What success looks like in year one
5. Compensation & benefits snapshot
6. [END OF JD]

After the JD, add a section called "Bias audit notes" listing any flagged phrases and suggested alternatives.
```

## Notes
- Remove the bias audit section before posting — it's for internal review only
- If compensation is undisclosed, instruct the model to write "Competitive, commensurate with experience" and note that transparency increases applicant quality
- Works best when you provide concrete KPIs rather than vague success descriptions
