---
title: Legal Brief & Case Summarizer
industry: legal
tags: [legal-research, brief, case-law, summary, litigation]
contributor: justfathi
---

## Description
Summarizes a legal brief, court opinion, or case document into a structured analysis — extracting the key facts, legal issues, arguments, holdings, and implications in plain language.

## Use Case
Law students, paralegals, and attorneys who need to rapidly digest a legal document, prepare a case summary for a client, or brief a colleague on a decision without reading the full text.

## The Prompt
```
You are a legal analyst. Summarize the legal document below into a structured case brief.

**CASE / DOCUMENT SUMMARY**

**Document type:** [Court opinion / Legal brief / Motion / Statute / Regulation / Other]
**Case name:** [if applicable]
**Court / Jurisdiction:** [if applicable]
**Date:** [if applicable]

---

**1. FACTS** (3–5 sentences)
[The key facts relevant to the legal issues — who did what, when, and what led to the dispute or action. Omit irrelevant background.]

**2. PROCEDURAL HISTORY** (if applicable)
[How the case got to this point — lower court decisions, appeals, remands]

**3. LEGAL ISSUES**
[The specific legal questions the court or brief is addressing — stated as questions:]
1. Whether [ISSUE 1]
2. Whether [ISSUE 2]

**4. HOLDING / CONCLUSION**
[The court's answer to each issue, or the brief's conclusion — direct and specific]

**5. REASONING**
[The legal logic and analysis — which rules, statutes, or precedents were applied and how. This is the most important section for understanding the document.]

**6. KEY RULES / TESTS ESTABLISHED**
[Any legal standard, multi-part test, or rule articulated in this document that has broader application]

**7. DISSENT / COUNTER-ARGUMENTS** (if applicable)
[Any dissenting opinion or opposing arguments raised — these often signal where the law is unsettled]

**8. PRACTICAL IMPLICATIONS**
[What does this mean in practice? Who is affected, how, and what behavior does it require or permit?]

**9. OPEN QUESTIONS**
[Any issues the document leaves unresolved or deliberately narrow — things that future cases will need to address]

---

Document to summarize:
[PASTE THE LEGAL DOCUMENT, BRIEF, OR CASE TEXT HERE]

Context (optional):
- Area of law: [CONTRACT / TORT / CONSTITUTIONAL / CRIMINAL / IP / EMPLOYMENT / OTHER]
- Why you're reading this: [e.g., "researching scope of fair use" / "advising a client on non-compete enforceability"]
- Jurisdiction context: [IF RELEVANT TO INTERPRETATION]
```

## Notes
- For very long opinions, paste the majority opinion first, then run a second pass for the dissent
- The "Practical Implications" section is the most valuable for advising clients — focus here when preparing client-facing summaries
- For statute or regulation summaries, adapt the structure: replace Holding with "Key Requirements" and Reasoning with "Legislative Intent"
- Always cite the original document — never rely solely on a summary for litigation or legal advice
