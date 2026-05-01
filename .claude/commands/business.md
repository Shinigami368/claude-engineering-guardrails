---
description: Delegate a business task to the business-lead orchestrator agent
argument-hint: "[task description]"
---

# Business

Delegates the task to the business-lead orchestrator agent.

The business-lead will:
1. Check optional local `.claude/product-marketing-context.md` if it exists
2. If it is missing, ask for the needed product context or proceed with explicit assumptions instead of treating the file as required
3. Create an execution plan (3-5 bullets)
4. Present the plan for your approval
5. On approval: delegate to specialized business agents and invoke skills
6. Track progress and deliver results

## Invoke

Use the Agent tool to spawn the business-lead agent:
- agent: business-lead
- Task: `$ARGUMENTS`

The business-lead has access to 3 specialized agents:
- **marketing-strategist** — Positioning, launch, content, copy, CRO, analytics, sales enablement
- **business-analyst** — Financial planning, market research, customer research, growth metrics
- **customer-ops-manager** — Customer success, billing ops, support SLA, compliance docs

## When to use

- SaaS launch planning and go-to-market strategy
- Marketing execution (copy, content, email, CRO)
- Financial planning (MRR projections, unit economics, fundraising math)
- Market and customer research (TAM, personas, JTBD, competitor analysis)
- Customer operations (onboarding, support, billing, retention)
- Compliance documents (Terms of Service, Privacy Policy drafts)
- Pricing strategy and packaging decisions
- Growth metrics analysis (funnels, cohorts, retention curves)

## Examples

```
/business SaaS launch strategy for my product
/business pricing strategy — 3 tiers
/business draft Terms of Service
/business customer onboarding playbook
/business financial projections — 12 month
/business growth funnel analysis
```
