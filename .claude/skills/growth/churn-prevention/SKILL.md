---
name: churn-prevention
description: "When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or implement retention strategies. Also use when the user mentions 'churn,' 'cancel flow,' 'offboarding,' 'save offer,' 'dunning,' 'failed payment recovery,' 'win-back,' 'retention,' 'exit survey,' 'pause subscription,' 'involuntary churn,' 'people keep canceling,' 'churn rate is too high,' 'how do I keep users,' or 'customers are leaving.' Use this whenever someone is losing subscribers or wants to build systems to prevent it. For post-cancel win-back email sequences, see email-sequence. For in-app upgrade paywalls, see paywall-upgrade-cro."
---

# Skill: churn-prevention

## When To Activate

Use this skill when:
- the user needs to reduce voluntary or involuntary churn
- the task is cancel-flow design, save offers, or offboarding strategy
- the user needs dunning, failed-payment recovery, or win-back structure
- retention risk needs to be addressed before customers fully cancel

Use `saas-operations` when the main problem is the broader subscription
operating model rather than churn-specific intervention.

## Context Prerequisites

- Check `.claude/product-marketing-context.md` first if it exists.
- Clarify:
  - current churn rate
  - voluntary versus involuntary split
  - active subscriber base
  - ARPU or MRR per customer
  - billing provider
  - existing cancel flow or dunning setup
  - available usage or cancellation-reason data
- Clarify whether the user needs:
  - a new cancel flow
  - retention optimization
  - dunning design
  - proactive churn prevention

Use the bundled references for deeper cancel-flow and dunning patterns:
- [references/cancel-flow-patterns.md](references/cancel-flow-patterns.md)
- [references/dunning-playbook.md](references/dunning-playbook.md)

## Discovery Questions

- What kind of churn is driving the problem?
- What do customers say when they leave?
- What save offers or downgrade paths exist today?
- What signals indicate a customer is at risk before cancellation?
- How easy or regulated must cancellation be?
- What tools or data can support dynamic offers or proactive outreach?

## Decision Framework

- Separate voluntary churn and involuntary churn before proposing fixes.
- Match save offers to the cancellation reason rather than using one generic
  discount.
- Keep cancellation clear and non-deceptive while still offering thoughtful
  alternatives.
- Use proactive risk signals when the business can act before cancellation.
- Design dunning as an operational recovery system, not just an email sequence.
- Measure save rate, recovery rate, and long-term retention, not only immediate
  cancellations avoided.

Important churn areas may include:
- exit survey and cancellation-reason taxonomy
- dynamic save-offer mapping
- pause, downgrade, and support-escalation flows
- dunning retries and payment-recovery timing
- pre-churn risk signals and health scoring
- post-cancel win-back logic

## Output Structure

1. CHURN PROBLEM

State whether the problem is voluntary, involuntary, or mixed.

2. CURRENT LEAKS

State what the existing flow or system is missing.

3. INTERVENTION DESIGN

Provide the cancel-flow, dunning, or proactive-retention design.

4. OFFER AND ESCALATION LOGIC

State the save-offer rules, owner, and escalation path.

5. METRICS AND TEST PLAN

State what should be measured and what should be tested first.

## Honesty And Non-Goals

- Do not use dark patterns in cancellation or retention flows.
- Do not treat all churn as price sensitivity.
- Do not assume discounts are the right save offer without evidence.
- Do not promise retention gains from tactic changes alone.
- Do not collapse churn prevention into generic customer-success advice without
  identifying the actual leak.

## References

- Cancel flow patterns: [references/cancel-flow-patterns.md](references/cancel-flow-patterns.md)
- Dunning playbook: [references/dunning-playbook.md](references/dunning-playbook.md)
