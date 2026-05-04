---
title: Threat Model Generator
industry: cybersecurity
tags: [threat-modeling, stride, security-design, appsec, architecture]
contributor: justfathi
---

## Description
Generates a structured STRIDE-based threat model for a described system or feature — identifying assets, trust boundaries, threats, mitigations, and residual risks in a format usable in design reviews.

## Use Case
Security engineers and application developers conducting threat modeling during design or pre-launch security reviews, especially when a dedicated security architect isn't available for every feature.

## The Prompt
```
You are a senior application security engineer conducting a threat model. Use the STRIDE framework (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege) to systematically identify threats for the system described below.

System description:
- System or feature name: [SYSTEM OR FEATURE NAME]
- Brief description: [2–4 SENTENCES — what it does, who uses it, what data it handles]
- Architecture components: [LIST KEY COMPONENTS, e.g. "React frontend, Node.js API, PostgreSQL DB, S3 file storage, Auth0 for authentication"]
- Data flows: [DESCRIBE HOW DATA MOVES — e.g. "User submits form → API validates → DB writes → confirmation email sent"]
- Trust boundaries: [WHERE DOES TRUST CHANGE? e.g. "Browser ↔ API boundary, API ↔ DB boundary, Third-party OAuth redirect"]
- Existing security controls: [LIST CONTROLS ALREADY IN PLACE, e.g. "JWT auth, HTTPS, input validation on API layer"]
- Compliance requirements: [e.g. "PCI-DSS", "HIPAA", "SOC 2", "None currently"]

Produce:
1. Asset inventory — what needs protecting and why
2. Trust boundary diagram (described in text — list each boundary and what crosses it)
3. STRIDE threat table — for each threat category, list: Threat description | Affected component | Likelihood (Low/Medium/High) | Impact (Low/Medium/High) | Current mitigation | Recommended mitigation | Residual risk
4. Top 5 priority findings ranked by combined likelihood × impact
5. Recommended security controls not currently in place
6. Open questions for the design team

Be specific to the described system — do not produce generic security advice.
```

## Notes
- The more precise the architecture description, the more actionable the threat model — vague input produces generic output
- Use the output as a starting point for a design review meeting, not a finished artifact
- For regulated environments (PCI, HIPAA), supplement with a compliance gap analysis prompt
