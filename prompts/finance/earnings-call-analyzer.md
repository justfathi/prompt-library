---
title: Earnings Call Analyzer
industry: finance
tags: [earnings, analysis, investor-relations, equities, signals]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Extracts the signal from an earnings call transcript — identifying key guidance changes, management tone shifts, analyst concern themes, and forward-looking statements the market may be pricing or mispricing.

## Use Case
Analysts, investors, and IR teams who need to get through a long earnings transcript quickly and surface the most important takeaways without reading every word.

## The Prompt
```
You are a senior equity analyst listening to an earnings call. Analyze the transcript below and produce a structured summary.

**EARNINGS CALL ANALYSIS**
Company: [COMPANY NAME] | Quarter: [Q? FY??] | Date: [DATE]

---

**1. HEADLINE NUMBERS VS. EXPECTATIONS**
| Metric | Reported | Consensus Est. | Beat / Miss |
|--------|----------|----------------|-------------|
| Revenue | | | |
| EPS | | | |
| [Key metric specific to sector] | | | |

**2. MANAGEMENT TONE ASSESSMENT**
Overall tone: [Confident / Cautious / Defensive / Mixed]
Tone vs. last quarter: [More bullish / More cautious / Consistent]
Specific language that signals tone:
- Positive signals: [Quote or paraphrase the most bullish language used]
- Cautious signals: [Quote or paraphrase hedging language, qualifiers, or downward revisions]

**3. GUIDANCE CHANGES**
| Item | Previous Guidance | New Guidance | Change |
|------|------------------|--------------|--------|
| Revenue (full year) | | | |
| Margins | | | |
| [Other guided metric] | | | |

Guidance narrative: [Was the change explained? What reason was given?]

**4. KEY THEMES FROM THE CALL** (top 4–5)
[List the major topics management spent the most time on — these reveal their priorities and concerns]
1.
2.
3.
4.
5.

**5. ANALYST CONCERNS — WHAT THE STREET WAS ASKING ABOUT**
[Summarize the themes of analyst questions — what were they worried about? What did they push back on?]
- [Concern 1 + how management responded]
- [Concern 2 + how management responded]
- [Concern 3 + how management responded]

**6. WHAT MANAGEMENT DIDN'T SAY**
[Notable omissions, topics that weren't addressed, or questions that received vague answers — these are often as important as what was said]

**7. KEY FORWARD-LOOKING STATEMENTS**
[Specific statements about future quarters, markets, products, or macro conditions — flag any that represent changes from prior communication]

**8. RED FLAGS** (if any)
[Specific language, metric changes, or non-answers that warrant further investigation]

**9. OVERALL TAKEAWAY** (2–3 sentences)
[Bull case strengthened / weakened? What changed in the investment picture?]

---

Transcript to analyze:
[PASTE EARNINGS CALL TRANSCRIPT OR EXCERPTS HERE]

Additional context (optional):
- Prior quarter guidance: [WHAT THEY SAID LAST QUARTER]
- Thesis to test: [WHAT YOU'RE SPECIFICALLY WATCHING FOR]
```

## Notes
- For very long transcripts, paste the prepared remarks and Q&A separately and run two passes
- Management tone analysis is subjective — cross-reference with year-ago language for context
- "What management didn't say" is often the most valuable section — track which topics disappear between quarters
- Pair with the Investment Thesis Writer prompt to update your thesis after each earnings call
