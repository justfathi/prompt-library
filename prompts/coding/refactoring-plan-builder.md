---
title: Refactoring Plan Builder
industry: coding
tags: [refactoring, technical-debt, planning, safety, incremental]
contributor: justfathi
---

## Description
Turns a messy file, module, or function into a sequenced, low-risk refactoring plan — with each step independently safe, testable, and revertible.

## Use Case
Engineers about to clean up a critical or load-bearing piece of code who want to avoid a giant rewrite PR, or tech leads scoping a refactor for a junior engineer to execute incrementally.

## The Prompt
```
You are a senior software engineer planning a refactor. Read the code below and produce a sequenced refactoring plan optimized for safety and reviewability.

Output format:

**REFACTOR GOAL** (1 sentence): [What the code should look like after — in terms of behavior, structure, or maintainability — based on the goal stated below]

**CURRENT STATE — what makes this code hard to work with**
- [Specific problem 1 — concrete, with line/section references]
- [Specific problem 2]
- [...]

**CONSTRAINTS — what must NOT change**
- Public interface / API: [Yes/No — describe what callers depend on]
- Externally observable behavior: [What must stay identical]
- Performance: [Latency or memory bounds, if any]
- Test coverage gap: [Describe; if low, add a "Step 0: add characterization tests"]

**SEQUENCED PLAN**

For each step, output:

**Step N: [Short imperative title]**
- What changes: [Specific code change]
- Why this step now: [What it unlocks; why it must come before later steps]
- Risk: [Low / Medium / High] — [Why]
- How to verify: [Specific test to run, behavior to spot-check, or invariant to assert]
- Revertibility: [Single commit revert / requires backout plan]
- Estimated diff size: [Tiny / Small / Medium / Large]

(Order steps so each one is independently mergeable, behavior-preserving, and reduces blast radius for the next step. Aim for 4–10 steps. The first step should always be the highest-confidence, lowest-risk one — usually adding tests or extracting a constant.)

**SUGGESTED COMMIT SEQUENCE**
A list of commit messages in order, in conventional commit style.

**WHAT TO LEAVE ALONE (and why)**
[Parts of the code that look refactorable but should be deferred — explain the reasoning.]

**EXIT CRITERIA**
[How to know the refactor is "done" — the specific signals to look for.]

Rules:
- Never include "rewrite from scratch" as a step
- Behavior-changing steps must be separated from pure-refactor steps and labeled BEHAVIOR CHANGE in bold
- If test coverage is insufficient to refactor safely, the first step MUST be adding characterization tests
- If a step requires coordination (DB migration, feature flag, deploy ordering), call that out explicitly under Risk

Refactor goal: [WHAT YOU WANT TO ACHIEVE — e.g. "extract payment logic into its own module so we can swap providers"]
Language / framework: [LANGUAGE + FRAMEWORK]
Test situation: [GOOD COVERAGE / SOME COVERAGE / ALMOST NONE — be honest]
Constraints: [ANY HARD CONSTRAINTS — public API, deploy windows, etc.]

Code to refactor:
```[LANGUAGE]
[PASTE CODE HERE]
```
```

## Notes
- The "BEHAVIOR CHANGE" labeling is the most important rule — most refactors go wrong by sneaking behavior changes into "just cleanup" PRs
- For code with no tests, expect Step 0 to be characterization tests; this is non-negotiable for high-risk areas
- Use this prompt before opening a refactor doc — the output drops cleanly into a planning ticket
- Re-run after each step on the updated code — the next steps often shift as the code becomes clearer
