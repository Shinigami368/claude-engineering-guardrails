# Content Architecture for Competitor Alternatives Pages

## Data Structure

### Frontmatter Schema
```yaml
---
type: competitor-alternatives
title: "[Your Product] vs [Competitor]"
meta_description: "[SEO description under 160 chars]"
target_competitors:
  - name: "[Competitor Name]"
    url: "[Competitor URL]"
    pricing_url: "[Competitor pricing page]"
comparison_focus:
  - "[Focus Area 1]"
  - "[Focus Area 2]"
  - "[Focus Area 3]"
last_updated: "[YYYY-MM-DD]"
author: "[Author Name]"
---
```

### Comparison Matrix Format
```
| Feature | [Your Product] | [Competitor 1] | [Competitor 2] |
|---------|:---:|:---:|:---:|
| Category: Core Features | | | |
| [Feature A] | ✅ Full | ⚠️ Limited | ❌ None |
| [Feature B] | ✅ | ✅ | ⚠️ |
| Category: Pricing | | | |
| [Pricing Model] | [Details] | [Details] | [Details] |
| [Free Tier] | [Yes/No + Limits] | [Yes/No + Limits] | [Yes/No + Limits] |
| Category: Integrations | | | |
| [Integration Count] | [X+] | [Y+] | [Z+] |
| [Notable Integrations] | [List] | [List] | [List] |
```

### Data Source Format for Automation
```json
{
  "competitors": [
    {
      "name": "[Competitor Name]",
      "founded": [Year],
      "headquarters": "[City, Country]",
      "pricing_model": "[e.g., per seat, usage-based, tiered]",
      "starting_price": [Number],
      "free_tier": true,
      "free_tier_limits": "[Description]",
      "key_strengths": ["[Strength 1]", "[Strength 2]"],
      "key_weaknesses": ["[Weakness 1]", "[Weakness 2]"],
      "best_for": ["[Use Case 1]", "[Use Case 2]"],
      "not_best_for": ["[Use Case 1]", "[Use Case 2]"]
    }
  ]
}
```

## Page Hierarchy

### 1. Headline Section
```
[Main Headline - H1]
[Subheadline with key differentiator - H2]

[Primary CTA Button]  [Secondary Link]

[Quick comparison table - 3-5 rows max]
```

### 2. Comparison Table (Full)
```
## Detailed Comparison

[Full feature matrix with 15-30 rows]

Legend: ✅ Full Support | ⚠️ Limited | ❌ None | [Number] = Limited quantity
```

### 3. In-Depth Sections
```
## [Category 1]
### [Your Product]'s Approach
[2-3 paragraphs]

### [Competitor]'s Approach  
[2-3 paragraphs]

### Verdict: [Category 1]
[Brief recommendation]
```

### 4. Use Case Mapping
```
## Which Should You Choose?

### Choose [Your Product] if:
- ✅ [Use Case A]
- ✅ [Use Case B]  
- ✅ [Use Case C]

### Choose [Competitor] if:
- ⚠️ [Use Case A]
- ⚠️ [Use Case B]
```

### 5. Social Proof
```
## What Customers Say

> "[Quote about specific outcome]" 
> — [Name], [Title] at [Company]

> "[Quote about specific outcome]"
> — [Name], [Title] at [Company]
```

### 6. FAQ / Objection Handling
```
## Frequently Asked Questions

### Q: [Common objection question]
A: [Honest answer that addresses the concern]

### Q: [Pricing question]
A: [Transparent pricing comparison]
```

## Internal Linking Structure

```
[Your Product] Main Page
    │
    ├── Competitor Alternative Pages
    │   ├── vs-[Competitor-1].md
    │   ├── vs-[Competitor-2].md
    │   └── vs-[Competitor-3].md
    │
    ├── Use Case Pages
    │   ├── [use-case-1].md
    │   └── [use-case-2].md
    │
    └── Integration Pages
        ├── [integration-1].md
        └── [integration-2].md
```

## Example: Notion vs. Coda Content Architecture

### Page: notion-vs-coda.md
```
---
type: competitor-alternatives
title: Notion vs. Coda - Which Wiki Tool Wins?
meta_description: Honest comparison of Notion vs. Coda for team wikis and docs.
target_competitors:
  - name: Notion
    url: https://notion.so
    pricing_url: https://notion.so/pricing
  - name: Coda
    url: https://coda.io
    pricing_url: https://coda.io/pricing
comparison_focus:
  - Document editing experience
  - Collaboration features
  - Template library
  - Pricing value
last_updated: 2024-01-15
---

## Headline
# Notion vs. Coda: Which One Should Your Team Use in 2024?

## Quick Verdict Table
| Use Case | Winner |
|----------|--------|
| Best free plan | Notion |
| Best for complex formulas | Coda |
| Best template library | Tie |
| Best mobile experience | Notion |

## Deep Comparison Sections...
```

## SEO Requirements

### Title Tag Formula
```
[Product A] vs [Product B] — [Honest Comparison for 2024] | [Your Brand]
```

### Meta Description Formula
```
Looking for [Product A] vs [Product B] comparison? We break down pricing, 
features, pros & cons to help you choose. Updated [Month Year].
```

### H1 Formula
```
[Product A] vs [Product B]: The [Year] Comparison Guide
```

### URL Structure
```
/[product-a]-vs-[product-b]/
/alternatives/[product-a]/
/competitors/[product-name]/
```

## Common Pitfalls

1. **Biased-only content**: Don't hide competitor weaknesses
2. **Feature bloat**: Focus on what matters, not every tiny feature
3. **Outdated pricing**: Update regularly (set quarterly reminder)
4. **No CTA**: Always give next step (trial, demo, consultation)
5. **Missing FAQ**: Address the "but what about..." questions
