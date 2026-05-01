# Paywall & Upgrade CRO Experiments

## A/B Test Ideas for Paywall Optimization

### 1. Timing Experiments

| Test | Hypothesis | Success Metric |
|------|------------|----------------|
| Early vs Late | Show paywall after 3 features vs 7 features | Conversion rate |
| Usage-triggered | Show after 5 actions vs time-based | Trial-to-paid |
| Scroll depth | Trigger at 50% vs 80% scroll | Activation + conversion |

### 2. Offer Structure Experiments

| Test | Hypothesis | Success Metric |
|------|------------|----------------|
| Annual vs Monthly | Annual discount drives more conversions | LTV, conversion |
| Feature gating | Gate 1 key feature vs 3 features | Upgrade rate |
| Price anchoring | Show high-tier first vs low-tier first | Average order value |

### 3. Copy Experiments

| Test | Hypothesis | Success Metric |
|------|------------|----------------|
| Value-first vs Problem-first | Lead with benefits vs pain points | Click-through |
| Specific vs Vague | "Save 3 hours/week" vs "Save time" | Trial signups |
| Social proof placement | Add testimonials in paywall vs below | Conversion |

### 4. Visual Experiments

| Test | Hypothesis | Success Metric |
|------|------------|----------------|
| Modal vs Inline | Modal interrupts vs inline expansion | User sentiment |
| Animated vs Static | Animated value props vs static | Attention time |
| Dark vs Light modal | Dark backgrounds feel premium | Conversion |

## Experiment Prioritization Matrix

```
High Impact + Easy to Test = Do First
├── Price anchoring
├── Offer timing
└── CTA copy

High Impact + Hard to Test = Plan Carefully
├── New pricing tiers
├── Freemium model changes
└── Feature gate restructuring

Low Impact + Easy to Test = Quick Wins
├── Button colors
├── Icon changes
└── Microcopy

Low Impact + Hard to Test = Deprioritize
├── Full page redesigns
├── Animation heavy features
└── Non-core feature gating
```

## Statistical Significance Calculator

### Minimum Sample Size (95% confidence, 80% power)

| Baseline Conversion | MDE (Minimum Detectable Effect) | Sample per Variant |
|--------------------|----------------------------------|---------------------|
| 1% | 20% relative | 19,000 |
| 1% | 10% relative | 73,000 |
| 5% | 20% relative | 3,700 |
| 5% | 10% relative | 14,000 |
| 10% | 20% relative | 1,800 |
| 10% | 10% relative | 6,800 |

### Rule of Thumb
- **B2B SaaS**: 50-100 conversions per variant minimum
- **B2C SaaS**: 100-200 conversions per variant minimum
- **E-commerce**: 200-500 conversions per variant minimum

## Multi-Armed Bandit vs A/B Test

| Approach | Best For | Risk |
|----------|----------|------|
| A/B Test | High-stakes decisions, clear winners | Slower to conclude |
| Multi-Armed Bandit | Fast iteration, equal variants | May miss subtle winners |

### When to Switch from Bandit to A/B
1. One variant reaches 95% confidence
2. After 2+ weeks with stable daily conversions
3. When variants are nearly equal at 50/50

## Funnel for Paywall Experiments

```
Impression → Click → Trial Start → Trial Continue → Upgrade → Paid
    ↓           ↓         ↓              ↓              ↓        ↓
 100%        10%        50%           30%            15%      80%
```

### Typical Drop-off Points
1. **Impression → Click**: 90% drop (paywall avoidance)
2. **Click → Trial Start**: 50% drop (friction in signup)
3. **Trial → Upgrade**: 70-85% drop (value not realized)

### Win-Back Experiment Flow
```
Cancel Intent → Save Offer → Accept Save → Retention
                  ↓              ↓            ↓
              Decline       Accept        Decline
                  ↓              ↓            ↓
              Cancel       Cancel        Churn
```

## Testing Save Offers

### Save Offer Hierarchy (Most to Least Effective)
1. **Plan downgrade** - Keep premium, reduce price
2. **Pause subscription** - Temporary relief, easy return
3. **Discount** - Immediate savings, no commitment
4. **Feature limited** - Keep full features, lower price
5. **Free extension** - Delay billing, no change

### Save Offer Timing
| Timing | Best For | Average Retention |
|--------|----------|-------------------|
| Pre-cancel | Soft intent | 60-70% |
| At cancel | Strong intent | 30-40% |
| Post-cancel | Committed to leave | 10-20% |

## Reference Sources
- CXL Institute: Paywall A/B Testing Guide
- Widerfunnel: PIE framework for prioritization
- Optimizely: Statistical significance calculator
