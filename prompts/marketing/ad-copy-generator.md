---
title: High-Converting Ad Copy Generator
industry: marketing
tags: [ads, copywriting, conversion, paid-social, paid-search]
models: [claude, gpt-4, llama]
contributor: justfathi
---

## Description
Generates high-converting ad copy variants for Facebook, Instagram, Google, or LinkedIn ads — including headline, primary text, and CTA — based on a product brief.

## Use Case
Performance marketers, copywriters, and founders who need multiple ad variations to A/B test across paid channels without spending hours writing copy from scratch.

## The Prompt
```
You are a direct-response copywriter with expertise in paid social and paid search advertising. Write ad copy for the campaign brief below.

Generate 3 distinct variations of the ad. Each variation should use a different psychological hook:
- Variation A: Problem-agitation (lead with the pain)
- Variation B: Social proof / outcome (lead with a result or testimonial angle)
- Variation C: Curiosity / pattern interrupt (lead with something unexpected)

For each variation, write:

**Headline:** (max 40 characters for Google / max 27 characters for Meta — write both if the platform is "both")
**Primary Text:** (max 125 characters for Meta feed / 90 characters for Google — write both if needed)
**Description Line:** (Google only, max 90 characters — skip if Meta only)
**CTA:** (Choose the most relevant: Shop Now / Learn More / Get Started / Sign Up / Book Now / Get Quote)

After the 3 variations, add:

**POWER WORDS USED:** [List the persuasive words used across the copy]
**SPLIT TEST RECOMMENDATION:** [Which two variations to pit against each other first and why]

Campaign brief:
Product/service: [PRODUCT OR SERVICE]
Target audience: [WHO THEY ARE — be specific about demographics, pain points, desires]
Primary benefit: [THE #1 THING THE AD SHOULD COMMUNICATE]
Offer or hook: [DISCOUNT, FREE TRIAL, GUARANTEE, URGENCY, ETC. — or "none"]
Platform: [Facebook / Instagram / Google / LinkedIn / All]
Tone: [Professional / Casual / Urgent / Playful / Luxury]
Landing page context (optional): [WHAT THE PAGE OFFERS OR SAYS]
```

## Notes
- The more specific the target audience description, the better the copy — "women 35–50 with back pain who've tried physiotherapy" beats "adults with pain"
- For Meta ads, primary text over 125 characters will be truncated in feed — check the character count
- Rotate hooks across ad sets to avoid audience fatigue
- Always pair with a matching landing page headline to maintain message continuity
