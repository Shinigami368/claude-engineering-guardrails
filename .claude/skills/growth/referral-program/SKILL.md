---
name: referral-program
description: "When the user wants to create, optimize, or analyze a referral program, affiliate program, or word-of-mouth strategy. Also use when the user mentions 'referral,' 'affiliate,' 'ambassador,' 'word of mouth,' 'viral loop,' 'refer a friend,' 'partner program,' 'referral incentive,' 'how to get referrals,' 'customers referring customers,' or 'affiliate payout.' Use this whenever someone wants existing users or partners to bring in new customers. For launch-specific virality, see launch-strategy."
---

# Skill: referral-program

## When To Activate

Use this skill when:
- the user wants to design or improve a referral, affiliate, or ambassador
  program
- the task is incentive design, referral-loop structure, or word-of-mouth
  activation
- the user needs to diagnose why referrals are not happening or not converting
- the business wants existing customers or partners to become an acquisition
  channel

Use `launch-strategy` for launch-specific virality plans and `email-sequence`
for the lifecycle communication that supports the program after its structure is
defined.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - program type
  - business model
  - customer LTV
  - current CAC
  - shareability of the product
  - current referral behavior
  - incentive budget
  - tool or platform constraints
- If the program touches commissions, payouts, or legal terms, note that those
  details may need finance or legal review outside this skill.

## Discovery Questions

- Is the program for:
  - customer referrals
  - affiliates
  - ambassadors
  - partners
  - a hybrid model
- What moment naturally triggers sharing today?
- What reward structure is currently used or being considered?
- What conversion path does the referred user see?
- What abuse, fraud, or low-quality lead risk exists?
- What current metrics indicate the program is weak:
  - awareness
  - share rate
  - conversion rate
  - payout efficiency
- What tools, attribution, or tracking systems exist today?

## Decision Framework

- Separate customer referral logic from affiliate or partner logic before
  designing incentives.
- Match rewards to unit economics so the program can scale without hidden
  margin damage.
- Design the loop from trigger moment through reward delivery, not just the
  reward amount.
- Make sharing simple and the referred-user experience credible.
- Use double-sided incentives only when they improve conversion enough to
  justify the added cost.
- Add fraud controls, payout rules, and attribution boundaries before scaling.
- Optimize for referred-customer quality, not just raw referral volume.

## Output Structure

1. PROGRAM GOAL

State the acquisition goal, program type, target participants, and success
metric.

2. REFERRAL OR AFFILIATE LOOP

State the trigger moment, share mechanism, landing experience, and conversion
path.

3. INCENTIVE AND GOVERNANCE DESIGN

State the reward structure, eligibility rules, payout logic, and abuse controls.

4. LAUNCH AND OPTIMIZATION PLAN

State how to launch, what to test first, and how to improve awareness, share
rate, or conversion over time.

5. RISKS AND GAPS

State economic, fraud, tooling, attribution, or policy concerns that still need
validation.

## Honesty And Non-Goals

- Do not assume a product is naturally referral-worthy without evidence.
- Do not recommend reward levels that ignore LTV, CAC, or margin reality.
- Do not imply direct platform or API integrations unless they actually exist.
- Do not treat referral volume as success if lead quality is poor.
- Do not present commission, tax, or legal-policy recommendations as settled
  advice without the right review.

## Related Skills

- `launch-strategy` for rollout planning
- `email-sequence` for referral and affiliate communication
- `marketing-psychology` for motivation and incentive framing
- `analytics-tracking` for attribution and program measurement
- `customer-success` for post-purchase moments that trigger sharing
