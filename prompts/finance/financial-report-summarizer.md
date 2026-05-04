---
title: Financial Report Summarizer
industry: finance
tags: [reporting, financial-statements, analysis, summary, investor-relations]
contributor: justfathi
---

## Description
Summarizes a financial report, 10-K, 10-Q, or annual report into a structured executive summary — highlighting revenue trends, margin changes, balance sheet health, cash flow signals, and key risks.

## Use Case
Investors, analysts, finance students, and executives who need to rapidly extract the most important signals from a lengthy financial filing without reading every page.

## The Prompt
```
You are a financial analyst. Summarize the financial report below into a clear, structured executive summary.

**FINANCIAL REPORT SUMMARY**
Company: [COMPANY NAME] | Period: [PERIOD] | Report type: [10-K / 10-Q / Annual Report / Other]

---

**1. HEADLINE PERFORMANCE** (3–4 sentences)
[The most important story told by this report — growth, profitability, cash position, or turnaround. What changed most since the prior period?]

**2. INCOME STATEMENT HIGHLIGHTS**
| Metric | This Period | Prior Period | Change % |
|--------|-------------|--------------|----------|
| Revenue | | | |
| Gross profit | | | |
| Gross margin % | | | |
| Operating income | | | |
| Operating margin % | | | |
| Net income | | | |
| EPS (diluted) | | | |

Key drivers: [What drove the revenue change — volume, price, new products, geographic expansion, FX?]
Margin story: [Did margins expand or compress? Why?]

**3. BALANCE SHEET HIGHLIGHTS**
| Metric | Current | Prior Year |
|--------|---------|------------|
| Cash & equivalents | | |
| Total debt | | |
| Net debt / (cash) | | |
| Current ratio | | |
| Debt/equity | | |

Balance sheet assessment: [Strengthening / Stable / Deteriorating — 1-sentence explanation]

**4. CASH FLOW HIGHLIGHTS**
| Metric | This Period | Prior Period |
|--------|-------------|--------------|
| Operating cash flow | | |
| Capital expenditures | | |
| Free cash flow | | |
| Dividends paid | | |
| Share buybacks | | |

Cash generation quality: [Is the company converting earnings to cash efficiently? Is FCF growing?]

**5. SEGMENT BREAKDOWN** (if applicable)
[Table or bullets showing revenue and profitability by business unit or geography — highlight which segments are growing and which are declining]

**6. MANAGEMENT'S OUTLOOK**
[Summary of any forward guidance, outlook statements, or strategic priorities mentioned in the report]

**7. KEY RISKS DISCLOSED**
[Top 3–5 risk factors from the report that are most material or new vs. prior filings]
1.
2.
3.

**8. NOTABLE ITEMS**
[Any one-time charges, restatements, accounting changes, impairments, or unusual items that affect comparability]

**9. TAKEAWAY** (2–3 sentences)
[Overall assessment: is the company's financial position improving or deteriorating? What is the single most important thing to watch going forward?]

---

Report to summarize:
[PASTE THE FINANCIAL REPORT TEXT, KEY TABLES, OR MD&A SECTION HERE]
```

## Notes
- For very long filings, prioritize pasting the MD&A (Management Discussion & Analysis) section plus the key financial tables
- The "Notable Items" section is critical for any period with restructuring charges, goodwill impairments, or tax effects — these can mask the underlying performance
- For 10-K summaries, also note changes in auditor, going-concern language, or material weaknesses
- Pair with the Earnings Call Analyzer prompt to get both the filed document and the spoken management narrative
