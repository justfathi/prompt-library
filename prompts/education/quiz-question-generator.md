---
title: Quiz & Assessment Question Generator
industry: education
tags: [quiz, assessment, questions, multiple-choice, bloom]
contributor: justfathi
---

## Description
Generates a set of quiz or test questions at specified cognitive levels — from recall to analysis to application — with answer keys and distractor rationale for multiple-choice questions.

## Use Case
Teachers, instructional designers, and course creators who need a variety of high-quality assessment questions quickly, covering different levels of thinking for a given topic.

## The Prompt
```
You are an experienced assessment designer. Generate quiz questions for the topic and specifications below.

For each question type requested, follow these standards:

**MULTIPLE-CHOICE QUESTIONS**
- 4 answer choices (A–D)
- One clearly correct answer
- Three plausible distractors that reflect common misconceptions (not obviously wrong)
- After each question, add: "Answer: [X] — Rationale: [why this is correct + why each distractor is wrong]"

**SHORT-ANSWER QUESTIONS**
- Clear, specific question that can be answered in 2–4 sentences
- Include a model answer with the key points required for full credit

**TRUE/FALSE QUESTIONS**
- Statement is unambiguously true or false (no "it depends")
- Include the answer and a 1-sentence explanation

**ESSAY / EXTENDED RESPONSE QUESTIONS**
- Open-ended question that requires analysis, synthesis, or evaluation
- Include a scoring guide: what a full-credit response must include

Cognitive levels (Bloom's Taxonomy) — distribute questions as specified:
- Remember: recall facts, definitions, dates
- Understand: explain in own words, summarize, classify
- Apply: use knowledge in a new situation, solve a problem
- Analyze: break down, compare/contrast, identify patterns
- Evaluate: judge, justify, argue a position
- Create: design, produce, synthesize something new

---

Generate the following:
- [X] multiple-choice questions
- [X] short-answer questions
- [X] true/false questions
- [X] essay questions

Cognitive level distribution: [e.g., "40% Remember/Understand, 40% Apply/Analyze, 20% Evaluate/Create"]

Topic: [TOPIC]
Subject: [SUBJECT]
Grade level / course: [GRADE OR COURSE NAME]
Specific content to cover: [KEY CONCEPTS, CHAPTERS, OR LEARNING OBJECTIVES]
Any question types to avoid: [e.g., "no trick questions" / "avoid calculation-heavy items"]
```

## Notes
- Bloom's distribution matters: a test that's 80% recall doesn't measure real understanding — aim for at least 30% Apply/Analyze
- Multiple-choice distractors should be designed around real misconceptions, not random wrong answers — this is what separates good from bad MC questions
- For standardized test prep, add a note specifying the test format (SAT, AP, GCSE, etc.) for style alignment
- Run a separate pass asking the model to review its own questions for ambiguity before using them
