---
name: email-sequence
description: When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email program. Also use when the user mentions "email sequence," "drip campaign," "nurture sequence," "onboarding emails," "welcome sequence," "re-engagement emails," "email automation," "lifecycle emails," "trigger-based emails," "email funnel," "email workflow," "what emails should I send," "welcome series," or "email cadence." Use this for any multi-email automated flow. For cold outreach emails, see cold-email. For in-app onboarding, see onboarding-cro.
---

# Skill: email-sequence

## When To Activate

Use this skill when:
- the user needs a drip campaign, lifecycle flow, or automated nurture sequence
- the task is to design welcome, onboarding, re-engagement, post-purchase, or
  lead-nurture email logic
- the user needs sequence timing, email roles, or CTA progression across
  multiple touches
- an existing email program needs restructuring or optimization

Use `cold-email` for outbound prospecting emails instead of warm or triggered
automation.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - what triggers entry
  - who enters the sequence
  - what they already know
  - the primary conversion goal
  - what other emails they already receive
- Clarify the sequence type:
  - welcome
  - onboarding
  - nurture
  - re-engagement
  - post-purchase
  - event-driven

Use the references for template depth, email categories, and copy standards.

## Discovery Questions

- What starts the sequence?
- What relationship stage is the audience in?
- What is the one primary outcome of the sequence?
- What supporting outcomes matter:
  - education
  - segmentation
  - activation
  - retention
- What constraints matter:
  - sales cycle length
  - product complexity
  - send frequency tolerance
  - current performance

## Decision Framework

- Give each email one primary job.
- Build trust with value before escalating the ask.
- Prefer relevance and progression over volume.
- Match cadence to context, urgency, and relationship stage.
- Coordinate email with the surrounding lifecycle instead of treating the
  sequence as an isolated funnel.
- Make the exit conditions and success criteria explicit.

## Output Structure

1. SEQUENCE STRATEGY

State the trigger, audience, goal, sequence type, and exit conditions.

2. CADENCE PLAN

State the number of emails, timing, and why that pacing fits.

3. EMAIL MAP

List each email’s role, key message, and CTA.

4. EMAIL DRAFTS

Provide subject, preview, and body copy for the requested emails.

5. MEASUREMENT PLAN

State the key metrics, benchmarks, and first test levers.

## Honesty And Non-Goals

- Do not mix cold outreach tactics into lifecycle email by default.
- Do not overload a single email with multiple unrelated jobs.
- Do not recommend frequency the audience or product stage cannot support.
- Do not promise benchmark outcomes as guaranteed results.
- Do not ignore the emails already hitting the same audience.

## References

- Sequence templates: [references/sequence-templates.md](references/sequence-templates.md)
- Email types: [references/email-types.md](references/email-types.md)
- Copy guidelines: [references/copy-guidelines.md](references/copy-guidelines.md)
