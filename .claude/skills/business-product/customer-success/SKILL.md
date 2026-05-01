---
name: customer-success
description: "When the user wants to design customer onboarding playbooks, support templates, knowledge bases, NPS programs, or retention strategies. Also use when the user mentions 'customer success,' 'support template,' 'help center,' 'knowledge base,' 'NPS,' 'customer health score,' 'customer onboarding,' 'retention strategy,' 'customer churn,' 'support SLA,' 'help documentation,' or 'how to keep customers happy.' Use this for any customer-facing operations work."
---

# Skill: customer-success

## When To Activate

Use this skill when:
- the user needs onboarding, support, or retention operations
- the task is to design knowledge-base structure, response templates, or NPS
  flows
- the user needs customer health scoring or intervention playbooks
- a churn, activation, or support-quality problem needs an operational response

Use `customer-research` when the task is to learn from customers rather than
design post-sale systems.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Reuse existing customer segments, use cases, and value promises before
  designing success workflows.
- Clarify the operating model:
  - self-serve
  - low-touch
  - high-touch
  - enterprise
- Clarify current scale:
  - customer count
  - segment mix
  - support volume
  - churn or retention concern

## Discovery Questions

Capture the minimum operating context:
- What part of customer success needs work:
  - onboarding
  - support
  - knowledge base
  - health scoring
  - NPS
  - retention
- What resources exist today?
- Who owns customer success right now?
- What are the strongest churn or escalation signals?
- What customer outcomes matter most after purchase?
- What response-time or service expectations already exist?

## Decision Framework

- Optimize for customer outcomes, not raw feature usage.
- Prefer proactive systems over reactive firefighting.
- Default to scalable workflows first, then add high-touch layers where account
  value or risk justifies it.
- Match onboarding, support, and intervention intensity to segment value and
  complexity.
- Use health signals that combine behavior, support, engagement, and contract
  context instead of a single metric.
- Make intervention thresholds and owners explicit so the playbook is
  operational, not aspirational.

## Output Structure

Choose the deliverable that matches the request:

1. CUSTOMER SUCCESS GOAL

State the business problem, target segment, and success metric.

2. OPERATING MODEL

State the service tier, owner, and system boundaries for the workflow.

3. PLAYBOOK OR ASSET

Provide the requested artifact, such as:
- onboarding sequence
- help-center structure
- support templates
- health score model
- NPS workflow
- retention intervention plan

4. ESCALATION AND MEASUREMENT

State triggers, owners, response timing, and the metrics used to evaluate the
system.

## Honesty And Non-Goals

- Do not promise SLA or staffing commitments that the team has not approved.
- Do not treat feature usage alone as proof of customer success.
- Do not design an enterprise-grade motion for a business that only supports
  self-serve operations.
- Do not invent churn causes or benchmark targets without evidence.
- Do not use this skill as a substitute for product or market research.

## Related Skills

- `customer-research` for discovering customer needs and churn drivers
- `growth-metrics` for retention and engagement measurement
- `onboarding-cro` for product-level onboarding optimization
- `email-sequence` for automated lifecycle communication
