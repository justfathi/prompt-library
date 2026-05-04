---
title: Unit Test Generator
industry: coding
tags: [testing, unit-tests, tdd, quality, coverage]
contributor: justfathi
---

## Description
Generates comprehensive unit tests for a function or class — covering the happy path, edge cases, error conditions, and boundary values — in the test framework of your choice.

## Use Case
Developers who need to write tests quickly without missing important cases, or teams adopting TDD who want to generate a test skeleton before writing the implementation.

## The Prompt
```
You are a senior software engineer writing unit tests. Generate a comprehensive test suite for the code below.

Requirements:
1. Cover the happy path (expected, normal usage)
2. Cover all edge cases you can identify from the function signature and logic
3. Cover error conditions and invalid inputs
4. Cover boundary values (empty strings, zero, null/undefined, max values, etc.)
5. Each test must have a descriptive name that reads like a sentence: "should return X when Y"
6. Add a brief comment on any non-obvious test explaining the reasoning
7. Group tests logically using describe blocks (or equivalent for the framework)

After the tests, provide:

**COVERAGE NOTES**
- Cases covered: [bulleted list]
- Cases NOT covered (and why): [anything deliberately excluded with reasoning]
- Suggested mocks/stubs: [any external dependencies that need mocking]

Framework: [Jest / Pytest / JUnit / RSpec / Go testing / Vitest / Mocha / other]
Language: [LANGUAGE]

Function/class to test:
```[LANGUAGE]
[PASTE THE CODE TO TEST HERE]
```

Additional context (optional):
- What does this function do? [PLAIN ENGLISH DESCRIPTION]
- Known edge cases to specifically include: [ANY CASES YOU ALREADY KNOW ABOUT]
- External dependencies to mock: [DB, API calls, file system, etc.]
```

## Notes
- For TDD: run this before writing the implementation and let the tests define the spec
- If the function has side effects (DB writes, API calls), always mock those — note them in the additional context
- For complex logic, run a separate pass asking specifically for property-based test ideas
- Generated tests should be reviewed for correctness — especially boundary assertions
