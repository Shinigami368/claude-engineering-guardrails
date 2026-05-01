# Schema Markup Examples

## Organization Schema

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "[Company Name]",
  "url": "https://[domain].com",
  "logo": "https://[domain].com/logo.png",
  "sameAs": [
    "https://twitter.com/[handle]",
    "https://linkedin.com/company/[handle]",
    "https://github.com/[handle]"
  ],
  "contactPoint": {
    "@type": "ContactPoint",
    "email": "hello@[domain].com",
    "contactType": "customer service"
  }
}
```

---

## FAQ Schema

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[Question 1]?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Answer 1]"
      }
    },
    {
      "@type": "Question",
      "name": "[Question 2]?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Answer 2]"
      }
    }
  ]
}
```

---

## Product Schema

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "[Product Name]",
  "description": "[Product description]",
  "image": "https://[domain].com/product.jpg",
  "brand": {
    "@type": "Brand",
    "name": "[Brand Name]"
  },
  "offers": {
    "@type": "Offer",
    "price": "[Price]",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock",
    "seller": {
      "@type": "Organization",
      "name": "[Company Name]"
    }
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "reviewCount": "124"
  }
}
```

---

## Article / Blog Schema

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "[Article Title]",
  "description": "[Meta description]",
  "image": "https://[domain].com/og-image.jpg",
  "author": {
    "@type": "Person",
    "name": "[Author Name]",
    "url": "https://[domain].com/author/[slug]"
  },
  "publisher": {
    "@type": "Organization",
    "name": "[Company Name]",
    "logo": {
      "@type": "ImageObject",
      "url": "https://[domain].com/logo.png"
    }
  },
  "datePublished": "[ISO date]",
  "dateModified": "[ISO date]",
  "mainEntityOfPage": {
    "@type": "WebPage",
    "@id": "[Canonical URL]"
  }
}
```

---

## HowTo Schema

```json
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "name": "[How-To Title]",
  "description": "[Description]",
  "totalTime": "PT30M",
  "estimatedCost": {
    "@type": "MonetaryAmount",
    "currency": "USD",
    "value": "0"
  },
  "supply": [
    {
      "@type": "HowToSupply",
      "name": "[Supply 1]"
    }
  ],
  "tool": [
    {
      "@type": "HowToTool",
      "name": "[Tool 1]"
    }
  ],
  "step": [
    {
      "@type": "HowToStep",
      "name": "[Step 1]",
      "text": "[Step 1 description]",
      "image": "https://[domain].com/step1.jpg"
    }
  ]
}
```

---

## Event Schema

```json
{
  "@context": "https://schema.org",
  "@type": "Event",
  "name": "[Event Name]",
  "description": "[Event description]",
  "startDate": "[ISO date]",
  "endDate": "[ISO date]",
  "eventStatus": "https://schema.org/EventScheduled",
  "eventAttendanceMode": "https://schema.org/OnlineEventAttendanceMode",
  "location": {
    "@type": "VirtualLocation",
    "url": "[Event URL]"
  },
  "performer": {
    "@type": "Person",
    "name": "[Speaker Name]"
  },
  "organizer": {
    "@type": "Organization",
    "name": "[Company Name]"
  },
  "offers": {
    "@type": "Offer",
    "price": "[Price]",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  }
}
```

---

## Local Business Schema

```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "[Business Name]",
  "image": "https://[domain].com/store.jpg",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[Street Address]",
    "addressLocality": "[City]",
    "addressRegion": "[State]",
    "postalCode": "[ZIP]",
    "addressCountry": "[Country]"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "[Lat]",
    "longitude": "[Lng]"
  },
  "telephone": "[Phone]",
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "09:00",
      "closes": "17:00"
    }
  ]
}
```

---

## Breadcrumb Schema

```json
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    {
      "@type": "ListItem",
      "position": 1,
      "name": "Home",
      "item": "https://[domain].com"
    },
    {
      "@type": "ListItem",
      "position": 2,
      "name": "[Category]",
      "item": "https://[domain].com/[category]"
    },
    {
      "@type": "ListItem",
      "position": 3,
      "name": "[Page Title]",
      "item": "https://[domain].com/[category]/[page]"
    }
  ]
}
```

---

## Video Schema

```json
{
  "@context": "https://schema.org",
  "@type": "Video",
  "name": "[Video Title]",
  "description": "[Video description]",
  "thumbnailUrl": "https://[domain].com/thumb.jpg",
  "uploadDate": "[ISO date]",
  "duration": "PT5M30S",
  "contentUrl": "https://[domain].com/video.mp4",
  "embedUrl": "https://[domain].com/player",
  "publisher": {
    "@type": "Organization",
    "name": "[Company Name]",
    "logo": {
      "@type": "ImageObject",
      "url": "https://[domain].com/logo.png"
    }
  }
}
```

---

## Testing Your Schemas

| Tool | URL |
|------|-----|
| Rich Results Test | https://search.google.com/test/rich-results |
| Schema Markup Validator | https://validator.schema.org |
| JSON-LD Playground | https://json-ld.org/playground |
| Ahrefs Schema Checker | https://ahrefs.com/tools/schema-markup-generator |
