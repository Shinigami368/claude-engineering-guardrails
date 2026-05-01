# Cancel Flow Patterns

## The 5 Exit Points

```
User clicks cancel
       ↓
[1] Cancellation Reason Survey
       ↓
[2] Save Offer (1st intervention)
       ↓
[3] Save Offer (2nd intervention)  
       ↓
[4] Downgrade Option
       ↓
[5] Final Cancellation
```

## 1. Cancellation Reason Survey

### What to Ask
```markdown
# Why are you canceling?

□ No longer using it
□ Too expensive
□ Missing features I need
□ Switching to a competitor
□ [Competitor name]
□ Found a better solution
□ Other: _______________
```

### Best Practices
- Limit to 4-6 options
- Include "Other" with text field
- Don't make required (reduces completion)
- Include "Switching to [specific competitor]" option
- Use single-select (easier to analyze)

### What NOT to Do
- ❌ Don't ask for email/phone again
- ❌ Don't have 10+ options (analysis paralysis)
- ❌ Don't require detailed written feedback
- ❌ Don't start with pricing options

## 2. Save Offers (1st Intervention)

### The "Pause" Offer
```
"Can't find the time? Pause your subscription instead.

Take a break for up to [X] months. 
We'll keep your data and settings exactly as you left them."

[Continue with Pause] [Continue Canceling]
```

**When to use**: Users citing "no time" as reason

### The "Discount" Offer
```
"We'd hate to see you go. 

As a thank you for being a valued customer, 
we'd like to offer you [X]% off your next [Y] months."

[Accept Offer] [Continue Canceling]
```

**When to use**: Users citing "too expensive" as reason

### The "Feature Roadmap" Offer
```
"We heard you — [specific feature they mentioned].

Good news: We're launching it on [date]. 
Want us to notify you the moment it's live?"

[Notify Me] [Continue Canceling]
```

**When to use**: Users citing "missing features"

### The "Talk to Us" Offer
```
"Before you go, we'd love to chat.

Our team might be able to create a custom 
setup that works better for you."

[Chat with Us] [Continue Canceling]
```

**When to use**: High-value customers (check CRM data first)

## 3. Save Offers (2nd Intervention)

### After Discount Rejected
```
"We get it — this might not be the right time.

How about we lock in your current price 
for the rest of this year?

You keep all your current features, 
and you can cancel anytime."

[Lock In Price] [Continue Canceling]
```

### After Pause Rejected
```
"If you just need a break, here's what we can do:

We'll give you a free [X]-day extension 
on top of your current billing period.

That's [Y] extra weeks to try 
everything without paying anything."

[Get Extension] [Continue Canceling]
```

## 4. Downgrade Option

```
"Before you cancel completely:

We have a free plan with the essentials. 
No credit card required. Keep your data."

┌─────────────────────────────┐
│ [Downgrade to Free]         │
│ [Continue Canceling]       │
└─────────────────────────────┘
```

### Downgrade Tiers to Consider
| Tier | Price | Features |
|------|-------|----------|
| Free Forever | $0 | Core features, limited usage |
| Lite | $X/mo | Basic everything |
| Pay-as-you-go | $X/use | No commitment |

## 5. Final Cancellation

### Confirmation Screen
```
# Ready to cancel?

We're sorry to see you go.

Your subscription will end on [date].
You'll still have access until then.

We'll send a confirmation to [email].

[Confirm Cancellation] [Change Mind]
```

### Post-Cancel Win-Back
```
Subject: "We hate to see you go — here's [X] for your next visit"

[For customers canceling with competitor mentioned]
```

## Cancel Flow Best Practices

### DO
- ✅ Make cancel button visible (don't hide it)
- ✅ Use a separate page/modal for cancel flow
- ✅ Show empathy ("We're sorry to see you go")
- ✅ Offer alternatives before final cancel
- ✅ Keep form short (max 30 seconds to complete)
- ✅ Show what they're losing (feature list)
- ✅ Time delays between save offers (3-5 seconds)
- ✅ Personalize based on cancellation reason
- ✅ Honor cancellation immediately (don't delay)

### DON'T
- ❌ Dark patterns (confusing wording, tiny cancel buttons)
- ❌ Long surveys (kills completion rate)
- ❌ Multiple pages for simple cancel
- ❌ Skip save offers (you're leaving money on table)
- ❌ Make save offers auto-selected
- ❌ guilt-trip or shame the user
- ❌ Delay the cancellation process
- ❌ Keep charging after confirmed cancel

## A/B Test Ideas

| Test | Hypothesis |
|------|------------|
| Save offer timing | Save offers at step 1 vs step 2 convert better |
| Number of save offers | 1 vs 2 vs 3 offers before final cancel |
| Discount amount | 20% vs 30% vs 50% |
| Pause vs Discount | Pause option vs discount vs free month |
| Form length | 3 options vs 6 options |
| Button copy | "Cancel" vs "Continue Canceling" |
