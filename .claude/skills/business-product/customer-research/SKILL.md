---
name: customer-research
description: "When the user wants to understand their customers through interviews, surveys, persona development, or jobs-to-be-done analysis. Also use when the user mentions 'user interview,' 'customer persona,' 'JTBD,' 'jobs to be done,' 'user research,' 'customer discovery,' 'feedback synthesis,' 'customer segments,' 'who is my customer,' 'what do customers want,' 'voice of customer,' or 'buyer persona.' Use this for any qualitative or quantitative customer understanding work."
---

# Skill: customer-research

## When To Activate

Use this skill when:
- the user needs interview guides, customer discovery, or JTBD analysis
- the task is persona development, PMF surveying, or feedback synthesis
- product, marketing, sales, or fundraising decisions need customer evidence
- the user needs a structured research plan before collecting customer input

Use `market-research` for category or competitor research rather than customer
behavior research.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Reuse existing customer language, segments, or positioning before asking
  repetitive intake questions.
- Clarify whether the audience is:
  - current customers
  - prospects
  - churned users
  - a mixed segment

If the research is supposed to change a real decision, name that decision
explicitly before designing the work.

## Discovery Questions

Capture the minimum context needed to run the research well:
- What question are we trying to answer?
- What decision will this inform?
- Who should be researched?
- What evidence already exists?
- What method fits the task:
  - interview
  - survey
  - feedback synthesis
  - persona/JTBD synthesis
- What is the timeline, sample size, or budget constraint?

## Analysis Standards

- Prioritize behavior over hypotheticals. Ask what customers did, not what
  they imagine doing.
- Preserve verbatim language whenever it materially affects positioning, copy,
  or product decisions.
- Separate discovery from validation. Open exploration and hypothesis testing
  are not the same mode.
- Treat repeated themes as signals and isolated anecdotes as inputs, not
  conclusions.
- When using JTBD framing, surface:
  - push
  - pull
  - habit
  - anxiety
- Distinguish clearly between:
  - observed evidence
  - interpreted patterns
  - recommended actions

## Output Structure

Choose the lightest output that answers the decision question:

1. RESEARCH PLAN

State the question, audience, method, and sample target.

2. COLLECTION ASSET

Provide the interview guide, survey draft, or tagging approach needed to gather
the evidence.

3. SYNTHESIS

Summarize the top themes, supporting quotes, and frequency or strength of the
signal.

4. CUSTOMER MODEL

Provide the persona, JTBD statement, or segment view only when the evidence
supports it.

5. DECISION IMPLICATIONS

State what product, marketing, sales, or retention decisions should change.

## Honesty And Non-Goals

- Do not invent personas, pain points, or customer quotes.
- Do not treat a tiny sample as statistically representative.
- Do not confuse feature requests with validated strategy without additional
  evidence.
- Do not claim product-market fit from a single survey signal alone.
- Do not use this skill for market sizing, competitor analysis, or funnel math
  that belongs to other skills.

## Related Skills

- `product-marketing-context` for shared product and audience grounding
- `market-research` for market, category, and competitor research
- `growth-metrics` for quantitative funnel or retention analysis
- `customer-success` for post-sale operational playbooks
