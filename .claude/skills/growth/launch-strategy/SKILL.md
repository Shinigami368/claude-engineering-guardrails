---
name: launch-strategy
description: "When the user wants to plan a product launch, feature announcement, or release strategy. Also use when the user mentions 'launch,' 'Product Hunt,' 'feature release,' 'announcement,' 'go-to-market,' 'beta launch,' 'early access,' 'waitlist,' 'product update,' 'how do I launch this,' 'launch checklist,' 'GTM plan,' or 'we're about to ship.' Use this whenever someone is preparing to release something publicly. For ongoing marketing after launch, see marketing-ideas."
---

# Skill: launch-strategy

## When To Activate

Use this skill when:
- the user is planning a new product launch, feature release, or public
  announcement
- the task is to structure beta, early access, waitlist, or GA rollout phases
- the user needs a channel plan, launch checklist, or launch-day runbook
- a release needs go-to-market sequencing rather than general ongoing marketing

Use `marketing-ideas` for ongoing channel ideas after the launch plan exists.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify what is launching:
  - new product
  - major feature
  - medium update
  - minor announcement
- Clarify the launch goal:
  - awareness
  - signups
  - activation
  - feedback
  - revenue
- Clarify available channel surface:
  - owned
  - rented
  - borrowed
- Clarify launch timing, audience size, and whether a Product Hunt launch is
  actually in scope.

## Discovery Questions

- Who is the launch for?
- What stage is the product or feature really in?
- What proof, demos, or customer evidence already exists?
- What channels already perform for this audience?
- What happened in prior launches, if any?
- What post-launch follow-through can the team realistically support?

## Decision Framework

- Match launch intensity to the size of the release. Not every update deserves
  a full campaign.
- Use phased launches when the product needs learning before scale:
  - internal
  - alpha
  - beta
  - early access
  - full launch
- Treat owned channels as the durable core. Use rented and borrowed channels to
  amplify, not replace, owned capture.
- Use Product Hunt only when the asset quality, prep, and audience fit justify
  it.
- Design post-launch follow-up before launch day so momentum converts into
  retained attention.

## Output Structure

1. LAUNCH RECOMMENDATION

State the recommended launch phase, goal, and audience.

2. CHANNEL PLAN

State the owned, rented, and borrowed channels to use and why.

3. ASSET CHECKLIST

State the landing page, demo, email, content, and proof assets required.

4. LAUNCH RUNBOOK

State the sequencing before launch, on launch day, and immediately after.

5. POST-LAUNCH FOLLOW-THROUGH

State how feedback, onboarding, comparisons, and the next launch moment will
be handled.

## Honesty And Non-Goals

- Do not promise virality or Product Hunt success.
- Do not recommend channels with no audience-fit evidence.
- Do not confuse launch planning with a generic full-funnel marketing strategy.
- Do not create a launch plan that the team cannot operationally support after
  announcement day.
- Do not treat every release as a major launch event.

## Related Skills

- `email-sequence` for launch and onboarding sequences
- `page-cro` for launch landing page optimization
- `competitor-alternatives` for post-launch comparison assets
- `marketing-ideas` for ongoing promotion after launch
