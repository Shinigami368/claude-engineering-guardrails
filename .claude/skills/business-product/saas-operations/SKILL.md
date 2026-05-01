---
name: saas-operations
description: "When the user wants to design billing lifecycle, subscription management, dunning flows, payment recovery, or support SLA systems. Also use when the user mentions 'billing,' 'subscription management,' 'dunning,' 'payment recovery,' 'failed payments,' 'churn recovery,' 'involuntary churn,' 'plan changes,' 'upgrade flow,' 'downgrade,' 'cancellation flow,' 'support SLA,' 'trial expiration,' 'billing integration,' 'Stripe setup,' 'subscription lifecycle,' or 'how to handle billing.' Use this for operational SaaS infrastructure that keeps revenue flowing."
---

# Skill: saas-operations

## When To Activate

Use this skill when:
- the user needs billing-lifecycle or subscription-operations design
- the task is dunning, payment recovery, trial handling, or plan management
- the user needs support-SLA or subscription-health operating rules
- operational SaaS revenue systems need to be designed or repaired

Use `churn-prevention` when the main problem is voluntary or involuntary churn
reduction rather than the broader subscription operating model.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - billing provider
  - self-serve versus enterprise motion
  - monthly and annual mix
  - current trial model
  - current payment-failure handling
  - support expectations and staffing
- If revenue loss or churn is the driver, clarify whether it comes from:
  - failed payments
  - bad plan design
  - weak trial conversion
  - poor support operations

## Discovery Questions

- What operational problem is the user trying to solve?
- What lifecycle states matter today:
  - prospect
  - trial
  - active
  - past due
  - cancelled
  - win-back
- What tooling is already in place?
- What manual work still happens in billing or support?
- What service tiers or SLA expectations exist?
- What current metrics indicate the system is failing?

## Decision Framework

- Design lifecycle states and transition rules before automating them.
- Optimize for reliable revenue capture and low operational ambiguity.
- Make upgrading easy and cancellation clear, without dark patterns.
- Treat involuntary churn as a solvable operations problem with dunning,
  retries, and payment-method recovery.
- Match plan-change, billing, and support workflows to the actual customer
  motion and account value.
- Define owner, trigger, and fallback for every critical lifecycle event.

Important operating areas may include:
- trial design and trial-to-paid conversion
- billing provider events and webhook handling
- upgrade, downgrade, pause, and cancellation flows
- dunning cadence and recovery targets
- support tiers, response expectations, and escalation rules

## Output Structure

1. OPERATIONS GOAL

State the business problem, lifecycle scope, and target outcome.

2. CURRENT-STATE RISKS

State where the current billing or support operation is leaking revenue or
creating friction.

3. OPERATING DESIGN

Provide the lifecycle, workflow, or policy design needed for the system.

4. AUTOMATION AND OWNERSHIP

State triggers, owner, and the automation or manual fallback for each critical
step.

5. METRICS AND NEXT STEPS

State the KPIs, thresholds, and first implementation priorities.

## Honesty And Non-Goals

- Do not assume a billing stack, SLA, or support model the user has not
  confirmed.
- Do not recommend dark-pattern cancellation flows.
- Do not treat payment recovery and voluntary churn as the same problem.
- Do not design enterprise-grade process overhead for a simple self-serve
  business without justification.
- Do not blur broad SaaS operations with deeper product, pricing, or retention
  strategy when another skill owns that boundary.

## Related Skills

- `churn-prevention` for cancel flows and churn-recovery tactics
- `pricing-strategy` for pricing and packaging choices
- `revops` for revenue handoff and CRM process design
- `customer-success` for post-sale service design
