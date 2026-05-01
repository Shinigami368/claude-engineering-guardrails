# Dunning & Payment Recovery Playbook

## What is Dunning?

Dunning = systematic process of recovering failed payments and preventing involuntary churn.

**Involuntary Churn**: Customer wants to stay but payment fails
**Voluntary Churn**: Customer actively cancels

Involuntary churn is often 2-3x higher than voluntary churn.

---

## The Dunning Timeline

### Day 0: Payment Fails
```
→ Send immediate notification (soft fail)
→ Retry in 3-5 days
→ Retry in 7-10 days
→ Send final warning
→ Account suspension/cancellation
```

### Recommended Schedule
| Attempt | Day | Action |
|---------|-----|--------|
| 1 | Day 0 | First retry (soft) |
| 2 | Day 5 | Retry + email |
| 3 | Day 10 | Retry + urgent email |
| 4 | Day 15 | Account at risk + email |
| 5 | Day 20 | Final warning |
| 6 | Day 25 | Suspend account |

---

## Email Templates

### Attempt 1: Friendly Reminder
```
Subject: Quick heads up — payment didn't go through

Hi [First Name],

We tried to charge the card ending in [last 4] 
for your [Plan Name] subscription, 
but the payment didn't go through.

This usually happens when:
- Your card has expired
- Your bank flagged the transaction
- There aren't sufficient funds

No worries — it's an easy fix:

[Update Payment Method]

Your subscription will continue as normal 
once we receive payment.

Questions? Reply to this email.

— The [Company] Team
```

### Attempt 2: More Urgent
```
Subject: Action required — update your payment info

Hi [First Name],

We weren't able to process your payment for 
[Plan Name] on [date].

Your subscription is at risk of being paused 
if we don't receive payment within 7 days.

[Update Payment Now]

If your card is up to date, it's possible 
your bank blocked the transaction. 
Try a different card or contact your bank.

— The [Company] Team
```

### Attempt 3: Final Warning
```
Subject: Last chance — subscription pauses [date]

Hi [First Name],

This is your final notice.

We haven't been able to process payment 
for [Plan Name] after multiple attempts.

Your subscription will be PAUSED on [date].

[Update Payment Now — Last Chance]

After suspension, you'll lose access to:
- [Feature 1]
- [Feature 2]
- [Feature 3]

We'll keep your data for 30 days after pause.

Questions? Reply immediately.

— The [Company] Team
```

---

## Key Strategies

### 1. Smart Retry Logic
```markdown
Retry times:
- Immediate (soft decline might clear)
- 1 day (common for temporary holds)
- 3 days
- 7 days
- 14 days

Card decline codes:
- "Insufficient funds" → More aggressive (7 day)
- "Expired card" → Update card link prominent
- "Do not honor" → Likely bank-specific, different card needed
- "Lost/stolen" → Don't retry, flag for customer outreach
```

### 2. Payment Method Updating
Make updating payment EASY:
- One-click link from email
- No logging in required (magic link or token)
- Multiple payment options (card, PayPal, bank)
- Clear instructions

### 3. Retention Bump
Offer something small to recover:
```
"We noticed you're having payment issues.
As a thank you for being a customer, 
here's 10% off your next month."
```

### 4. Alternative Payment Methods
| Method | Use Case |
|--------|----------|
| PayPal | Card declined repeatedly |
| Bank Transfer (ACH) | US customers, lower fees |
| Wire Transfer | Enterprise, large amounts |
| Crypto | International, tech customers |

---

## Prevention Tactics

### Before Payment Fails

1. **Card Expiry Alerts**
   - Send email 30 days before card expires
   - Update link in email

2. **Pre-authorization**
   - Run small $1 charge at signup to validate card
   - Check card validity without charging

3. **AccountUpdater Integration**
   - Visa/Mastercard account updating service
   - Automatically update saved cards when new card is issued
   - Reduces decline rates by 10-30%

4. **Grace Period**
   - 3-7 day grace after failed payment
   - Don't suspend immediately
   - Send reminder, then retry

---

## Metrics to Track

| Metric | Target | Formula |
|--------|--------|---------|
| **Recovery Rate** | >60% | Recovered / Failed |
| **Dunning Conversion** | >30% | Converted / At-risk |
| **Time to Recover** | <5 days | Average |
| **Involuntary Churn Rate** | <2% | Failed payments / Total |
| **Email Open Rate** | >50% | Dunning emails |

---

## Tools & Platforms

### Dunning Platforms
- **Churn Buster** - Specialized dunning
- **Rocketr** - Payment recovery
- **Maximizer** - Enterprise dunning
- **Stripe** - Built-in retry logic + Smart Retries

### Payment Providers with Smart Retry
- Stripe (Smart Retries - ML-powered)
- Braintree (Retry schedule)
- Recurly (Dunning automation)

### Alert Services
- **Churn Buster** - Payment failure alerts
- **Baremetrics** - Revenue analytics + alerts

---

## Common Mistakes

### ❌ Retrying Too Fast
- Don't retry within 24 hours
- Banks need time to clear temporary holds

### ❌ Retrying Too Slow
- Don't wait 2+ weeks
- Customer forgets, loses momentum

### ❌ No Clear CTA
- Every email needs ONE clear action
- "Update Payment" button above the fold

### ❌ Guilt-Tripping
- Don't use aggressive language
- Don't threaten or shame

### ❌ No Personalization
- Use first name, plan name, amount
- Don't send template text that looks automated
