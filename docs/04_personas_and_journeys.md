# Personas & Journeys

**Who Uses UCP in India — And Where They Drop Off**

---

## Persona Overview

| Persona | Archetype | UCP Fit |
|---------|-----------|---------|
| Priya | Tier-2 Value Buyer | Medium |
| Ramesh | Trust-First Buyer | Low |
| Arjun | D2C Repeat Buyer | High |
| Meena | SMB Merchant Owner | High |

---

## Persona 1: Priya — Tier-2 Value Buyer

![Persona Cards](https://raw.githubusercontent.com/VIKAS9793/UCP-integration-Indian-consumer-market/main/assets/persona_cards.png)

### Profile
- **Age:** 28
- **Location:** Jaipur, Rajasthan
- **Income:** ₹6-8 lakh/year
- **Device:** Android smartphone (₹15,000 range)
- **Shopping Behavior:** 4-6 orders/month, mostly fashion and home

### Pain Points
- Compares prices across 3-4 apps before buying
- Frustrated by account creation on new sites
- Uses COD for 50% of orders (trust + returns flexibility)
- Abandons cart if extra charges appear at checkout

### Job To Be Done
> "Help me find the best deal and complete purchase without hassle, but let me pay on delivery if I'm unsure."

### Current Journey

```
See ad on Instagram (Discovery)
    ↓
Open merchant website (Interest)
    ↓
Add to cart (Intent)
    ↓
Asked to create account ← DROP-OFF (30%)
    ↓
Enter shipping details
    ↓
See ₹99 shipping charge ← DROP-OFF (20%)
    ↓
Choose COD (trust fallback)
    ↓
Complete purchase
```

### Where Drop-offs Happen
- **Account creation wall:** 30% drop-off
- **Unexpected shipping charges:** 20% drop-off
- **Payment option mismatch:** 10% drop-off

### How UCP Changes This

| Current State | With UCP |
|---------------|----------|
| Create account per site | Linked identity via OAuth |
| Re-enter shipping address | Pre-filled from UCP profile |
| Discover charges at checkout | Transparent pricing in AI surface |

**UCP Impact:** Medium — Priya's COD preference limits full UCP benefit, but account linking helps.

---

## Persona 2: Ramesh — Trust-First Buyer


### Profile
- **Age:** 45
- **Location:** Varanasi, UP
- **Income:** ₹4-5 lakh/year
- **Device:** Entry-level Android, prefers WhatsApp
- **Shopping Behavior:** 1-2 orders/month, only known brands

### Pain Points
- Deeply skeptical of online payments
- Only buys from Amazon/Flipkart (trust)
- Uses COD 90% of time
- Won't share card details online

### Job To Be Done
> "Show me the product is real, price is fair, and I can return it easily. I'll pay when it arrives."

### Current Journey

```
Son recommends product on WhatsApp (Discovery)
    ↓
Opens Amazon app (Trust anchor)
    ↓
Searches for product
    ↓
Compares with Flipkart price
    ↓
Adds to cart on Amazon
    ↓
Selects COD (non-negotiable)
    ↓
Verifies product on delivery
    ↓
Pays cash
```

### Where Drop-offs Happen
- **Unfamiliar merchant site:** 80% bounce
- **Online payment required:** 70% drop-off
- **No COD option:** 90% drop-off

### How UCP Changes This

| Current State | With UCP |
|---------------|----------|
| Only trusts Amazon/Flipkart | *No change — trust is brand, not protocol* |
| Requires COD | *No change — UCP is prepaid-first* |
| Won't enter payment details | *Slight improvement via OAuth, but trust barrier remains* |

**UCP Impact:** Low — Ramesh is not the early adopter. Requires trust-building at platform level first.

---

## Persona 3: Arjun — D2C Repeat Buyer


### Profile
- **Age:** 32
- **Location:** Bangalore, Karnataka
- **Income:** ₹15-20 lakh/year
- **Device:** iPhone, uses multiple apps
- **Shopping Behavior:** 10+ orders/month, D2C brands, subscriptions

### Pain Points
- Annoyed by re-entering payment details across sites
- Tracks orders across 6-7 apps
- Wants seamless repurchase for regular items
- Low patience for checkout friction

### Job To Be Done
> "I've decided what to buy. Just complete the purchase instantly without making me jump through hoops."

### Current Journey

```
Sees product in Instagram Reel (Discovery)
    ↓
Clicks Shop Now
    ↓
Opens D2C brand website
    ↓
Already has account (repeat buyer)
    ↓
Quick checkout with saved UPI
    ↓
Purchase complete in 30 seconds
```

### Where Drop-offs Happen
- **New brand = new account:** 20% friction
- **Payment gateway issues:** 10% failure rate
- **Context switch from discovery app:** 15% drop-off

### How UCP Changes This

| Current State | With UCP |
|---------------|----------|
| Create new account per brand | Single linked identity |
| Payment saved per site | Unified payment across all UCP merchants |
| Leave Instagram to complete | Complete purchase in-app |

**UCP Impact:** High — Arjun is the ideal early adopter. Already prepaid, already frustrated by fragmentation.

---

## Persona 4: Meena — SMB Merchant Owner


### Profile
- **Age:** 38
- **Location:** Indore, MP
- **Business:** D2C ethnic wear brand, ₹50 lakh annual revenue
- **Stack:** Shopify + Razorpay + Instagram Shop
- **Team Size:** 5 (including herself)

### Pain Points
- 65% cart abandonment rate
- High RTO on COD orders (28%)
- Customers ask same questions repeatedly
- Can't afford custom integrations

### Job To Be Done
> "Reduce cart abandonment and returns without building new tech. Let me focus on products, not platform issues."

### Current Journey (Merchant Perspective)

```
Customer discovers on Instagram (Traffic)
    ↓
Clicks to Shopify store (Conversion attempt)
    ↓
65% abandon at checkout ← PROBLEM
    ↓
35% complete order
    ↓
60% COD, 40% prepaid
    ↓
28% RTO on COD orders ← COST
```

### Merchant Pain Points
- **Checkout abandonment:** 65% (industry: 70%)
- **COD RTO cost:** ₹200-400 per failed order
- **Integration burden:** Can't build custom AI experiences

### How UCP Changes This

| Current State | With UCP |
|---------------|----------|
| Each customer creates account | Pre-linked customers via UCP |
| Custom checkout optimization | Standard UCP checkout |
| Can't appear in AI assistants | Discoverable in Gemini, AI surfaces |
| No insight into drop-off reasons | Standardized funnel visibility |

**UCP Impact:** High — Meena gets enterprise-level checkout without enterprise-level investment.

---

## Summary: UCP Fit by Persona

| Persona | UCP Fit | Primary Barrier | Adoption Likelihood |
|---------|---------|-----------------|---------------------|
| Priya (Tier-2 Value) | Medium | COD preference | Later adopter |
| Ramesh (Trust-First) | Low | Deep trust issues, COD-only | Unlikely |
| Arjun (D2C Repeat) | High | None significant | Early adopter |
| Meena (SMB Merchant) | High | Tech awareness | Early adopter (with enabler) |

---

## So What?

**Arjun and Meena are the beachhead.** They have the problem (friction), the means (prepaid, digital stack), and the motivation (convenience, revenue). 

Priya follows once value is proven. Ramesh may never adopt unless trust landscape fundamentally shifts.

---

*Independent Case Study by Vikas Sahani. Based on public sources. No affiliation or endorsement implied.*

[← Back to India Market Fit](https://github.com/VIKAS9793/UCP-integration-Indian-consumer-market/blob/main/docs/03_india_market_fit.md) | [Next: Competitive Comparison →](https://github.com/VIKAS9793/UCP-integration-Indian-consumer-market/blob/main/docs/05_competitive_comparison.md)
