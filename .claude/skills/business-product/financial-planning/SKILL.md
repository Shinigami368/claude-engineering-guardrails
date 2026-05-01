---
name: financial-planning
description: "When the user wants to build revenue projections, unit economics models, burn rate calculations, or financial plans for a SaaS business. Also use when the user mentions 'MRR,' 'ARR,' 'unit economics,' 'LTV,' 'CAC,' 'burn rate,' 'runway,' 'revenue model,' 'financial projections,' 'pricing model math,' 'break-even,' or 'how much money do I need.' Use this for any financial modeling or planning for a SaaS product."
---

# Skill: financial-planning

## When To Activate

Use this skill when:
- the user needs revenue projections, runway planning, or burn analysis
- the task is unit economics, pricing-model math, or fundraising planning
- the user needs scenario planning for growth, hiring, or cash needs
- business decisions depend on financial assumptions being made explicit

Use `pricing-strategy` for packaging and pricing design when the main question is
what to charge rather than how the math plays out.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify the business stage:
  - pre-revenue
  - early revenue
  - scaling
- Clarify the minimum financial inputs:
  - current MRR or ARR
  - customer count
  - pricing model
  - churn or retention assumptions
  - fixed and variable costs
  - cash on hand
- If the model is for fundraising or investor materials, keep assumptions aligned
  with the canonical facts used elsewhere.

## Discovery Questions

- What decision should the model support?
- What timeframe matters:
  - next quarter
  - 12 months
  - runway to next raise
- Which assumptions are known versus estimated?
- What acquisition and retention channels drive the model?
- Does the user need:
  - revenue projection
  - unit economics
  - burn and runway view
  - fundraising math
  - scenario comparison

## Decision Framework

- Prefer bottom-up math over vague topline targets.
- Make every important assumption visible rather than burying it in outputs.
- Separate current-state facts from forward-looking assumptions.
- Use scenarios only when uncertainty materially changes the decision.
- Tie cost growth and hiring plans to explicit milestones, not flat plug values.
- End with the decision implication, not just the spreadsheet logic.

Key financial areas that may need to be covered:
- revenue metrics such as MRR, ARR, net new MRR, ARPU, and ACV
- unit economics such as LTV, CAC, payback, and gross margin
- retention metrics such as logo churn, revenue churn, and NRR
- burn, runway, raise size, and use-of-funds logic

## Output Structure

1. CURRENT STATE

State the known metrics, cash position, and business stage.

2. ASSUMPTIONS

List the operating assumptions and clearly flag estimates.

3. MODEL OUTPUT

Provide the requested model view, such as projections, unit economics, runway,
or raise planning.

4. RISK AND SCENARIOS

State the main model sensitivities and the downside or upside cases when they
matter.

5. RECOMMENDATION

State what the model implies for pricing, hiring, fundraising, or growth
choices.

## Honesty And Non-Goals

- Do not fabricate metrics, cash position, or retention data.
- Do not present a precise model when the assumptions are weak or missing.
- Do not treat scenario ranges as predictions.
- Do not present this output as accounting, tax, or investment advice.
- Do not hide the assumptions that make the model work.

## Related Skills

- `pricing-strategy` for pricing choices that feed the model
- `growth-metrics` for funnel and conversion analysis
- `market-research` for market sizing context
- `investor-materials` for aligned fundraising outputs
