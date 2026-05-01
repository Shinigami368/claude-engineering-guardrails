---
name: paid-ads
description: "When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X, or other ad platforms. Also use when the user mentions 'PPC,' 'paid media,' 'ROAS,' 'CPA,' 'ad campaign,' 'retargeting,' 'audience targeting,' 'Google Ads,' 'Facebook ads,' 'LinkedIn ads,' 'ad budget,' 'cost per click,' 'ad spend,' or 'should I run ads.' Use this for campaign strategy, audience targeting, bidding, and optimization. For bulk ad creative generation and iteration, see ad-creative. For landing page optimization, see page-cro."
---

# Skill: paid-ads

## When To Activate

Use this skill when:
- the user needs paid-media strategy, campaign structure, or channel selection
- the task is audience targeting, budget allocation, bidding, retargeting, or
  optimization
- the user wants to decide whether paid ads should be used at all
- an existing paid-acquisition motion is underperforming and needs diagnosis

Use `ad-creative` for bulk ad-copy iteration and `page-cro` for post-click
conversion work once the acquisition plan is defined.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - acquisition objective
  - target CPA or ROAS
  - budget
  - offer
  - landing page
  - audience
  - platform history
  - tracking setup
  - attribution constraints
- If the business has already run ads, clarify what worked, what failed, and
  where the funnel is currently leaking.

## Discovery Questions

- What is the campaign trying to drive:
  - awareness
  - traffic
  - leads
  - sales
  - app installs
- Which platform or platforms are in scope?
- What is the conversion event, and how is it measured today?
- What creative assets or production capacity already exist?
- What audience signals are available:
  - search intent
  - interests
  - job title
  - lookalike seed
  - retargeting pool
- What compliance, geography, or brand constraints apply?
- Is the main problem:
  - channel selection
  - tracking
  - targeting
  - creative fit
  - landing-page mismatch
  - budget fragmentation

## Decision Framework

- Make sure tracking and conversion definitions are credible before recommending
  spend scale-up.
- Choose platforms based on buying intent, audience location, and creative fit,
  not trendiness.
- Keep campaign structure simple enough that budget can learn and signal can be
  read.
- Separate testing from scaling:
  - test angles, audiences, and offers intentionally
  - scale only proven combinations
- Diagnose the real bottleneck before changing bids:
  - poor intent
  - weak creative
  - bad landing-page fit
  - broken tracking
  - weak offer
- Use retargeting and exclusions deliberately so spend is not wasted on the
  wrong audience.

## Output Structure

1. ACQUISITION GOAL

State the objective, target economics, offer, and audience.

2. CHANNEL RECOMMENDATION

State which platforms should be used, why, and which should be deprioritized.

3. CAMPAIGN DESIGN

Provide the recommended campaign structure, audience plan, budget logic, and
measurement setup.

4. TESTING AND OPTIMIZATION PLAN

State what should be tested first, how success should be judged, and what to
change only after enough signal exists.

5. RISKS AND GAPS

State missing tracking, creative, funnel, or attribution issues that could make
ad spend unreliable.

## Honesty And Non-Goals

- Do not imply direct access to ad-platform accounts or APIs unless that access
  is actually present in the user environment.
- Do not recommend scaling spend before the conversion path is measurable.
- Do not treat every paid-ads problem as a bidding problem.
- Do not ignore landing-page quality, offer strength, or creative fit.
- Do not promise ROAS, CPA, or algorithmic performance outcomes.

## Related Skills

- `ad-creative` for ad-copy and creative variation generation
- `copywriting` for landing-page messaging
- `analytics-tracking` for conversion instrumentation
- `ab-test-setup` for post-click testing
- `page-cro` for landing-page optimization
- `marketing-psychology` for persuasion and framing choices
