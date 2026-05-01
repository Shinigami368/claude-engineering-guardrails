---
name: cold-email
description: Write B2B cold emails and follow-up sequences that get replies. Use when the user wants to write cold outreach emails, prospecting emails, cold email campaigns, sales development emails, or SDR emails. Also use when the user mentions "cold outreach," "prospecting email," "outbound email," "email to leads," "reach out to prospects," "sales email," "follow-up email sequence," "nobody's replying to my emails," or "how do I write a cold email." Covers subject lines, opening lines, body copy, CTAs, personalization, and multi-touch follow-up sequences. For warm/lifecycle email sequences, see email-sequence. For sales collateral beyond emails, see sales-enablement.
---

# Skill: cold-email

## When To Activate

Use this skill when:
- the user needs B2B cold outreach emails or follow-up touches
- the task is to draft a first-touch outbound email with a reply-oriented CTA
- the user wants subject lines, personalization angles, or cold sequence logic
- outbound messaging needs to sound human instead of templated

Use `email-sequence` for warm, lifecycle, onboarding, or nurture flows rather
than true cold outreach.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify the minimum viable context:
  - who the recipient is
  - what specific problem is relevant to them
  - the intended ask
  - available proof
  - any personalization or research hook
- If there is no real personalization or relevance signal, label the output as
  a template that still needs personalization.

Use the bundled references for depth on:
- personalization
- subject lines
- frameworks
- follow-up angles
- benchmarks

## Discovery Questions

- Who is this going to and why this person?
- What outcome do we want from the email?
- What concrete proof or credibility anchor do we have?
- What signal makes this outreach relevant now?
- Is the task one email or a short follow-up sequence?
- What tone fits the audience:
  - executive
  - mid-level
  - technical

## Decision Framework

- Write like a peer, not a vendor.
- Lead with the recipient’s world, not a company introduction.
- Keep every sentence earned; cold outreach should feel easy to skim.
- Make personalization connect to the problem, not sit as a disconnected intro.
- Prefer one low-friction ask over a heavy meeting request.
- Use follow-ups only when each touch adds a new angle, proof point, or reason
  to reply.

## Output Structure

1. OUTREACH STRATEGY

State the recipient, hook, value angle, and intended next step.

2. SUBJECT LINE OPTIONS

Provide short, plausible subject lines matched to the audience and email goal.

3. EMAIL DRAFT

Provide the first-touch email in full.

4. FOLLOW-UP TOUCHES

If requested, provide the follow-up sequence with timing and the new angle for
each touch.

5. STRENGTHENING GAPS

State what missing proof, personalization, or context would materially improve
the draft.

## Honesty And Non-Goals

- Do not fake familiarity, research, or personalization.
- Do not use hype language or vendor jargon to replace substance.
- Do not ask for too much in a first touch unless the user explicitly wants a
  heavier CTA.
- Do not treat warm lifecycle email tactics as cold outreach best practice.
- Do not present unverified proof claims as send-ready facts.

## References

- Personalization: [references/personalization.md](references/personalization.md)
- Subject lines: [references/subject-lines.md](references/subject-lines.md)
- Frameworks: [references/frameworks.md](references/frameworks.md)
- Follow-up sequences: [references/follow-up-sequences.md](references/follow-up-sequences.md)
- Benchmarks: [references/benchmarks.md](references/benchmarks.md)
