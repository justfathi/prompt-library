---
title: Comparative Market Analysis (CMA) Summary Writer
industry: real-estate
tags: [cma, pricing, market-analysis, valuation, buyers-sellers]
contributor: justfathi
---

## Description
Transforms raw CMA data into a clear, client-ready narrative summary that explains the pricing recommendation, the comparable sales logic, and the market context — without overwhelming a client with a spreadsheet.

## Use Case
Listing agents and buyer's agents who need to present a CMA recommendation in a way clients actually understand and trust — turning data into a persuasive, readable narrative.

## The Prompt
```
You are a real estate market analyst. Using the CMA data below, write a clear, client-ready summary that explains the pricing recommendation and the reasoning behind it.

**COMPARATIVE MARKET ANALYSIS SUMMARY**
Property: [ADDRESS]
Prepared by: [AGENT NAME]
Date: [DATE]

---

**1. SUBJECT PROPERTY OVERVIEW** (2–3 sentences)
[Brief description of the property and its key attributes that affect value]

**2. MARKET CONDITIONS**
Current market type: [Seller's market / Buyer's market / Balanced — and why]
Key market indicators:
- Average days on market: [X days]
- List-to-sale price ratio: [X%]
- Months of inventory: [X months]
- Trend: [Prices rising / Stable / Softening]

[2–3 sentences explaining what this means for the client — seller or buyer]

**3. COMPARABLE SALES ANALYSIS**
| Address | Beds/Baths | Sq Ft | Sale Price | $/Sq Ft | Days on Market | Sold Date | Adjustment Notes |
|---------|------------|-------|------------|---------|----------------|-----------|------------------|
| [Comp 1] | | | | | | | |
| [Comp 2] | | | | | | | |
| [Comp 3] | | | | | | | |

[2–3 sentences: which comps are most similar and why, and how adjustments were made for differences]

**4. ACTIVE COMPETITION** (what buyers are seeing right now)
| Address | List Price | Days on Market | Key Differences |
|---------|------------|----------------|-----------------|
| [Active 1] | | | |
| [Active 2] | | | |

**5. PRICING RECOMMENDATION**
Recommended range: [$LOW — $HIGH]
Target list price: [$X]

Rationale: [3–5 sentences explaining why this price is supported by the data — be specific about which comps anchor the recommendation and what features justify being at the top or bottom of the range]

**6. PRICING STRATEGY**
[For sellers: pricing at $X positions the home to attract [X buyer profile] and is designed to [generate multiple offers / sell within X days / maximize net proceeds — choose based on the market]. For buyers: [offer strategy relative to list price based on market conditions]]

**7. WHAT HAPPENS IF PRICED DIFFERENTLY**
- Priced $X above recommendation: [Likely outcome]
- Priced $X below recommendation: [Likely outcome]

---

CMA data to summarize:
Subject property details: [DESCRIPTION]
Comparable sales: [PASTE COMP DATA]
Active listings: [PASTE ACTIVE LISTINGS]
Market statistics: [DAYS ON MARKET, ABSORPTION RATE, LIST-TO-SALE RATIO]
Client type: [Seller / Buyer]
Client's initial price expectation (optional): [$X — helps calibrate the narrative]
```

## Notes
- "What happens if priced differently" is the most persuasive section for sellers who want to overprice — use concrete, local data
- For buyer clients, reframe Section 5 as "offer price analysis" rather than listing price recommendation
- The list-to-sale ratio is the most important single metric in a hot market — highlight it prominently
- Always anchor the recommendation to the most recent and most similar sold comp — not the average of all comps
