# Frontend Design Quality Checklist

Use this checklist before handing a visual contract to `website-build` or implementation. It is intentionally small and local: it captures reusable design review patterns without importing external style catalogs.

## Required Contract

- Product goal, primary audience, and strongest user intent are stated in one paragraph.
- Visual direction names what the interface should feel like and what it must avoid.
- Typography defines font family, base size, scale, line height, and weight use.
- Color tokens define background, surface, text, muted text, border, primary action, secondary action, success, warning, and error.
- Spacing uses a named scale instead of one-off values.
- Radius, shadow, border, and motion tokens are explicit.
- Interactive states include default, hover, focus-visible, active, disabled, loading, and error.

## Accessibility Gate

- Focus-visible treatment is defined for every interactive element.
- Color is not the only signal for success, warning, error, selected, or disabled states.
- Text/background contrast target is stated; use WCAG AA as the default floor.
- Tap targets account for mobile touch use.
- Motion respects reduced-motion preferences when animations are part of the contract.

## Responsive Gate

- Mobile behavior is defined first.
- Tablet and desktop breakpoints are named with exact widths or width ranges.
- Navigation behavior is explicit for all breakpoints.
- Long labels and dynamic content cannot resize fixed-format controls, tiles, boards, or toolbars.
- No horizontal overflow is acceptable unless the component is explicitly scrollable.

## Layout Stability Gate

- Cards, tiles, controls, tables, toolbars, boards, and media frames define stable dimensions or explicit wrapping rules.
- Loading, empty, error, and long-content states do not shift surrounding layout unexpectedly.
- User-generated text has a max width, wrapping rule, truncation rule, or expansion pattern.
- Interactive state changes do not move neighboring content.

## Browser Evidence Gate

- The expected `browser-audit` preset is named: Quick, Standard, or Exhaustive.
- Browser-visible changes name the required viewport evidence.
- Known third-party telemetry noise is separated from actionable product findings.
- Any skipped browser evidence is explained in the handoff notes.

## Visual Anti-Patterns

- Avoid one-note palettes dominated by one hue family.
- Avoid generic AI-purple gradient styling unless the product brief specifically justifies it.
- Avoid card-in-card layouts and decorative frames around the primary experience.
- Avoid vague labels such as modern, premium, delightful, or clean unless token-level rules make them concrete.
- Avoid ornamental effects that do not support hierarchy, state, or comprehension.

## Handoff Evidence

The final design contract should include:

- token table
- component state matrix
- responsive behavior notes
- browser evidence preset
- design QA checklist
- any unresolved design decisions that require maintainer input
