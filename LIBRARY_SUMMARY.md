# Library Summary

Auto-updated snapshot of the current library state. Update this file whenever prompts are added.

**Total prompts:** 53  
**Industries:** 10  
**Last updated:** 2026-05-06

---

## Existing Industries & Prompts

### Healthcare (5)
- Clinical SOAP Note Writer
- Differential Diagnosis Assistant
- Patient Education Explainer
- Prior Authorization Letter Writer
- Hospital Discharge Summary Generator

### Marketing (6)
- High-Converting Ad Copy Generator
- Email Drip Sequence Writer
- Brand Voice Extractor & Style Guide Builder
- SEO Content Brief Writer
- Product Launch Announcement Pack
- Customer Persona Builder

### Coding (6)
- Code Review Assistant
- Unit Test Generator
- Bug Root Cause Explainer
- API Documentation Writer
- SQL Query Optimizer
- Refactoring Plan Builder

### Finance (5)
- Investment Thesis Writer
- Earnings Call Analyzer
- Budget Variance Analyst
- Personal Financial Plan Builder
- Financial Report Summarizer

### Education (5)
- Lesson Plan Generator
- Rubric Builder
- Student Feedback Writer
- Quiz & Assessment Question Generator
- Socratic Tutor

### Legal (5)
- Contract Clause Explainer
- NDA Drafter
- Privacy Policy Generator
- Legal Brief & Case Summarizer
- Terms of Service Red Flag Reviewer

### Real Estate (5)
- Property Listing Description Writer
- Comparative Market Analysis (CMA) Summary Writer
- Real Estate Offer Letter Drafter
- Lease Clause Reviewer
- Neighborhood Profile Writer

### HR (6)
- Job Description Writer
- Performance Review Generator
- Interview Question Builder
- Employee Onboarding Plan Builder
- HR Policy Drafter
- Employee Recognition Note Writer

### Cybersecurity (5)
- Threat Model Generator
- Incident Response Runbook Writer
- Security Audit Findings Report Writer
- Vulnerability Disclosure Email Writer
- Security Awareness Training Scenario Builder

### Customer Support (5)
- Support Ticket Response Drafter
- Canned Response Macro Generator
- Escalation Handoff Note Writer
- Customer Sentiment & Theme Analyzer
- Knowledge Base Article Writer

---

## Prompt File Conventions

- Location: `prompts/{industry}/{descriptive-filename}.md`
- Frontmatter fields: `title`, `industry`, `tags`, `contributor`
- Sections: Description, Use Case, The Prompt (inside a code block), Notes
- index.json fields: `title`, `industry`, `tags`, `description`, `file`

## Commit Convention

`add: {industry} — {prompt title}`

## Industry Slug Convention

Folder names use lowercase kebab-case: `real-estate`, `healthcare`, etc.  
New industries must also be added to the `meta` object in `index.html`.
