---
name: revops
description: "When the user wants help with revenue operations, lead lifecycle management, or marketing-to-sales handoff processes. Also use when the user mentions 'RevOps,' 'revenue operations,' 'lead scoring,' 'lead routing,' 'MQL,' 'SQL,' 'pipeline stages,' 'deal desk,' 'CRM automation,' 'marketing-to-sales handoff,' 'data hygiene,' 'leads aren't getting to sales,' 'pipeline management,' 'lead qualification,' or 'when should marketing hand off to sales.' Use this for anything involving the systems and processes that connect marketing to revenue. For cold outreach emails, see cold-email. For email drip campaigns, see email-sequence. For pricing decisions, see pricing-strategy."
---

# Skill: revops

## When To Activate

Use this skill when:
- the user needs revenue-operations design across marketing, sales, and CS
- the task is lead lifecycle, scoring, routing, or pipeline-stage design
- the user needs CRM automation, handoff rules, or deal-desk process design
- a revenue leak exists between teams, systems, or lifecycle stages

Use channel or content skills for acquisition execution; use this skill for the
system that routes and measures revenue motion.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - GTM motion
  - ACV range
  - sales cycle length
  - current stack
  - current ownership model
  - current leak or failure point
- If the problem is already narrow, start there instead of rebuilding the whole
  funnel model.

## Discovery Questions

- Where is the lifecycle breaking today?
- What are the current lead and opportunity stages?
- How are MQL, SQL, and opportunity defined?
- What routing method is used now?
- What SLAs exist between teams?
- Which automation, scoring, or data-quality rules are missing?
- What metric should improve if the system is fixed?

## Decision Framework

- Choose one system of record and align the rest to it.
- Define stages, scoring, routing, and handoff rules before automating them.
- Require both fit and intent where qualification depends on both.
- Treat every handoff as a measurable leak point with an owner and SLA.
- Match routing and deal-desk complexity to deal size and motion rather than
  overbuilding process.
- Use hygiene, auditability, and fallback ownership to keep leads from stalling.

Important revenue-ops areas may include:
- lifecycle stage definitions
- MQL and SQL qualification logic
- explicit and implicit lead scoring
- routing rules and speed-to-lead
- pipeline stage requirements and stale-deal controls
- CRM automation and deal-desk thresholds
- data hygiene, enrichment, and dedup strategy

## Output Structure

1. REVENUE OPS GOAL

State the business problem, funnel boundary, and target improvement.

2. LIFECYCLE DESIGN

State the stage definitions, owners, and entry or exit rules.

3. ROUTING AND AUTOMATION

State the scoring, routing, SLA, and workflow logic.

4. DATA AND GOVERNANCE

State the system-of-record, hygiene rules, and accountability checks.

5. METRICS AND PRIORITIES

State what should be measured and what to implement first.

## Honesty And Non-Goals

- Do not automate undefined or disputed lifecycle logic.
- Do not recommend scoring or routing rules without a clear business reason.
- Do not treat every funnel issue as a tooling issue.
- Do not build enterprise-grade RevOps process if the sales motion does not
  justify it.
- Do not ignore ownership and SLA design when recommending automation.

## Related Skills

- `saas-operations` for subscription and billing operations
- `growth-metrics` for funnel and conversion analysis
- `cold-email` for outbound copy execution
- `email-sequence` for lifecycle email execution
