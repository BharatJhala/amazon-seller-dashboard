# 📊 Amazon Seller Dashboard
### A Product Analytics Prototype by Bharat Jhala

> **Live Demo →** [bharatjhala.github.io/amazon-seller-dashboard](https://bharatjhala.github.io/amazon-seller-dashboard)
> **Medium Article →** Your Dashboard Is Lying to You
---

## Overview

A dashboard prototype designed for **small Amazon third-party sellers** — helping them move from reactive firefighting to proactive decision-making using data they already have.

Most sellers find out something broke only after sales fall. By then a lost buy box or a slipped search rank has been bleeding them for days. This dashboard surfaces the right signal at the right time — so the seller sees the cause before it becomes a crisis.

---

## The Problem

Small Amazon sellers face four critical pain points:

| Pain Point | Impact |
|---|---|
| Can't explain their own sales dip | Too many causes lumped together — no diagnosis |
| Can't see buy box or search visibility status | Invisible bleeding until it's too late |
| Competitor prices move faster than they can track | Lose buy box without knowing why |
| Inventory planning is guesswork | Stockouts wreck rankings for weeks |

---

## North Star Metric

**Buy Box Win Rate** — the single metric that best captures seller health.

> *"If you're not winning the buy box, you're doing all the work of getting found and handing the sale to someone else."*

**Why Buy Box Win Rate over Search Rank or Total Sales?**

- High search rank + lost buy box = competitor profits from YOUR visibility
- Total sales is a lagging indicator — it confirms what already happened
- Buy Box Win Rate is the earliest warning signal in the revenue chain

---

## Metric Framework

The dashboard is built on a three-layer causal model:

```
OUTCOME  →  Did we win?
            Buy Box Win Rate (NSM)
            Sales & Revenue

OUTPUT   →  What directly determines whether we win?
            Competitive Price Gap
            Inventory Availability
            Seller Rating / Fulfillment Method

INPUT    →  What predicts whether outputs will hold?
            Search Rank & Visibility
            View-to-Order Conversion
            Units Sold & Sell-Through Rate
            Returns Rate
            Competitor Price Movement
```

When the NSM drops, the dashboard immediately answers *why* — by surfacing the output and input metrics that caused it.

---

## Threshold Logic

Each metric uses evidence-based thresholds to drive the green/amber/red status:

| Metric | 🟢 Green | 🟡 Amber | 🔴 Red |
|---|---|---|---|
| Buy Box Win Rate | > 80% | 60–80% | < 60% |
| Inventory Availability | > 6 weeks | 3–6 weeks | < 3 weeks |
| Competitive Price Gap | Within $1 | $1–$3 | > $3 |
| View-to-Order Conversion | > 10% | 6–10% | < 6% |
| Returns Rate | < 2% | 2–4% | > 4% |

**Rationale:**
- **Buy Box 80%** — sellers below this threshold see measurable revenue decline per Amazon's seller data
- **Inventory 3 weeks** — average FBA reorder lead time is 2–3 weeks; below that, stockout risk is real
- **Price gap $3** — Amazon's algorithm begins heavily favouring competitors beyond a $2–3 price gap
- **Conversion 10%** — average Amazon conversion rate; below 6% signals a listing quality problem

---

## Dashboard Structure

The dashboard is organized around one question: **what does the seller need to know right now?**

```
SECTION 1 — "How am I doing right now?"
  → 4 metric cards: NSM + key outcomes
  → Each shows: current week value, delta vs last week,
    8-week sparkline trend, green/amber/red status

SECTION 2 — "Why am I doing that?"
  → Buy box win rate 8-week trend chart
  → Your price vs. buy box winner comparison chart
  → 3 mini diagnostic charts: search rank,
    conversion rate, returns rate

SECTION 3 — "What should I do about it?"
  → 3 actionable alerts with severity levels
  → Each alert: what happened + what it means + next step
```

---

## Actionable Alerts

The dashboard doesn't just report — it recommends:

**🔴 Pricing Alert (Urgent)**
> Your price on Product X is $4.20 higher than the current buy box winner. You lost 38 points of buy box share this week — costing an estimated $5,800 in revenue. Drop to $23.99 to reclaim the buy box immediately.

**🔴 Inventory Alert (Urgent)**
> Product X has 100 units left. At your current sell rate of 50 units/week, you have 2 weeks of stock remaining. A stockout will cause Amazon to demote your listing and suppress your search rank for weeks. Reorder at least 100 units now.

**🟡 Conversion Alert (Watch Closely)**
> Your conversion rate dropped from 12.4% to 6.1% this week — half your usual buyers are landing on your listing and leaving without purchasing. A recent 2-star review is likely hurting trust. Update your main product image, review pricing vs. similar listings, and respond to the negative review today.

---

## Design Decisions

**Why weekly view?**
Daily metrics are too noisy — Monday always looks different from Saturday. Weekly view smooths out weekday patterns, holidays, and seasonal variance. It's the standard benchmark in e-commerce analytics.

**Why 8-week sparklines?**
A single number tells you where you are. An 8-week trend tells you which direction you're moving and how fast. The difference between a sudden cliff and a slow erosion requires the longer view — and each demands a different response.

**Why AWS color theme?**
The seller operates within the AWS/Amazon ecosystem. A dashboard that feels native to that environment reduces cognitive load and signals that the product understands the seller's world.

---

## Tech Stack

```
HTML / CSS / JavaScript   →  Single file, no framework needed
Chart.js 4.4.1            →  Line charts, bar charts, sparklines
GitHub Pages              →  Free hosting, live URL
```

---

## Files

```
amazon-seller-dashboard/
├── index.html    →  Complete dashboard (single file)
└── README.md     →  This file
```

---

## About

**Bharat Jhala** — Sr. Business Analyst & Certified Scrum Product Owner with 14 years of experience across government, health, banking and insurance sectors.

[![GitHub](https://img.shields.io/badge/GitHub-BharatJhala-FF9900?style=flat&logo=github)](https://github.com/BharatJhala)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Bharat_Jhala-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/bharatjhala)

---

*Product Analytics Prototype · 2026*
