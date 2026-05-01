# Programmatic SEO Playbooks

## Overview

Programmatic SEO = creating hundreds/thousands of pages automatically using templates + data.

## Core Playbook Types

### 1. Location Pages

```
Template: /[city]/[service].html
Data Source: City database + Service list
Output: 500 cities × 10 services = 5,000 pages
```

#### Data Requirements
| Data Point | Source | Update Frequency |
|------------|--------|------------------|
| City name, state, population | Census data, GeoDB | Annual |
| Local keywords | Google Keyword Planner | Monthly |
| Local competitors | Google Maps scraping | Quarterly |
| Reviews/ratings | Google Places API | Weekly |

#### Content Template Structure
```markdown
# [Service] in [City, State]

## Intro (50-80 words)
Local [service] in [City]. [Unique value prop] serving
[City] and surrounding areas since [year].

## Services Offered
- [Service 1]
- [Service 2]
- [Service 3]

## Why Choose Us in [City]
- [Local differentiator 1]
- [Local differentiator 2]
- [Local differentiator 3]

## Frequently Asked Questions
### Question about [City] [Service]?
[Answer...]

## Contact Us
[City] Location details + contact form
```

### 2. Comparison Pages

```
Template: /[product1]-vs-[product2].html
Data Source: Product database + review data
Output: N×(N-1)/2 comparison pages
```

#### Comparison Page Structure
```markdown
# [Product A] vs [Product B]

## Quick Verdict
[One sentence comparison at a glance]

## Side-by-Side Comparison
| Feature | [Product A] | [Product B] |
|---------|-------------|--------------|

## [Category] Comparison
### Pricing
[Detailed pricing analysis]
### Features
[Feature-by-feature breakdown]
### Pros and Cons
[Bullet lists for each]
```

### 3. Integration Pages

```
Template: /[product]-integrations/[integration].html
Data Source: Integration database + user reviews
Output: 100 products × 50 integrations = 5,000 pages
```

#### Integration Page Template
```markdown
# [Integration Name] Integration with [Product]

## Overview
[Integration description and use case]

## How to Connect
1. Step-by-step setup instructions
2. Configuration options
3. Troubleshooting tips

## Key Features
- Feature 1 with screenshot
- Feature 2 with screenshot

## Use Cases
- [Use case 1]
- [Use case 2]

## Pricing Impact
[Integration cost and product pricing interaction]
```

### 4. FAQ/Question Pages (People Also Ask)

```
Template: /questions/[long-tail-question].html
Data Source: Google Search Console + Quora + Reddit
Output: Top 1,000 questions × 1 = 1,000 pages
```

#### Question Page Template
```markdown
# [Question]

## Short Answer
[2-3 sentence direct answer]

## Detailed Answer
[Comprehensive 300-500 word answer]

## Related Questions
- [Related question 1]
- [Related question 2]

## Sources
[Cited sources with links]
```

## Data Pipeline Architecture

```
┌─────────────┐     ┌──────────────┐     ┌─────────────┐
│ Data Source │ ──▶ │  Transform   │ ──▶ │   Output    │
│  (CSV/JSON) │     │  (Python)    │     │  (Markdown) │
└─────────────┘     └──────────────┘     └─────────────┘
      │                    │                     │
      ▼                    ▼                     ▼
  Raw data           Clean + enrich         Template render
  Unstructured       Add geo/meta           Static HTML/MD
```

## Quality Checklist

### On-Page SEO
- [ ] Unique <title> per page
- [ ] Unique <meta description> per page
- [ ] Proper heading hierarchy (single H1)
- [ ] Internal linking strategy
- [ ] Schema markup (FAQ, LocalBusiness, Product)
- [ ] Image alt text
- [ ] Canonical URLs
- [ ] XML sitemap inclusion

### Content Quality
- [ ] Minimum 300 words per page
- [ ] No duplicate content across pages
- [ ] Actual value vs thin template content
- [ ] Freshness signals (date, updates)
- [ ] User engagement signals considered

### Technical
- [ ] Page load speed < 3s
- [ ] Mobile responsive
- [ ] Proper URL structure
- [ ] No broken links
- [ ] JavaScript-renderable (if needed)

## Scaling Strategy

### Tiered Approach
| Tier | Pages | Quality Bar | Update Freq |
|------|-------|-------------|-------------|
| High-value | 100-500 | 500+ words | Weekly |
| Mid-value | 500-2000 | 300-500 words | Monthly |
| Low-value | 2000-10000 | 200-300 words | Quarterly |

### When to Deprecate Pages
- Zero organic traffic after 6 months
- Thin content with no improvement path
- Cannibalizes high-performing pages
- Updates require constant maintenance

## Tools & Resources
- Screaming Frog (crawl + audit)
- Surfer SEO (content guidelines)
- PageSpeed Insights (performance)
- Google Search Console (ranking data)
- Ahrefs (keyword research + competitor analysis)
