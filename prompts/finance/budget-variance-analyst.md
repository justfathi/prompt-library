---
title: Budget Variance Analyst
industry: finance
tags: [budgeting, variance, fp-and-a, reporting, analysis]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Analyzes actual vs. budget (or prior period) financial data, explains the root causes of each significant variance, and produces a concise management commentary ready for a finance review.

## Use Case
FP&A analysts, finance managers, and CFOs who need to prepare monthly or quarterly budget variance commentary — explaining the numbers in plain language for management or board consumption.

## The Prompt
```
You are a financial planning and analysis (FP&A) specialist. Analyze the variance data below and produce a structured management commentary.

**BUDGET VARIANCE ANALYSIS**
Period: [MONTH/QUARTER] | Entity/Department: [SCOPE]

---

**1. EXECUTIVE SUMMARY** (3–4 sentences)
[High-level performance against budget — the one paragraph a CFO reads before the detail. Lead with the net result, then the 2–3 biggest drivers. Be direct.]

**2. REVENUE VARIANCE**
| Line Item | Budget | Actual | $ Variance | % Variance |
|-----------|--------|--------|------------|------------|
| [Revenue stream 1] | | | | |
| [Revenue stream 2] | | | | |
| **Total Revenue** | | | | |

Root cause analysis:
- Favorable variances: [SPECIFIC EXPLANATION — volume vs. price vs. mix, not "revenue was higher"]
- Unfavorable variances: [SPECIFIC EXPLANATION]
- One-time items: [ANYTHING NON-RECURRING THAT DISTORTS THE COMPARISON]

**3. EXPENSE VARIANCE**
| Line Item | Budget | Actual | $ Variance | % Variance |
|-----------|--------|--------|------------|------------|
| [Expense category 1] | | | | |
| [Expense category 2] | | | | |
| **Total Expenses** | | | | |

Root cause analysis:
- Favorable variances: [EXPLANATION]
- Unfavorable variances: [EXPLANATION]
- Timing differences: [ANY SPEND THAT SHIFTED PERIODS]

**4. KEY METRICS**
| Metric | Budget | Actual | Commentary |
|--------|--------|--------|------------|
| Gross margin % | | | |
| Operating margin % | | | |
| [Sector-specific KPI] | | | |

**5. RISKS AND OPPORTUNITIES**
Risks to remainder of year: [2–3 specific items that could cause further negative variance]
Opportunities: [2–3 specific items that could drive outperformance]

**6. MANAGEMENT ACTIONS**
[What corrective actions are planned or underway for unfavorable variances?]

**7. FORECAST UPDATE**
[Has the full-year or next quarter forecast changed based on this period's actuals? By how much and why?]

---

Variance data to analyze:
[PASTE YOUR ACTUAL VS. BUDGET TABLE OR DATA HERE]

Context:
- Period: [MONTH/QUARTER AND YEAR]
- Department or entity: [SCOPE]
- Known one-time items: [ANYTHING UNUSUAL THIS PERIOD]
- Key business events this period: [LAUNCHES, HEADCOUNT CHANGES, MARKET EVENTS, ETC.]
```

## Notes
- Always separate volume/price/mix effects in revenue variance — "revenue was $500K above budget" is not commentary, it's a number
- Timing differences should be called out explicitly — shifted spend shouldn't distort the recurring performance picture
- For board reporting, the Executive Summary is all most members will read — make it standalone
- Flag any variances that will recur vs. those that are one-time
