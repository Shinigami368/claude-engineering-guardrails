---
name: frontend-implement
description: Implement user-facing frontend changes with repo-native patterns, responsive checks, and browser-verifiable evidence.
domain: product_design_qa
role: execute_build
scope: bounded_task
power: local_repo_mutation
---

# Skill: frontend-implement

## Purpose / Use When

Use this skill when:
- implementing or updating web UI in an existing repo
- changing components, client state, forms, layout, routing, or interaction behavior
- a design already exists and the main job is shipping the UI correctly
- the user needs code changes plus browser-verifiable evidence

## When Not to Use

Do not use this skill when:
- the task is design exploration only; use `frontend-design`
- the task is site architecture or route planning only; use `website-build`
- the task is backend-only Node.js work; use `node-implement`
- the repo or target UI surface is unknown; start with `repo-navigator`
- the task is native iOS or Android implementation without repo-specific mobile tooling

## Input Expectation

Provide:
- the target route, component, or screen
- acceptance criteria and critical user flows
- design constraints, tokens, breakpoints, or visual references when available
- repo/package context for monorepos
- any accessibility, browser, or performance constraints

## Steps / Tasks

1. Run `repo-navigator` to map the UI entry points, component boundaries, and repo-native test/build commands.
2. If the design is missing or unstable, stop and use `frontend-design` first.
3. If the change alters page structure, route composition, or cross-page layout, use `website-build` before editing.
4. Implement the smallest UI change that satisfies the acceptance criteria.
5. Match existing component, styling, state, and test patterns instead of introducing a new frontend architecture.
6. Verify responsive behavior for the affected flow and preserve semantic HTML, keyboard access, and obvious focus states.
7. Run repo-native quality gates, then use `browser-audit` or `webapp-testing` when user-visible behavior changed.
8. Finish with `self-check`.

## Output Contract

Return:
- the affected UI surfaces
- the implementation summary
- the verification commands that ran
- browser or accessibility evidence, or the reason it could not be collected
- residual risks or follow-ups

## Tools / Commands

- `rg` for route, component, and state lookup
- repo-native package manager scripts for lint, type-check, test, and build
- `node $HOME/.claude/skills/browser-audit/scripts/run_browser_audit.js --help`
- `git diff -- <path>`

## Dependencies

- `repo-navigator`
- `frontend-design`
- `website-build`
- `node-implement`
- `browser-audit`
- `accessibility`
- `webapp-testing`
- `self-check`

## Example

Implement the mobile navigation drawer for an existing React route, keep the current design system tokens, run the package-scoped test suite, then collect mobile and desktop browser evidence with `browser-audit`.
