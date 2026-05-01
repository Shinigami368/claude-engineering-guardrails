# A/B Test Sample Size Guide

## Formula

The core formula for minimum sample size per variation:

```
n = (Z_α/2 + Z_β)² × (p₁ × (1-p₁) + p₂ × (1-p₂)) / (p₁ - p₂)²
```

Where:
- `Z_α/2` = Z-score for significance level (1.96 for 95% confidence)
- `Z_β` = Z-score for power (0.84 for 80% power)
- `p₁` = Baseline conversion rate
- `p₂` = Expected conversion rate (minimum detectable effect)

## Simplified Calculator

| Baseline Rate | MDE (Relative) | MDE (Absolute) | Sample/Variation |
|---------------|-----------------|-----------------|-----------------|
| 5% | 10% | 0.5% | 61,000 |
| 5% | 20% | 1.0% | 15,500 |
| 5% | 30% | 1.5% | 7,000 |
| 10% | 10% | 1.0% | 29,000 |
| 10% | 20% | 2.0% | 7,300 |
| 10% | 30% | 3.0% | 3,300 |
| 20% | 10% | 2.0% | 13,500 |
| 20% | 20% | 4.0% | 3,400 |
| 20% | 30% | 6.0% | 1,500 |

*MDE = Minimum Detectable Effect | 95% confidence, 80% power*

## Quick Rules of Thumb

### For 5% conversion rate with 20% relative MDE:
- ~15,000 visitors per variation
- ~30,000 total for A/B test

### For 10% conversion rate with 20% relative MDE:
- ~7,300 visitors per variation
- ~14,600 total for A/B test

### For email (0.5% response rate):
- Need 100,000+ per variation
- Consider Bayesian approaches or hold-out tests

## Duration Estimation

```
Test Duration (days) = Sample Size Needed / Daily Visitors
```

| Daily Visitors | 15K Sample/Var | 30K Sample/Var |
|----------------|-----------------|-----------------|
| 500 | 30 days | 60 days |
| 1,000 | 15 days | 30 days |
| 2,500 | 6 days | 12 days |
| 5,000 | 3 days | 6 days |
| 10,000 | 1.5 days | 3 days |

## Common Mistakes

### ❌ Running tests without power calculation
- "Let's test for a week" often leads to underpowered tests

### ❌ Stopping based on significance alone
- Early stopping inflates false positive rate
- Use sequential testing or always run to calculated duration

### ❌ Testing too many variations
- Each additional variation needs more sample
- 4-way test needs 2x the sample of 2-way test

### ❌ Ignoring seasonal effects
- Run tests for full business cycles (7-14 days minimum)
- Avoid holiday periods unless testing holiday-specific hypotheses

## Tools

- [Evan's Awesome A/B Tools](https://www.evanmiller.org/ab-testing/) - Calculator
- [Google Optimize Sample Size Calculator](https://marketingplatform.google.com/about/optimize/)
- [VWO Bayesian Calculator](https://vwo.com/ab-split-test-significance-calculator/)
- [R package: power.prop.test](https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/power.prop.test)
- [Python: statsmodels.stats.power](https://www.statsmodels.org/stable/generated/statsmodels.stats.power.zt_ind_solve_power.html)

## Advanced: Sequential Testing

For tests where you want to check results mid-test:

### Beta-Binomial Sequential Testing
```
Allow early stopping with proper error rate control
- Install: pip install sequential
- Use: always run to pre-calculated max duration
- Stop early ONLY if results are extreme
```

### Always valid интервалы (Always Valid p-values)
- `lab.js` - Sequential testing library
- `arty` - Always valid p-values in Python
