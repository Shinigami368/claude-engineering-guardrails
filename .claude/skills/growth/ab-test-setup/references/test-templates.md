# A/B Test Templates

## Template 1: Two-Way Test (A/B)

```markdown
# A/B Test Plan: [Test Name]

## Hypothesis
[Hypothesis in format: "If we [change], then [metric] will [increase/decrease] 
by [X%] because [reason]."]

## Primary Metric
[One metric to make the decision: conversion rate, CTR, revenue, etc.]

## Secondary Metrics
- [Metric 1] — [what we'll learn from it]
- [Metric 2] — [what we'll learn from it]

## Guardrail Metrics
- [Metric that should NOT decrease]
- [Metric that should NOT decrease]

## Variant A (Control)
[Current version description]

## Variant B (Treatment)
[What changes in the new version]

## Randomization Unit
[User / Session / Page View]

## Minimum Sample Size
[Calculate using sample size calculator]
- Baseline rate: [X%]
- MDE: [X% relative / absolute]
- Power: 80%
- Significance: 95%

## Test Duration
- Estimated: [X] days
- Must run at least: [X] days
- Reason: [business cycle consideration]

## Launch Criteria
- Statistical significance: p < 0.05
- Minimum sample: [X] per variation
- Direction: [Primary metric must move in expected direction]

## Rollback Criteria
- [Guardrail metric drops by >X%]
- [Any unexpected behavior]

## Technical Notes
[Implementation details, tracking setup, etc.]
```

## Template 2: Multi-Variate Test (A/B/C/D)

```markdown
# Multi-Variate Test Plan: [Test Name]

## Hypothesis
[Overall hypothesis - what you're trying to learn]

## Test Design
| Variation | Description | Traffic Split |
|-----------|-------------|---------------|
| A (Control) | [Current version] | 25% |
| B | [Change 1] | 25% |
| C | [Change 2] | 25% |
| D | [Change 1 + 2] | 25% |

## Primary Metric
[One metric]

## Multiple Comparison Correction
Method: [Bonferroni / Holm-Bonferroni / Benjamini-Hochberg]
Adjusted alpha: [0.05/4 = 0.0125 for Bonferroni]

## Analysis Plan
1. Check overall significance (chi-square or ANOVA)
2. If significant, compare each variant to control
3. Apply correction for multiple comparisons
4. Report winning variation with adjusted p-value

## Sample Size
Per variation: [X]
Total: [X × 4]

## Duration
[X] days minimum
```

## Template 3: Redirect Test (Split URL)

```markdown
# Redirect Test Plan: [Test Name]

## Hypothesis
[If we implement [completely different page], then [metric] will [change] 
by [X%] because [reason].]

## Test Type
Split URL redirect (not inline A/B)

## URLs
| Variation | URL | Purpose |
|-----------|-----|---------|
| A (Control) | /original-page | Current experience |
| B (Treatment) | /test-page | New design |

## Technical Implementation
- Redirect at [load balancer / CDN / tag manager]
- Random assignment based on: [cookie / IP / user ID]
- Persist assignment across sessions: [Yes/No]

## Tracking Considerations
- Ensure both URLs fire same tracking events
- Check UTM parameter handling
- Verify conversion attribution

## Primary Metric
[One metric]

## Sample Size
Same as two-way test formula

## Duration
[X] days minimum
```

## Template 4: Bandit Test (Thompson Sampling)

```markdown
# Multi-Armed Bandit Test: [Test Name]

## When to Use
- Want to minimize "regret" (lost conversions during test)
- Testing many variations (4+)
- Automated optimization desired

## Test Design
| Arm | Description | Initial Weight |
|-----|-------------|----------------|
| A | [Control] | 25% |
| B | [Variant 1] | 25% |
| C | [Variant 2] | 25% |
| D | [Variant 3] | 25% |

## Algorithm
Thompson Sampling with Beta-Binomial conjugate

## Exploration Settings
- Initial exploration: 50% random, 50% learned
- Minimum exploration: 10% (never fully stop exploring)
- Learning rate: [per event / daily refresh]

## Monitoring
- Daily check: no single arm should get >60% traffic
- Weekly review: arm performance rankings
- Monthly: evaluate if test is conclusive

## Switch to A/B if:
- One arm reaches 95% probability of being best
- 30 days elapsed with stable rankings
- Business decides to "lock in" winner

## Tools
- [VWO](https://vwo.com/smart-code/) - Built-in bandit
- [Optimizely](https://www.optimizely.com/) - Multi-armed bandit
- Custom: [Thompson Sampling Python implementation]
```

## Template 5: Hold-Out Validation

```markdown
# Hold-Out Validation Plan

## Purpose
Confirm A/B test results before full rollout

## When to Use
- High-stakes tests with major business impact
- Tests showing surprising/non-intuitive results
- When stakeholder buy-in is uncertain

## Design
1. Run A/B test normally (80% of traffic)
2. Hold back 20% as hold-out group
3. Apply winner to hold-out group
4. Compare hold-out results to original test results

## Validation Criteria
| Metric | Original Test | Hold-Out | Tolerance |
|--------|---------------|----------|-----------|
| [Metric 1] | +X% | +Y% | ±20% relative |
| [Metric 2] | +X% | +Y% | ±20% relative |

## Interpretation
- ✅ Hold-out confirms: Safe to roll out to 100%
- ⚠️ Hold-out differs: Investigate difference before rollout
- ❌ Hold-out contradicts: Do not rollout, re-test

## Timeline
- Original test: [X] days
- Hold-out validation: [X] days
- Total: [X] days
```

## Common Test Parameters

| Parameter | Value | Notes |
|-----------|-------|-------|
| Significance level (α) | 0.05 | 95% confidence |
| Power (1-β) | 0.80 | 80% chance of detecting true effect |
| MDE (relative) | 20% | Minimum clinically/practically meaningful |
| Minimum duration | 7 days | Capture full weekly cycles |
| Maximum duration | 30 days | Avoid seasonal/hotjar effects |
| Traffic allocation | 50/50 | Default for equal sample sizes |
