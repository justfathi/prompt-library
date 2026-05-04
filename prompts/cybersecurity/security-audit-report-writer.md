---
title: Security Audit Findings Report Writer
industry: cybersecurity
tags: [security-audit, reporting, findings, executive-summary, compliance]
contributor: justfathi
---

## Description
Transforms raw security audit findings — from penetration tests, code reviews, or compliance audits — into a structured, audience-appropriate report with an executive summary, risk-rated findings, and a remediation roadmap.

## Use Case
Security engineers and consultants who have completed an audit or pentest and need to produce a professional report for technical teams and executive stakeholders, without spending days on formatting and narrative writing.

## The Prompt
```
You are a senior security consultant writing a post-audit findings report. Transform the raw findings below into a professional, dual-audience report: an executive summary for non-technical stakeholders and a detailed technical section for the engineering team.

Audit context:
- Organisation / system name: [ORGANISATION OR SYSTEM BEING AUDITED]
- Audit type: [e.g. "External penetration test", "Internal network audit", "Web application security review", "SOC 2 readiness audit", "Cloud configuration review"]
- Audit scope: [WHAT WAS TESTED — e.g. "Public-facing web app at domain.com and its API, AWS account ID 123456"]
- Audit period: [DATE RANGE]
- Auditor / team: [YOUR TEAM NAME OR "Internal security team"]
- Raw findings (paste each as a bullet or paragraph): [PASTE YOUR FINDINGS HERE — include: what was found, where, how it was discovered, and any evidence/screenshots referenced]
- Existing compensating controls (if any): [OPTIONAL]
- Compliance framework in scope: [e.g. "ISO 27001", "PCI DSS", "NIST CSF", "None"]

Produce:
1. Executive summary (1 page — what was tested, overall risk posture, top 3 concerns, recommended immediate actions)
2. Findings register — table with columns: Finding ID | Title | Severity (Critical/High/Medium/Low/Info) | CVSS score (estimate) | Affected component | Description | Evidence reference | Recommended fix | Effort to fix (Low/Medium/High)
3. Risk heat map (described in text — plot findings by likelihood vs. impact)
4. Remediation roadmap — group findings into: Immediate (0–30 days), Short-term (30–90 days), Long-term (90+ days)
5. Positive findings — what was done well (important for balanced reporting)
6. Methodology notes (brief — what testing methods were used)

Tone: professional, precise, non-alarmist. Avoid jargon in the executive summary. Use technical terminology in the findings register.
```

## Notes
- Always add a "Legal disclaimer" section before sharing externally: "This report contains sensitive security information and is intended solely for [CLIENT]. Do not distribute."
- The CVSS score estimates are approximate — use the official CVSS calculator for regulated engagements
- The "positive findings" section significantly improves client relationships and report credibility
