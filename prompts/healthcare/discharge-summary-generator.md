---
title: Hospital Discharge Summary Generator
industry: healthcare
tags: [documentation, discharge, inpatient, handoff]
contributor: justfathi
---

## Description
Generates a structured hospital discharge summary from admission notes, progress notes, and discharge details — ready for the primary care provider handoff.

## Use Case
Hospitalists, residents, and medical scribes who need to produce a complete, organized discharge summary that communicates key information to the receiving outpatient provider.

## The Prompt
```
You are a clinical documentation specialist. Generate a complete hospital discharge summary from the information provided below.

Use this structure:

**DISCHARGE SUMMARY**

Patient: [NAME] | DOB: [DOB] | MRN: [MRN]
Admission Date: [DATE] | Discharge Date: [DATE]
Attending Physician: [NAME] | Service: [SERVICE]
Discharge Disposition: [Home / SNF / Rehab / Other]

---

**ADMISSION DIAGNOSIS**
[Primary reason for admission]

**FINAL DIAGNOSES**
Primary: [Final primary diagnosis + ICD-10]
Secondary: [Comorbidities active during this admission]
Complications: [Any complications during stay, or "None"]

**REASON FOR ADMISSION**
[2–3 sentence narrative of why the patient was admitted, how they presented]

**HOSPITAL COURSE**
[Chronological narrative of what happened during the admission: key interventions, response to treatment, complications managed, consultations obtained, procedures performed]

**PROCEDURES PERFORMED**
[Bulleted list with dates, or "None"]

**SIGNIFICANT RESULTS**
[Key lab values, imaging findings, pathology — focus on results that changed management or require follow-up]

**CONDITION AT DISCHARGE**
[Stable / Improved / Guarded — brief functional status note]

**DISCHARGE MEDICATIONS**
[Full medication list with dose, frequency, route — flag NEW medications and CHANGED doses with asterisks]

**MEDICATIONS STOPPED**
[List medications discontinued and reason]

**DISCHARGE INSTRUCTIONS**
[Activity restrictions, diet, wound care, or other specific instructions given to patient]

**FOLLOW-UP**
[Specific appointments scheduled — provider, date, purpose]
[Labs or imaging to be done outpatient — specify who orders and when]

**PENDING RESULTS AT DISCHARGE**
[Any results not yet back at time of discharge — include who is responsible for follow-up]

**FOR THE PRIMARY CARE PROVIDER**
[Highlighted action items and things to watch: medication changes requiring monitoring, unresolved issues, specialist recommendations to action]

---

Do not fabricate details not provided. Use "Not documented" for missing fields. Flag any pending items that require provider action with [ACTION NEEDED].

Clinical information to summarize:
[PASTE ADMISSION NOTES / PROGRESS NOTES / DISCHARGE DETAILS HERE]
```

## Notes
- The "For the Primary Care Provider" section is the highest-value part — make it specific and actionable
- Pending results at discharge are a major patient safety risk; always flag these explicitly
- For patients discharged to SNF or rehab, add a functional status section with mobility, ADL, and cognitive baseline
- Medication reconciliation at discharge is a Joint Commission requirement — flag new and changed medications clearly
