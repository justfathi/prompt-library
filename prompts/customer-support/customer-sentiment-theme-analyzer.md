---
title: Customer Sentiment & Theme Analyzer
industry: customer-support
tags: [voc, sentiment, themes, feedback, analytics]
contributor: justfathi
---

## Description
Analyzes a batch of support tickets, reviews, NPS comments, or chat logs and produces a structured Voice-of-Customer report with ranked themes, sentiment breakdown, and prioritized actions for product and support leadership.

## Use Case
Support managers running weekly or monthly Voice-of-Customer reviews, product teams synthesizing user feedback before a planning cycle, or CX leads building a board-ready report from a mountain of unstructured comments.

## The Prompt
```
You are a customer experience analyst. Analyze the customer feedback batch below and produce a structured Voice-of-Customer report.

Output format:

**EXECUTIVE SUMMARY (5 bullets max)**
- Overall sentiment: [Positive / Neutral / Negative / Mixed] with a 1-sentence justification
- Top 3 themes by volume
- The single most important theme by business impact
- Most surprising finding
- Recommended next action for leadership

**SENTIMENT BREAKDOWN**
- Positive: [%] — what they love
- Neutral: [%] — what they tolerate
- Negative: [%] — what frustrates them
(Estimate percentages from the sample; flag if sample is too small to be meaningful.)

**THEMES (ranked by frequency)**
For each theme, output:
1. **[Theme Name]** — [count or "%"] of mentions — Sentiment: [+ / – / mixed]
   - What customers are saying: [1–2 sentence synthesis in their voice, not yours]
   - Representative quote: "[verbatim, lightly trimmed]"
   - Likely root cause: [your best hypothesis — flag as hypothesis]
   - Recommended owner: [Product / Support / Engineering / Marketing / Pricing]
   - Suggested action: [specific, not "improve X"]

(List 5–10 themes. Combine near-duplicates.)

**EMERGING SIGNALS (low volume, high importance)**
[Themes mentioned by only a few customers but worth watching — e.g. early signal of a churn driver, mention of a competitor, regulatory concern. List 2–5.]

**WHAT'S MISSING**
[Topics you'd expect to see but didn't — also useful intel.]

**METHODOLOGY NOTES**
- Sample size: [N items analyzed]
- Time window: [START — END]
- Sentiment estimation method: [keyword + context pattern matching — flag this is approximate]
- Limitations: [list 2–3]

Rules:
- Use the customer's words, not corporate paraphrase
- Distinguish observation from interpretation — never blend them
- Ignore pleasantries ("thanks!", "love you guys") unless they cluster around a specific feature
- Flag any theme that could indicate a security, legal, or safety risk at the top of the report

Source type: [SUPPORT TICKETS / NPS COMMENTS / APP STORE REVIEWS / CHAT LOGS / SURVEY / MIXED]
Time window: [DATE RANGE]
Product context: [WHAT YOUR PRODUCT DOES IN ONE SENTENCE]

Feedback batch:
"""
[PASTE OR LIST THE COMMENTS, ONE PER LINE OR SEPARATED BY ===]
"""
```

## Notes
- Quality scales with batch size — under 30 items, treat themes as directional, not statistical
- Always include the verbatim quote per theme — paraphrase loses the emotional signal product teams need
- "What's missing" is often more valuable than what's there — surfaces blind spots
- For ongoing use, keep the categorization stable across runs so you can track theme volume over time
