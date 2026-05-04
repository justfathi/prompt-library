---
title: Privacy Policy Generator
industry: legal
tags: [privacy, gdpr, ccpa, compliance, data-protection]
contributor: justfathi
---

## Description
Drafts a comprehensive, plain-language privacy policy covering GDPR, CCPA, and general best practices — based on a description of what data the product collects and how it's used.

## Use Case
Founders, product managers, and developers launching a product who need a privacy policy that's legally substantive and actually readable — not a copy-paste wall of legalese.

## The Prompt
```
You are a privacy counsel drafting a privacy policy. Using the information below, write a complete privacy policy that is legally substantive, plain-language, and covers GDPR and CCPA requirements.

The policy must include:

1. **Introduction** — who you are, what this policy covers, effective date
2. **Information We Collect** — broken into: information you provide directly, information collected automatically, information from third parties
3. **How We Use Your Information** — specific purposes with legal basis (for GDPR: consent, legitimate interest, contract performance, legal obligation)
4. **How We Share Your Information** — categories of third parties, purpose of sharing, no selling of personal data (or disclosure if you do sell)
5. **Cookies and Tracking** — what's used, why, and how to opt out
6. **Data Retention** — how long data is kept and why
7. **Your Rights** — cover: access, correction, deletion, portability, objection, restriction, opt-out of sale (CCPA), withdrawal of consent (GDPR)
8. **How to Exercise Your Rights** — specific contact method and response timeframe
9. **Data Security** — what measures are in place (be honest — don't overclaim)
10. **Children's Privacy** — COPPA compliance statement (13+ or 16+ for GDPR)
11. **International Data Transfers** — if applicable (EU → US standard clauses)
12. **Changes to This Policy** — how users will be notified
13. **Contact Us** — data controller contact details / DPO if applicable

Write in plain English. Use short paragraphs. Avoid passive voice where possible. Each section should be scannable.

---

Product details:
Product name: [PRODUCT NAME]
Company name: [COMPANY NAME]
Company location: [COUNTRY / STATE]
Product type: [Web app / Mobile app / SaaS / E-commerce / Other]
Users located in: [e.g., "US only" / "US and EU" / "Global"]
Data collected: [List everything — email, name, payment info, location, usage data, device info, etc.]
Third-party services used: [e.g., Stripe, Google Analytics, Intercom, AWS, Mailchimp — list all that touch user data]
Do you sell user data: [Yes / No]
Minimum user age: [13 / 16 / 18 / other]
Contact email for privacy requests: [EMAIL]
```

## Notes
- A generated privacy policy is a strong starting point — have it reviewed by a privacy attorney before launch if you serve EU users or handle sensitive data (health, financial, children's data)
- Be accurate about what data you actually collect — overpromising in a privacy policy creates legal liability
- GDPR requires identifying a "legal basis" for each processing activity — the prompt handles this, but verify the basis chosen matches your actual use case
- Update the policy whenever you add a new third-party service or change how you use data
