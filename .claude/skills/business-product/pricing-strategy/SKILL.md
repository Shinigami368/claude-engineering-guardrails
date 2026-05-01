---
name: pricing-strategy
description: "When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions 'pricing,' 'pricing tiers,' 'freemium,' 'free trial,' 'packaging,' 'price increase,' 'value metric,' 'Van Westendorp,' 'willingness to pay,' 'monetization,' 'how much should I charge,' 'my pricing is wrong,' 'pricing page,' 'annual vs monthly,' 'per seat pricing,' or 'should I offer a free plan.' Use this whenever someone is figuring out what to charge or how to structure their plans. For in-app upgrade screens, see paywall-upgrade-cro."
---

# Skill: pricing-strategy

## When To Activate

Use this skill when:
- the user needs pricing, packaging, or monetization design
- the task is to choose tiers, value metrics, or price points
- the user is evaluating a free trial, free plan, annual discount, or price
  increase
- a pricing page or GTM motion needs pricing logic behind it

Use `paywall-upgrade-cro` for in-product upgrade UX and `page-cro` for pricing
page conversion work once the pricing model itself is defined.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - product type
  - target segment
  - GTM motion
  - current pricing
  - current plan structure
  - current conversion and churn signals
  - main business goal
- If competitors or substitutes are relevant, clarify which set matters for the
  decision.

Use bundled references when the task needs deeper research design:
- [references/tier-structure.md](references/tier-structure.md)
- [references/research-methods.md](references/research-methods.md)

## Discovery Questions

- What decision is being made:
  - initial pricing
  - repricing
  - repackaging
  - tier redesign
  - price increase
  - trial or free-plan strategy
- What does the customer value most?
- What is the current or proposed value metric?
- Which persona or segment is the pricing optimized for?
- What feedback, conversion, churn, or sales objections indicate pricing is
  broken today?
- What operational or contract constraints limit the design?

## Decision Framework

- Separate packaging, pricing metric, and price point before recommending
  changes.
- Align price with customer value and buying motion rather than cost to serve
  alone.
- Choose one primary optimization goal:
  - growth
  - revenue
  - profitability
  - expansion
- Use tier differentiation that is easy to explain and hard to misinterpret.
- Treat annual billing, discounts, and grandfathering as rollout decisions, not
  afterthoughts.
- Use willingness-to-pay or feature-value research when uncertainty is high
  instead of pretending the answer is obvious.
- Keep the pricing model operationally supportable by sales, finance, and
  customer success.

## Output Structure

1. PRICING QUESTION

State the business goal, target segment, and pricing decision being made.

2. CURRENT STATE AND CONSTRAINTS

State the current pricing structure, market context, and the main signals
driving change.

3. PRICING DESIGN

Provide the recommended:
- packaging model
- value metric
- tier structure
- price points
- billing options

4. ROLLOUT AND TEST PLAN

State migration approach, experiment ideas, customer communication needs, and
what to measure after launch.

5. RISKS AND OPEN QUESTIONS

State where research, data, or competitive evidence is still missing.

## Honesty And Non-Goals

- Do not recommend prices without clarifying the business model and segment.
- Do not treat competitor pricing as the only pricing logic.
- Do not collapse pricing, packaging, and CRO into the same recommendation.
- Do not propose discounts, free plans, or enterprise complexity without a
  clear strategic reason.
- Do not hide uncertainty when research or willingness-to-pay data is weak.

## References

- Tier structure patterns: [references/tier-structure.md](references/tier-structure.md)
- Pricing research methods: [references/research-methods.md](references/research-methods.md)

## Related Skills

- `paywall-upgrade-cro` for in-app upgrade and plan-change surfaces
- `page-cro` for pricing-page conversion optimization
- `copywriting` for pricing-page messaging
- `marketing-psychology` for pricing perception and framing
- `ab-test-setup` for pricing experiments
- `revops` for deal-desk and pricing-governance workflows
- `sales-enablement` for pricing decks, ROI framing, and proposal support
