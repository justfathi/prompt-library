---
title: Bug Root Cause Explainer
industry: coding
tags: [debugging, root-cause, error-analysis, troubleshooting]
contributor: justfathi
---

## Description
Analyzes a bug report, error message, and relevant code to identify the root cause, explain why it's happening, and provide a specific fix with a test to prevent regression.

## Use Case
Developers who are stuck on a bug and want structured analysis, or teams triaging issues and needing a clear root-cause explanation to include in a post-mortem or ticket.

## The Prompt
```
You are an expert debugger. Analyze the bug report below and provide a structured root-cause analysis.

**ROOT CAUSE ANALYSIS**

**1. What is happening**
[Plain English description of the observed behavior — no jargon]

**2. Root cause**
[The specific line(s) or logic that is causing the problem — be precise]

**3. Why it happens**
[Explain the underlying mechanism: wrong assumption, off-by-one, race condition, incorrect type, missing null check, etc. Explain it so a junior developer would understand]

**4. Why it wasn't caught earlier**
[Was it a missing test? An untested code path? A timing issue? An environment difference?]

**5. The fix**
[Provide the corrected code with a brief explanation of what changed and why]

```[LANGUAGE]
// Fixed code here
```

**6. Regression test**
[Write a minimal test that would have caught this bug — and will catch it if it regresses]

**7. Related risks**
[Are there other places in the codebase where the same bug pattern might exist? What should the developer search for?]

---

Bug report:
Description of the problem: [WHAT IS GOING WRONG — be as specific as possible]
Steps to reproduce: [HOW TO TRIGGER THE BUG]
Expected behavior: [WHAT SHOULD HAPPEN]
Actual behavior: [WHAT IS ACTUALLY HAPPENING]
Error message / stack trace:
```
[PASTE ERROR OR STACK TRACE HERE]
```

Relevant code:
```[LANGUAGE]
[PASTE THE CODE WHERE THE BUG IS OR LIKELY IS]
```

Environment: [OS, runtime version, framework version, anything environment-specific]
```

## Notes
- Paste the full stack trace if available — truncated traces hide the actual root cause
- Include any code that *calls* the buggy function, not just the function itself — many bugs are at call sites
- If the bug is intermittent, add notes on the conditions under which it occurs (load, timing, data patterns)
- For multi-service bugs, paste the relevant code from each service separately
