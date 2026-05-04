---
title: Performance Review Generator
industry: hr
tags: [performance-review, feedback, hr, management, employee-development]
contributor: justfathi
---

## Description
Converts a manager's raw bullet-point notes about an employee into a complete, balanced performance review — with rated sections, specific examples, and a forward-looking development plan.

## Use Case
Managers preparing annual or mid-year reviews who have observations and examples but struggle to translate them into structured, fair written evaluations within the allotted review window.

## The Prompt
```
You are an experienced HR business partner helping a manager write a fair, specific, and constructive performance review. Use the inputs below to produce a complete review document.

Employee context:
- Employee name (or use initials): [NAME OR INITIALS]
- Role / level: [JOB TITLE AND LEVEL, e.g. "Senior Software Engineer L4"]
- Review period: [e.g. "Jan–Dec 2025" or "H1 2025"]
- Manager's raw notes — strengths: [PASTE BULLET POINTS ON WHAT WENT WELL]
- Manager's raw notes — areas for growth: [PASTE BULLET POINTS ON WHAT NEEDS IMPROVEMENT]
- Key projects or contributions this period: [LIST 2–4 NOTABLE PROJECTS OR ACHIEVEMENTS]
- Any specific incidents (positive or negative) to reference: [OPTIONAL — PASTE DETAILS]
- Agreed goals for next period: [LIST 2–3 GOALS IF KNOWN, OR LEAVE BLANK]

Performance rating scale: [e.g. "1–5 where 1=Does Not Meet, 3=Meets, 5=Exceeds" — OR describe your company's scale]

Produce these sections:
1. Overall performance summary (3–4 sentences)
2. Core competency ratings — rate and explain each: [LIST YOUR COMPANY'S COMPETENCIES, e.g. "Execution, Collaboration, Communication, Growth Mindset"]
3. Notable contributions this period (2–3 paragraphs with specific examples)
4. Areas for development (honest, specific, non-punitive — 2–3 areas)
5. Development plan for next period (goals, actions, support needed, timeline)
6. Overall rating with brief justification

Tone: direct, specific, fair. Avoid vague praise ("great team player") — anchor every claim to a concrete example from the inputs.
```

## Notes
- Replace generic compliments with the specific examples from your notes before running — vague input produces vague output
- HR teams can use this as a calibration draft; managers should personalise before submitting
- If the review is for a difficult conversation, ask the model to produce a separate "manager talking points" section
