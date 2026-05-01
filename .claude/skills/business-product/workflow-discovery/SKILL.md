---
name: workflow-discovery
description: "Map, document, and analyze operational workflows for any industry. Use when the user mentions 'map our workflow,' 'document our process,' 'how does our operation work,' 'process mapping,' 'workflow analysis,' 'operational bottleneck,' 'process improvement,' 'value stream,' 'workflow automation,' 'which steps can we automate,' or 'where are we losing time.' Works for any business type — not limited to SaaS."
---

# Skill: workflow-discovery

## When To Activate

Use this skill when:
- the user wants to map or document a current operational workflow
- the task is to find bottlenecks, handoff failures, rework loops, or hidden
  waiting time
- the user is planning automation and needs current-state clarity first
- the team needs a standard process document before improving, measuring, or
  handing off the work

Use `runbook-generator` after the workflow is clear and needs to be converted
into an operational procedure, not while the current process is still being
discovered.

## Context Prerequisites

- Check `.claude/industry-context.md` first if it exists.
- Check `.claude/product-marketing-context.md` when the workflow depends on how
  the product or service is delivered.
- Clarify:
  - process name
  - start trigger
  - end condition
  - actors involved
  - frequency
  - current pain point
- If the workflow spans multiple teams or systems, make those boundaries
  explicit before analysis starts.

## Discovery Questions

- What process is being mapped, and where does it start and end?
- Who performs each part of the work:
  - person
  - team
  - tool
  - system
- What steps happen in sequence, and which ones happen in parallel?
- Where are the decision points, wait states, and exception paths?
- What inputs, outputs, or artifacts move between steps?
- Which handoffs are slow, lossy, or error-prone?
- What currently goes wrong most often?

## Decision Framework

- Map reality first, not the idealized process.
- Follow the flow of work across teams and systems rather than mirroring the
  org chart.
- Treat every handoff as a potential source of delay, information loss, or
  rework.
- Make invisible work visible:
  - shadow work
  - manual copy-paste
  - approval loops
  - waiting time
  - undocumented exceptions
- Separate:
  - current-state mapping
  - issue analysis
  - improvement recommendations
- Only recommend automation after the current-state workflow is understood and
  the repetitive, rule-based parts are visible.

## Output Structure

1. WORKFLOW GOAL

State the process being mapped, the trigger, the outcome, the frequency, and
the actors involved.

2. CURRENT-STATE MAP

Document the actual steps, including:
- actor
- tool or system
- input
- action
- output
- duration or wait time when known

3. DECISION POINTS AND HANDOFFS

State branching logic, cross-team transfers, and the main failure or delay
risks at each handoff.

4. KNOWN ISSUES AND IMPROVEMENT OPPORTUNITIES

Call out bottlenecks, rework loops, single points of failure, automation
candidates, and redesign opportunities.

5. MEASUREMENT AND NEXT STEPS

State the metrics, checkpoints, or follow-on work needed to improve the
workflow.

## Honesty And Non-Goals

- Do not assume the workflow without walking through the actual current state.
- Do not jump straight to the ideal future-state process.
- Do not recommend automation for steps that are still ambiguous or
  exception-heavy.
- Do not hide compliance-relevant steps when industry context suggests they
  matter.
- Do not turn the workflow map into a generic operations essay.

## Related Skills

- `industry-context` for vertical and compliance grounding
- `operations-kpi-scorecard` for measuring the workflows you mapped
- `saas-operations` for SaaS-specific operational workflows
- `observability-designer` for monitoring gaps in technical workflow steps
- `runbook-generator` for converting a stable workflow into an operational
  runbook
