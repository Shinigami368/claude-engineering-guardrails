---
name: marketing-psychology
description: "When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when the user mentions 'psychology,' 'mental models,' 'cognitive bias,' 'persuasion,' 'behavioral science,' 'why people buy,' 'decision-making,' 'consumer behavior,' 'anchoring,' 'social proof,' 'scarcity,' 'loss aversion,' 'framing,' or 'nudge.' Use this whenever someone wants to understand or leverage how people think and make decisions in a marketing context."
---

# Skill: marketing-psychology

## When To Activate

Use this skill when:
- the user wants behavioral-science guidance for marketing decisions
- the task is to improve messaging, pricing perception, conversion, or
  activation by understanding how buyers decide
- the user needs a psychological diagnosis for why a campaign, page, or offer
  is underperforming
- the question is about persuasion principles, mental models, or ethical choice
  architecture in a GTM context

Use `customer-research` when the missing piece is direct evidence about what
customers actually think, and use `copywriting`, `page-cro`, or `paid-ads` when
execution rather than diagnosis is the main job.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - audience segment
  - stage of the journey
  - asset or channel in scope
  - desired behavior
  - current friction or underperformance
  - ethical or compliance constraints
- If the problem is tied to pricing, retention, onboarding, or ads, clarify
  that downstream workflow before recommending psychology-based changes.

## Discovery Questions

- What behavior should change:
  - click
  - sign up
  - buy
  - upgrade
  - continue
  - refer
- Where is the friction showing up today?
- What does the current message, offer, or experience ask the user to do?
- What evidence exists:
  - user feedback
  - funnel data
  - tests
  - customer language
- Is the problem about:
  - trust
  - clarity
  - urgency
  - motivation
  - effort
  - risk perception
- Which channel or asset is in scope?

## Decision Framework

- Start with the behavior and friction point, not the mental model label.
- Prefer the smallest set of principles that explains the behavior clearly.
- Match the intervention to the real decision barrier:
  - low trust
  - low relevance
  - too much effort
  - poor framing
  - weak social proof
  - unclear value
- Treat psychology as a design lens, not a substitute for customer evidence.
- Use ethical persuasion only:
  - no fake scarcity
  - no fabricated social proof
  - no manipulative dark patterns
- If multiple models apply, prioritize the ones that produce the clearest
  change in messaging, offer design, or interaction design.

Common principle families may include:
- framing and anchoring
- loss aversion and risk reduction
- social proof and authority
- defaults, choice reduction, and ease
- commitment, progress, and habit formation

## Output Structure

1. BEHAVIOR GOAL

State the target audience, current context, and the behavior that should
change.

2. PSYCHOLOGICAL DIAGNOSIS

State the most likely decision barriers and why they matter.

3. PRINCIPLES TO APPLY

List the 1 to 3 most relevant principles and how each one maps to the problem.

4. MARKETING APPLICATION

Provide the concrete changes to make in the relevant asset, offer, or journey.

5. RISKS AND TESTS

State ethical guardrails, likely failure modes, and what should be tested or
validated next.

## Honesty And Non-Goals

- Do not use psychology language to justify manipulative tactics.
- Do not present generic bias lists as if they were decision-ready advice.
- Do not claim certainty where customer evidence is weak or missing.
- Do not substitute borrowed mental models for actual messaging clarity.
- Do not fabricate urgency, social proof, or authority signals.

## Related Skills

- `customer-research` for direct buyer evidence
- `copywriting` for message execution
- `page-cro` for page-level conversion improvement
- `pricing-strategy` for pricing perception and framing
- `paid-ads` for channel and campaign execution
- `referral-program` for motivation design in word-of-mouth loops
