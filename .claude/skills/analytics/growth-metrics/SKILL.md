---
name: growth-metrics
description: "When the user wants to analyze growth funnels, activation/retention metrics, cohort analysis, or define a north star metric. Also use when the user mentions 'funnel analysis,' 'activation rate,' 'retention curve,' 'cohort analysis,' 'north star metric,' 'growth rate,' 'conversion funnel,' 'DAU/MAU,' 'weekly active users,' 'engagement metrics,' 'product metrics,' 'pirate metrics,' 'AARRR,' 'how fast are we growing,' or 'which metrics should I track.' Use this for any quantitative growth analysis for a SaaS product."
---

# Growth Metrics

You help SaaS founders and operators measure, analyze, and improve growth through data-driven funnel analysis, retention tracking, cohort analysis, and metric selection.

## Before Starting

**Check for product marketing context first:**
If `.claude/product-marketing-context.md` exists, read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

---

## Core Principles

### 1. One North Star Metric
Every team needs a single metric that best captures the core value delivered to customers. All other metrics feed into it.

### 2. Leading > Lagging
Revenue is a lagging indicator. Focus on leading indicators (activation, engagement, feature adoption) that predict future revenue.

### 3. Rates > Absolutes
"50 new users" means nothing without context. "12% week-over-week growth" tells a story.

### 4. Cohorts > Aggregates
Aggregate metrics hide trends. Cohort analysis reveals whether you're actually improving over time.

---

## AARRR Framework (Pirate Metrics)

### The Funnel

| Stage | Question | Key Metric |
|-------|----------|------------|
| **Acquisition** | How do users find you? | Visitors, signups by channel |
| **Activation** | Do they have a great first experience? | % reaching "aha moment" |
| **Retention** | Do they come back? | Day 1/7/30 retention, DAU/MAU |
| **Revenue** | Do they pay? | Conversion to paid, ARPU, MRR |
| **Referral** | Do they tell others? | Viral coefficient, NPS |

### Defining Each Stage

For each stage, define:
1. **The event** — What specific action counts?
2. **The timeframe** — Within what window?
3. **The benchmark** — What's "good" for your stage/vertical?

---

## North Star Metric

### Selection Criteria

A good north star metric:
- Reflects core value delivered to customers
- Is a leading indicator of revenue
- Is actionable (teams can influence it)
- Is simple enough to rally around

### Examples by Product Type

| Product Type | North Star Metric |
|-------------|-------------------|
| Collaboration tool | Weekly active teams |
| Analytics platform | Queries run per week |
| Marketplace | Weekly transactions |
| Content platform | Weekly content consumed |
| DevTool / API | Weekly API calls |
| Security tool | Threats detected and resolved |

### Supporting Metrics

The north star needs 3-5 supporting metrics that decompose it:

```
North Star: Weekly Active Teams
├── New teams activated this week
├── Returning teams (retained)
├── Features used per team per week
└── Team members invited per team
```

---

## Funnel Analysis

### Building a Funnel

1. **Define stages** — Map each step from first touch to paid conversion
2. **Instrument events** — Track each transition
3. **Measure conversion** — Calculate % moving between stages
4. **Find the biggest drop** — Focus optimization there
5. **Set targets** — Define "good" for each conversion rate

### Example SaaS Funnel

```
Website Visit        100%
  → Signup           5-10%
  → Activation       40-60%
  → Week 1 Retained  25-40%
  → Paid Conversion   2-5%
  → Month 2 Retained 80-95%
```

### Funnel Diagnosis

| Symptom | Likely Issue | Investigation |
|---------|-------------|---------------|
| Low visit→signup | Weak value prop or targeting | Check messaging, traffic sources |
| Low signup→activation | Onboarding friction | Analyze drop-off steps |
| Low activation→retention | Product doesn't deliver value | User interviews, feature usage |
| Low retention→paid | Pricing or packaging problem | Check willingness to pay, plans |

---

## Retention Analysis

### Retention Curves

**Types:**
- **User retention** — % of users active in period N
- **Revenue retention** — % of revenue retained (net of churn + expansion)
- **Feature retention** — % still using a specific feature

### Healthy Retention Benchmarks (SaaS)

| Timeframe | Consumer | SMB SaaS | Enterprise SaaS |
|-----------|----------|----------|-----------------|
| Day 1 | 40%+ | 60%+ | 80%+ |
| Day 7 | 20%+ | 40%+ | 70%+ |
| Day 30 | 10%+ | 30%+ | 60%+ |
| Month 12 | — | 70%+ (logo) | 85%+ (logo) |

### Retention Curve Shape

- **Flattening curve** = Good. Users who stay past a threshold stick around.
- **Declining curve** = Bad. Even long-term users are leaving.
- **Smiling curve** = Great. Users come back after initial drop (resurrection).

### DAU/MAU Ratio

- **50%+** = Exceptional (daily habit product)
- **25-50%** = Good (regular use product)
- **10-25%** = Average (weekly use product)
- **<10%** = Concerning (infrequent use)

---

## Cohort Analysis

### Building Cohorts

Group users by:
- **Time-based** — Sign-up week/month (most common)
- **Behavior-based** — First action taken, activation path
- **Source-based** — Acquisition channel, campaign
- **Plan-based** — Free vs. paid, plan tier

### Reading a Cohort Table

```
Cohort    M0    M1    M2    M3    M4
Jan       100%  45%   38%   35%   34%
Feb       100%  48%   42%   39%   —
Mar       100%  52%   46%   —     —
Apr       100%  55%   —     —     —
```

**What to look for:**
- Are newer cohorts retaining better? (column comparison)
- Where is the biggest drop? (row analysis)
- Is there a flattening point? (when does churn stabilize)

---

## Engagement Metrics

### Feature Adoption

| Metric | Formula | Use |
|--------|---------|-----|
| Feature adoption rate | Users using feature / Total active users | Which features matter |
| Feature frequency | Avg uses per user per period | How deeply features are used |
| Feature breadth | Avg features used per user | How broadly product is used |
| Stickiness | DAU / MAU | How habitual the product is |

### Engagement Scoring

Create a composite engagement score:

1. **Define key actions** — List 5-10 meaningful product actions
2. **Weight by value** — Assign importance weights
3. **Score users** — Sum weighted actions per period
4. **Segment** — Power users, regular, casual, dormant
5. **Track movement** — Are users moving up or down?

---

## Growth Rate Metrics

### Key Growth Metrics

| Metric | Formula | Benchmark |
|--------|---------|-----------|
| MoM Growth | (This month - Last month) / Last month | 15-20% early stage |
| Quick Ratio | (New MRR + Expansion) / (Contraction + Churn) | >4 excellent, >2 good |
| Viral Coefficient | Invites sent × conversion rate | >1 = viral growth |
| Payback Period | CAC / (ARPU × Gross Margin) | <12 months |

### Growth Accounting

```
Start of Period Users: 1000
  + New Users:          200
  + Resurrected Users:   30
  - Churned Users:       80
= End of Period Users: 1150
Net Growth Rate: 15%
```

---

## Output Format

### Metrics Dashboard Specification

```
# Growth Metrics Dashboard — [Product Name]

## North Star
- Metric: [name]
- Current: [value]
- Target: [value]
- Trend: [improving/flat/declining]

## Funnel (Last 30 Days)
| Stage | Count | Conversion | Target | Status |
|-------|-------|-----------|--------|--------|

## Retention (Latest Cohort)
| Period | Retention | Benchmark | Status |
|--------|----------|-----------|--------|

## Key Cohort Insights
-

## Growth Health
- Quick Ratio: [value]
- MoM Growth: [value]%
- DAU/MAU: [value]

## Recommendations
1.
2.
3.
```

---

## Task-Specific Questions

1. What stage is your product? (pre-launch, early, growth, scale)
2. What metrics are you currently tracking?
3. What does "active user" mean for your product?
4. What's your current retention curve look like?
5. What's your primary growth channel?

---

## Related Skills

- **financial-planning**: For revenue projections and unit economics
- **analytics-tracking**: For implementing metric tracking
- **customer-research**: For qualitative context behind metrics
- **pricing-strategy**: For conversion and monetization optimization
- **onboarding-cro**: For activation rate improvement
