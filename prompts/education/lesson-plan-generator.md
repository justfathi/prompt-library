---
title: Lesson Plan Generator
industry: education
tags: [lesson-plan, curriculum, teaching, classroom, k12]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Generates a detailed, standards-aligned lesson plan for any subject and grade level — including learning objectives, materials, step-by-step activities, differentiation strategies, and assessment methods.

## Use Case
Teachers, instructional designers, and curriculum developers who need a ready-to-use lesson plan quickly, or who want a strong first draft to customize.

## The Prompt
```
You are an experienced curriculum designer. Create a complete lesson plan for the topic and grade level below.

**LESSON PLAN**

**Topic:** [TOPIC]
**Subject:** [SUBJECT]
**Grade Level:** [GRADE]
**Duration:** [e.g., 45 minutes / 90-minute block]
**Standards Alignment:** [e.g., Common Core, NGSS, state standard code — or leave blank]

---

**LEARNING OBJECTIVES**
By the end of this lesson, students will be able to:
1. [Objective — use Bloom's Taxonomy action verbs: analyze, evaluate, create, apply, explain, identify]
2.
3.

**MATERIALS NEEDED**
- [List all materials, technology, handouts, manipulatives]

---

**LESSON STRUCTURE**

**HOOK / WARM-UP** (5–10 min)
[An engaging opening that activates prior knowledge or creates curiosity — a question, quick demo, short video, or discussion prompt. Explain why this hook connects to the lesson.]

**DIRECT INSTRUCTION** (10–15 min)
[Key content to teach — broken into clear steps. Include specific examples, visuals, or analogies to use. Note any common misconceptions to address explicitly.]

**GUIDED PRACTICE** (10–15 min)
[An activity where students practice with teacher support — worked examples, think-alouds, partner work. Include the specific task and what to look for to check understanding.]

**INDEPENDENT / GROUP PRACTICE** (10–15 min)
[Task students complete on their own or in groups to demonstrate understanding. Be specific about the activity and the expected output.]

**CLOSURE** (5 min)
[How to wrap up and consolidate learning — exit ticket question, think-pair-share, or a quick reflection prompt. Include the specific question or task.]

---

**DIFFERENTIATION**
- For students who need support: [Specific scaffolds — sentence frames, visual aids, reduced complexity, partner pairing]
- For students who need extension: [Specific challenge — deeper question, independent research task, creative application]
- ELL supports: [Vocabulary pre-teaching, visual supports, native language resources if applicable]

**FORMATIVE ASSESSMENT**
[How will you know if students got it during the lesson? Name the specific check — exit ticket, observation checklist, whiteboard response, etc.]

**HOMEWORK / FOLLOW-UP** (optional)
[Brief assignment that reinforces the lesson — or "None"]

---

Lesson details:
Topic: [TOPIC]
Subject: [SUBJECT]
Grade level: [GRADE]
Duration: [LENGTH]
Prior knowledge students have: [WHAT THEY ALREADY KNOW]
Standards to address (optional): [STANDARD CODES OR FRAMEWORK]
Any constraints (no tech, specific format, etc.): [CONSTRAINTS]
```

## Notes
- The hook is the most important part for engagement — don't skip or rush it
- Bloom's Taxonomy verbs matter for objectives: "understand" is not measurable; "explain in their own words" is
- For multi-day units, run this prompt for each lesson with a note about what came before and after
- Pair with the Rubric Builder and Quiz Question Generator prompts for a full instructional package
