---
name: market-research
description: Conduct market research, competitive analysis, investor due diligence, and industry intelligence with source attribution and decision-oriented summaries. Use when the user wants market sizing, competitor comparisons, fund research, technology scans, or research that informs business decisions.
---

# Skill: market-research

## When To Activate

Use this skill when:
- researching a market, category, company, investor, or technology trend
- building TAM, SAM, or SOM estimates
- comparing competitors or substitutes
- preparing investor dossiers or partnership due diligence
- evaluating a new geographic market, vertical, or regulatory shift

This is a lane-backbone research skill. Keep outputs decision-oriented rather
than encyclopedic.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` if product positioning is
  relevant.
- Check `.claude/industry-context.md` if the research depends on vertical or
  regulatory context.
- Name the decision question before starting:
  - market entry
  - competitor response
  - fundraising target
  - vendor choice
  - category sizing
- Clarify geography, timeframe, and target customer segment when they affect
  the answer.

## Discovery Questions

Capture only what materially changes the research scope:
- What decision will this research support?
- Which market, company set, or technology set is in scope?
- What depth is needed:
  - quick scan
  - comparison
  - full research memo
- What evidence already exists?
- Does the user need:
  - competitor analysis
  - market sizing
  - investor research
  - technology evaluation
  - industry deep dive

## Research Standards

- Source every material claim.
- Date all time-sensitive data and flag anything meaningfully stale.
- Show the math for market sizing and scenario estimates.
- Separate:
  - verified fact
  - inference
  - speculation
- Include downside, counterevidence, or disconfirming signals when they matter.
- End with a decision implication, not just a fact dump.

Use the lightest research mode that answers the question:
- competitor analysis
- market sizing
- investor or fund research
- technology or vendor evaluation
- industry or vertical deep dive

## Output Structure

1. RESEARCH QUESTION

State the decision being supported and the confidence target.

2. KEY FINDINGS

List the most decision-relevant findings first.

3. EVIDENCE

For each major finding, provide the source, date, and the extracted signal or
calculation.

4. IMPLICATIONS

State what the findings mean for strategy, prioritization, or risk.

5. RISKS AND GAPS

State uncertainty, missing evidence, or areas that still need validation.

6. RECOMMENDATION

Provide the next action or decision path supported by the evidence.

## Honesty And Non-Goals

- Do not fabricate numbers, URLs, valuations, or market sizes.
- Do not hide stale or low-confidence evidence behind precise language.
- Do not present research as legal, investment, or regulatory advice.
- Do not confuse category commentary with a decision-ready recommendation.
- Do not write research theater that fails to answer the user’s actual
  question.
