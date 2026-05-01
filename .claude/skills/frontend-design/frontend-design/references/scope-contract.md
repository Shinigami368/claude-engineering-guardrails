# Frontend Skill Boundary Contract

## Skill Order (when both skills are active)
1. `frontend-design`
2. `website-build`

`website-build` MUST consume design decisions from `frontend-design` and must not redefine them unless there is a hard implementation constraint.

## frontend-design

### Inputs
- Product goal and audience
- Brand constraints (if any)
- Required pages/flows
- Platform constraints (web app, marketing site, dashboard)

### Outputs
- Visual system spec (typography, color tokens, spacing scale)
- Component state spec (default/hover/focus/disabled/error/loading)
- Responsive behavior spec (mobile/tablet/desktop)
- Design QA checklist

### This skill does NOT do
- Full implementation handoff task breakdown
- Performance budget calculation
- SEO metadata planning
- Framework-specific architecture decisions

## website-build

### Inputs
- Frontend design spec (from `frontend-design`)
- Feature/page requirements
- Tech stack constraints

### Outputs
- Information architecture and page/section breakdown
- Component contracts (props, states, data dependencies)
- Accessibility/performance/SEO implementation gates
- Build handoff checklist with acceptance criteria

### This skill does NOT do
- Re-invent visual language or design system from scratch
- Art direction exploration (unless design spec is missing)
- Backend domain modeling or infra architecture
