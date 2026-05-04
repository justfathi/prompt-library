---
title: Personal Financial Plan Builder
industry: finance
tags: [personal-finance, planning, budgeting, savings, goals]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Builds a structured, prioritized personal financial plan from a snapshot of someone's income, expenses, debts, and goals — with specific action steps and a timeline.

## Use Case
Individuals who want a structured financial plan but can't afford a financial advisor, or advisors who want to produce a first-draft plan document quickly before a client meeting.

## The Prompt
```
You are a personal financial planner. Using the financial snapshot below, build a structured, prioritized personal financial plan.

**PERSONAL FINANCIAL PLAN**
Prepared for: [NAME or "Client"]
Date: [DATE]

---

**1. FINANCIAL SNAPSHOT SUMMARY**
| Category | Monthly Amount | Notes |
|----------|---------------|-------|
| Gross income | | |
| Net take-home | | |
| Total fixed expenses | | |
| Total variable expenses | | |
| Current monthly savings | | |
| Total debt | | |
| Total liquid savings/investments | | |

**2. FINANCIAL HEALTH ASSESSMENT**
- Savings rate: [% of net income currently saved — benchmark: 20%+]
- Emergency fund status: [X months of expenses covered — target: 3–6 months]
- Debt-to-income ratio: [Monthly debt payments / gross income — flag if >36%]
- Overall health: [Strong / Adequate / Needs attention / At risk — with 1-sentence reason]

**3. PRIORITY ACTION PLAN**
[Ranked by urgency and impact. For each action:]

**Priority 1: [ACTION NAME]** ← Most urgent
Why: [1 sentence]
How: [Specific steps]
Target: [Measurable goal]
Timeline: [By when]

**Priority 2: [ACTION NAME]**
[Same structure]

[Continue through Priority 5]

Standard priority order (adjust based on individual situation):
1. Stop the bleeding (high-interest debt, emergency fund minimum of 1 month)
2. Employer match capture (free money — always first)
3. High-interest debt payoff (>7% rate)
4. Emergency fund to 3–6 months
5. Long-term investing (retirement, index funds)

**4. DEBT PAYOFF STRATEGY**
| Debt | Balance | Rate | Min Payment | Recommended Strategy |
|------|---------|------|-------------|----------------------|
| [Debt 1] | | | | |
| [Debt 2] | | | | |

Strategy recommendation: [Avalanche (highest rate first) or Snowball (lowest balance first) — with reasoning for this person's situation]
Payoff timeline at current pace: [X months]
Payoff timeline with [recommended extra payment]: [Y months]
Interest saved: [$Z]

**5. SAVINGS & INVESTMENT PLAN**
| Goal | Target Amount | Timeline | Monthly Contribution Needed | Account Type |
|------|--------------|----------|-----------------------------|--------------|
| Emergency fund | | | | High-yield savings |
| [Goal 1] | | | | |
| Retirement | | | | 401k / IRA |

**6. MONTHLY BUDGET RECOMMENDATION**
| Category | Current | Recommended | Change |
|----------|---------|-------------|--------|
| Housing | | | |
| Food | | | |
| Transport | | | |
| Subscriptions | | | |
| Savings | | | |
| Debt payments | | | |
| Discretionary | | | |

**7. QUICK WINS** (actions that take less than 1 hour)
1. [Specific immediate action]
2.
3.

**8. 12-MONTH MILESTONES**
[Month 3 / Month 6 / Month 12 — specific measurable targets to hit]

---

Financial snapshot:
Gross monthly income: [AMOUNT]
Net monthly take-home: [AMOUNT]
Monthly expenses (itemize if possible): [LIST]
Current savings and investments: [ACCOUNTS AND BALANCES]
Debts: [NAME, BALANCE, INTEREST RATE, MINIMUM PAYMENT]
Financial goals: [LIST GOALS WITH DESIRED TIMELINE]
Age: [AGE]
Employer retirement match: [% AND MATCH STRUCTURE — or "none"]
```

## Notes
- This produces a planning framework — it does not constitute licensed financial advice
- The priority action plan adjusts based on the individual situation; the model will weight emergency fund vs. debt payoff based on rates and risk
- For tax optimization (Roth vs. traditional, HSA, tax-loss harvesting), run a separate prompt with the full tax picture
- Revisit the plan every 6 months or after any major life change (job change, marriage, child, home purchase)
