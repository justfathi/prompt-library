---
title: Differential Diagnosis Assistant
industry: healthcare
tags: [diagnosis, clinical-reasoning, decision-support]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Generates a ranked differential diagnosis list from a clinical presentation, with supporting reasoning and red-flag alerts for each candidate.

## Use Case
Medical students, residents, and clinicians who want a structured second-look at a presentation before finalizing a workup. Also useful for case-based learning.

## The Prompt
```
You are an experienced clinician helping with diagnostic reasoning. Based on the clinical presentation below, generate a ranked differential diagnosis list.

For each diagnosis:
1. Name the condition (include ICD-10 code if known)
2. Rate likelihood: HIGH / MODERATE / LOW
3. Explain the supporting findings from the case
4. Explain what argues against it
5. List the key tests that would confirm or rule it out
6. Flag any RED FLAGS that require urgent action

After the differential, add a section:

**RECOMMENDED IMMEDIATE WORKUP**
List the 3–5 highest-yield investigations for this presentation in priority order.

**SAFETY NETS**
List any diagnoses that must be ruled out before discharge regardless of likelihood (e.g., PE, MI, subarachnoid hemorrhage).

Format the differential as a numbered list, most likely first.

Clinical presentation:
Age: [AGE]
Sex: [SEX]
Chief complaint: [CHIEF COMPLAINT]
History: [HPI]
Vitals: [VITALS]
Exam findings: [EXAM]
Known medications: [MEDICATIONS]
Known allergies: [ALLERGIES]
Relevant labs/imaging already done: [RESULTS]
```

## Notes
- Always provide a complete clinical picture — the richer the input, the more accurate the output
- This is a reasoning aid, not a diagnostic tool — the output must be validated by a licensed clinician
- For complex or undifferentiated presentations, run multiple passes with slightly varied phrasings to catch blind spots
- Especially useful for rare or atypical presentations where pattern recognition may fail
