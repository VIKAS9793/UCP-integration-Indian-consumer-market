# Metrics & Experiments

**How We Measure UCP Success in India**

---

## North Star Metric

### **Checkout Completion Rate via UCP**

> Percentage of users who start a UCP-enabled checkout and complete purchase.

**Formula:**
```
UCP Checkout Completion Rate = (Completed UCP Purchases / UCP Checkout Initiations) × 100
```

**Why This Metric:**
- Directly measures UCP's core value proposition (reduced checkout friction)
- Comparable to existing merchant checkout rates
- Actionable at merchant and protocol level

**Target:**
| Segment | Current (Non-UCP) | Target (With UCP) | Improvement |
|---------|-------------------|-------------------|-------------|
| D2C Beauty | 30-35% | 45-50% | +15 pp |
| Travel | 40-45% | 55-60% | +15 pp |
| Overall Retail | 25-30% | 35-40% | +10 pp |

*Note: Baseline estimates from industry averages. Targets are assumptions requiring validation.*

---

## KPI Tree

![Metrics Success Dashboard](https://raw.githubusercontent.com/VIKAS9793/UCP-integration-Indian-consumer-market/main/assets/metrics_dashboard.png)

```
North Star: UCP Checkout Completion Rate
    │
    ├── Conversion Metrics
    │   ├── Cart-to-Checkout Rate (UCP surfaces)
    │   ├── Payment Success Rate
    │   └── First-Time User Completion Rate
    │
    ├── Adoption Metrics
    │   ├── Merchant Adoption (# of UCP-enabled stores)
    │   ├── Consumer Adoption (# of linked UCP accounts)
    │   └── AI Surface Coverage (# of platforms integrated)
    │
    ├── Engagement Metrics
    │   ├── Repeat Purchase Rate (UCP users)
    │   ├── Cross-Merchant Purchase Rate
    │   └── UCP vs Non-UCP Session Duration
    │
    └── Business Metrics
        ├── Merchant GMV via UCP (₹ crore)
        ├── Prepaid Order Share (UCP vs baseline)
        └── Cart Abandonment Rate Reduction
```

---

## KPI Definitions

### Conversion Metrics

| KPI | Definition | Target |
|-----|------------|--------|
| Cart-to-Checkout Rate | % of add-to-cart events that initiate checkout | +10% vs baseline |
| Payment Success Rate | % of payment attempts that succeed | >95% |
| First-Time User Completion | % of new UCP users who complete first purchase | >40% |

### Adoption Metrics

| KPI | Definition | Phase 1 Target |
|-----|------------|----------------|
| Merchant Adoption | # of live UCP-enabled stores | 50 merchants |
| Consumer Adoption | # of users with linked UCP accounts | 1 lakh users |
| AI Surface Coverage | # of AI platforms with UCP integration | 2 platforms |

### Engagement Metrics

| KPI | Definition | Target |
|-----|------------|--------|
| Repeat Purchase Rate | % of UCP users who make 2+ purchases within 90 days | >25% |
| Cross-Merchant Purchase | % of users buying from 2+ UCP merchants | >15% |

### Business Metrics

| KPI | Definition | Phase 1 Target |
|-----|------------|----------------|
| Merchant GMV via UCP | Total transaction value through UCP | ₹50 crore |
| Prepaid Order Share | % of UCP orders that are prepaid | >90% |
| Abandonment Rate Reduction | % point improvement in abandonment | -15 pp |

---

## Experiment Plan

### Experiment 1: UCP vs Standard Checkout (A/B Test)

**Hypothesis:** UCP checkout increases completion rate by 15+ percentage points compared to standard merchant checkout.

| Dimension | Detail |
|-----------|--------|
| Test Design | A/B split on product pages |
| Control | Standard Shopify checkout |
| Variant | UCP-enabled checkout |
| Traffic Split | 50/50 |
| Sample Size | 10,000 sessions per arm |
| Duration | 4 weeks |

**Success Metrics:**
| Metric | Success Threshold | Kill Threshold |
|--------|-------------------|----------------|
| Checkout Completion Rate | +15 pp | <5 pp improvement |
| Payment Success Rate | >95% | <90% |
| Customer Complaints | <1% of orders | >3% of orders |

**Kill Criteria:** If completion rate improvement <5 pp OR payment success <90% OR complaints >3%, halt experiment and diagnose.

---

### Experiment 2: AI Surface Discovery (Gemini Integration)

**Hypothesis:** Users who discover products via Gemini and checkout with UCP have higher completion rates than users who click through to merchant site.

| Dimension | Detail |
|-----------|--------|
| Test Design | Cohort comparison |
| Cohort A | Gemini discovery → UCP checkout in-app |
| Cohort B | Gemini discovery → Merchant site checkout |
| Sample Size | 5,000 users per cohort |
| Duration | 6 weeks |

**Success Metrics:**
| Metric | Success Threshold | Kill Threshold |
|--------|-------------------|----------------|
| Checkout Completion Rate | +20 pp (Cohort A vs B) | <10 pp difference |
| Time to Purchase | <2 minutes | >5 minutes |
| User Satisfaction (CSAT) | >4.0/5.0 | <3.5/5.0 |

**Kill Criteria:** If no significant completion improvement OR CSAT falls below 3.5.

---

### Experiment 3: Repeat Purchase Velocity

**Hypothesis:** UCP users make repeat purchases faster than non-UCP users (within 30 days vs 60 days).

| Dimension | Detail |
|-----------|--------|
| Test Design | Cohort comparison |
| Metric | Days to second purchase |
| Cohort A | UCP-linked users |
| Cohort B | Non-UCP users (same merchant) |
| Sample Size | 2,000 users per cohort |
| Duration | 90 days |

**Success Metrics:**
| Metric | Success Threshold | Kill Threshold |
|--------|-------------------|----------------|
| Median Days to Repeat | <30 days (UCP) vs <60 days (control) | No significant difference |
| Repeat Purchase Rate | >30% (UCP) | <20% |

---

### Experiment 4: Prepaid Conversion Lift

**Hypothesis:** UCP increases prepaid order share by reducing checkout friction for prepaid options.

| Dimension | Detail |
|-----------|--------|
| Test Design | Before/after merchant comparison |
| Metric | Prepaid order % |
| Sample | 10 D2C merchants |
| Duration | 8 weeks (4 pre, 4 post) |

**Success Metrics:**
| Metric | Success Threshold | Kill Threshold |
|--------|-------------------|----------------|
| Prepaid Share | +10 pp (e.g., 40% → 50%) | <5 pp improvement |
| COD RTO Rate | No increase | RTO increases by >5 pp |

---

### Experiment 5: Trust Signal Impact

**Hypothesis:** Adding UPI logo + merchant verification badge increases UCP checkout initiation by 15%.

| Dimension | Detail |
|-----------|--------|
| Test Design | A/B on checkout modal |
| Control | UCP checkout (no badges) |
| Variant | UCP checkout + UPI + verified merchant badges |
| Traffic Split | 50/50 |
| Sample Size | 5,000 sessions per arm |
| Duration | 3 weeks |

**Success Metrics:**
| Metric | Success Threshold | Kill Threshold |
|--------|-------------------|----------------|
| Checkout Initiation Rate | +15% | <5% improvement |
| User Reported Trust (survey) | >75% "trusted" | <60% "trusted" |

---

## Experiment Prioritization

| Priority | Experiment | Confidence | Impact |
|----------|------------|------------|--------|
| P0 | Exp 1: UCP vs Standard Checkout | High | High |
| P0 | Exp 5: Trust Signal Impact | Medium | High |
| P1 | Exp 2: AI Surface Discovery | Medium | Medium |
| P2 | Exp 3: Repeat Purchase Velocity | Low | Medium |
| P2 | Exp 4: Prepaid Conversion Lift | Medium | Medium |

---

## Measurement Infrastructure Requirements

| Need | Solution |
|------|----------|
| Event tracking | UCP checkout events → merchant analytics |
| A/B test framework | Merchant-side (Shopify app) or Google-side |
| Cohort analysis | User ID linking across sessions |
| Survey integration | Post-purchase CSAT collection |

---

## So What?

**Measurement must prove:**
1. UCP actually reduces friction (completion rate up)
2. Users trust UCP checkout (low complaints, high CSAT)
3. Merchants see ROI (GMV, prepaid share up)

**If these fail:** UCP has protocol-market fit issues in India and needs iteration before scale.

---

*Independent Case Study by Vikas Sahani. Based on public sources. No affiliation or endorsement implied.*

[← Back to Adoption & GTM](https://github.com/VIKAS9793/UCP-integration-Indian-consumer-market/blob/main/docs/06_adoption_and_gtm.md) | [Next: Risks & Governance →](https://github.com/VIKAS9793/UCP-integration-Indian-consumer-market/blob/main/docs/08_risks_trust_governance.md)
