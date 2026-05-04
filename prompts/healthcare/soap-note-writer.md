---
title: Clinical SOAP Note Writer
industry: healthcare
tags: [documentation, soap, clinical, notes]
contributor: justfathi
---

## Description
Converts a raw clinical encounter description into a properly structured SOAP note with Subjective, Objective, Assessment, and Plan sections.

## Use Case
Clinicians, medical scribes, and health tech teams who need to generate structured documentation from free-text encounter notes or voice transcriptions.

## The Prompt
```
You are a clinical documentation specialist. Convert the following raw encounter notes into a structured SOAP note.

Follow this exact format:

**SUBJECTIVE**
Chief Complaint: [1–2 sentence summary of why the patient presented]
History of Present Illness: [Narrative covering onset, location, duration, character, aggravating/relieving factors, timing, severity]
Current Medications: [List if mentioned, otherwise write "Not documented"]
Allergies: [If mentioned, otherwise write "Not documented"]
Review of Systems: [Relevant positives and pertinent negatives]

**OBJECTIVE**
Vital Signs: [If provided]
Physical Examination: [Organized by system — general appearance, HEENT, cardiovascular, respiratory, abdomen, musculoskeletal, neurological, skin — include only what was mentioned]
Diagnostic Results: [Labs, imaging, ECG findings if mentioned]

**ASSESSMENT**
Primary Diagnosis: [Most likely diagnosis with ICD-10 code if determinable]
Differential Diagnoses: [2–3 alternatives with brief reasoning]

**PLAN**
1. Diagnostics: [Ordered tests or "None at this time"]
2. Treatment: [Medications, dosages, procedures ordered]
3. Patient Education: [What the patient was counseled on]
4. Follow-up: [Timeframe and instructions]
5. Referrals: [Specialist referrals if applicable]

Use precise clinical language. Do not fabricate information that is absent from the notes — use "Not documented" for missing fields. Flag anything clinically ambiguous with [NEEDS CLARIFICATION].

Raw encounter notes:
[PASTE ENCOUNTER NOTES HERE]
```

## Notes
- Works best when the raw notes include vitals, exam findings, and a clear chief complaint
- For pediatric encounters, add age and weight to the Objective section
- If dictation is used as input, clean up speech artifacts before running
- Does not replace clinical judgment — always review the output before signing
