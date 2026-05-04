---
title: Investment Thesis Writer
industry: finance
tags: [investing, equity, thesis, research, analysis]
contributor: justfathi
---

## Description
Structures a rigorous investment thesis for a public or private company — covering the core opportunity, key assumptions, risk factors, and catalysts — from raw research notes or a company description.

## Use Case
Analysts, portfolio managers, and investors who need to articulate a structured investment case for a stock pitch, investment committee memo, or internal review.

## The Prompt
```
You are a senior equity analyst. Write a structured investment thesis for the company described below.

**INVESTMENT THESIS: [COMPANY NAME] ([TICKER if public])**
Date: [DATE]
Recommendation: [BUY / SELL / HOLD — or leave blank to derive from the analysis]
Target Price / Fair Value: [IF KNOWN — otherwise leave for analyst to add]

---

**1. BUSINESS OVERVIEW** (3–4 sentences)
What the company does, its primary revenue model, key markets, and competitive position. No fluff.

**2. THE CORE THESIS** (2–3 sentences)
The single most important reason to own or avoid this company. This should be specific and falsifiable — not a vague positive sentiment.

**3. WHY NOW — THE CATALYST**
[What specific event, trend, or inflection point makes this an interesting opportunity at this moment?]
- Near-term catalyst (0–6 months): [SPECIFIC TRIGGER]
- Medium-term catalyst (6–18 months): [STRUCTURAL DRIVER]

**4. KEY ASSUMPTIONS**
[List the 4–5 specific, quantifiable assumptions the thesis depends on — these are the things that have to be true for the thesis to play out]
1. [Assumption + why it's reasonable]
2.
3.
4.
5.

**5. WHAT THE MARKET IS MISSING**
[What does the current price imply? What does the market believe that you think is wrong or overly pessimistic/optimistic?]

**6. FINANCIAL SNAPSHOT**
| Metric | Current | Your Estimate (Year+1) | Year+2 |
|--------|---------|------------------------|--------|
| Revenue | | | |
| Revenue growth % | | | |
| EBITDA margin | | | |
| EPS | | | |
| P/E | | | |
| EV/EBITDA | | | |
[Fill in what's known — leave blanks for the analyst to complete]

**7. VALUATION**
[Primary valuation methodology and derived price target or range — e.g., "20x NTM earnings implies $X at the midpoint of our estimates"]

**8. RISK FACTORS**
| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| [Risk 1] | H/M/L | H/M/L | [How to monitor or hedge] |
| [Risk 2] | | | |
| [Risk 3] | | | |

**9. WHAT WOULD MAKE US WRONG**
[The specific 2–3 developments that would invalidate the thesis and trigger a position review]

**10. MONITORING CHECKLIST**
[The 4–5 metrics or events to track each quarter to determine if the thesis is on track]

---

Company information:
Company name: [NAME]
Ticker (if public): [TICKER]
Industry/sector: [SECTOR]
Market cap: [MARKET CAP]
Key products/services: [DESCRIPTION]
Recent developments: [ANY RELEVANT NEWS, EARNINGS, EVENTS]
Your initial view: [BULLISH / BEARISH / NEUTRAL — and the one-sentence reason]
Available data: [PASTE ANY FINANCIAL DATA, EARNINGS NOTES, OR RESEARCH YOU HAVE]
```

## Notes
- The "What the Market is Missing" section is the heart of any differentiated thesis — spend the most effort here
- Assumptions should be specific and testable — "revenue grows 20% in FY25" not "strong growth expected"
- For private companies, replace the financial table with whatever metrics are available (ARR, NRR, burn rate, etc.)
- This prompt produces the structure of a thesis — the numbers still need to come from your own research and models
