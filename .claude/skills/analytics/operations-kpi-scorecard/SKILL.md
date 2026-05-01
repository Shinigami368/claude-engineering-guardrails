---
name: operations-kpi-scorecard
description: "Design, build, and maintain operational KPI scorecards for any industry. Use when the user mentions 'KPI scorecard,' 'operational metrics,' 'performance dashboard,' 'OKRs,' 'business metrics,' 'what should we measure,' 'how do we track performance,' 'operational health,' 'efficiency metrics,' 'SLA tracking,' 'department metrics,' or 'executive dashboard.' Works for any business type — not limited to SaaS."
---

# Skill: operations-kpi-scorecard

## When To Activate

Use this skill when:
- the user needs a KPI scorecard, operating dashboard, or review cadence
- the task is to choose what a team, function, or business should measure
- the user needs KPI definitions, owners, thresholds, or executive reporting
- the problem is metric sprawl, vanity metrics, or weak operational visibility

Use `growth-metrics` for SaaS growth and retention frameworks when the main
question is product-growth measurement rather than cross-functional operations.

## Context Prerequisites

- Check `.claude/industry-context.md` first if it exists.
- Check workflow maps or process documents if they already exist.
- Check `.claude/product-marketing-context.md` when customer, funnel, or growth
  goals affect KPI selection.
- Clarify:
  - scorecard audience
  - review cadence
  - business model
  - team or function in scope
  - current data sources
  - known reporting pain points

## Discovery Questions

- What decisions should this scorecard support?
- Who reviews it:
  - executive team
  - department lead
  - operations team
  - functional manager
- What operating domains matter most:
  - financial
  - customer
  - operational
  - quality
  - people
  - compliance
- What metrics exist today, and which ones are ignored or distrusted?
- What owner, benchmark, or data-source gaps already exist?
- What signals should act as leading indicators rather than lagging summaries?

## Decision Framework

- Prefer 8 to 15 meaningful KPIs over a large dashboard with weak signal.
- Every KPI must have:
  - a definition
  - an owner
  - a data source
  - a review cadence
  - thresholds
  - an action trigger
- Balance leading and lagging indicators so the scorecard supports action, not
  just retrospective reporting.
- Match metric categories to the actual operating model and industry instead of
  forcing generic SaaS defaults onto every business.
- Use trend, target, and benchmark context so the scorecard is interpretable at
  review time.
- Flag vanity metrics, unowned KPIs, and stale targets as design failures.

Typical KPI categories may include:
- financial
- customer
- operational
- quality
- people
- compliance
- delivery
- sales or pipeline

## Output Structure

1. SCORECARD GOAL

State the business scope, audience, review cadence, and decision purpose.

2. KPI SET

List the recommended KPIs by category with a short reason each one belongs on
the scorecard.

3. KPI DEFINITIONS

For each KPI, provide:
- definition
- owner
- data source
- frequency
- target
- thresholds
- action trigger
- leading or lagging classification

4. REVIEW OPERATING MODEL

State who reviews the scorecard, how often, and what should happen when a KPI
goes yellow or red.

5. RISKS AND GAPS

State benchmark gaps, instrumentation gaps, owner ambiguity, or places where
the scorecard still needs validation.

## Honesty And Non-Goals

- Do not propose KPIs before understanding the business model and operating
  context.
- Do not confuse dashboards with management systems.
- Do not recommend vanity metrics that fail to inform decisions.
- Do not leave KPI definitions ambiguous or ownerless.
- Do not invent industry benchmarks when none have been confirmed.

## Related Skills

- `industry-context` for vertical and regulatory grounding
- `workflow-discovery` for mapping the processes that need measurement
- `growth-metrics` for SaaS growth and retention metrics
- `financial-planning` for forecast and unit-economics modeling
- `analytics-tracking` for implementing product or funnel instrumentation
- `observability-designer` for technical reliability metrics
