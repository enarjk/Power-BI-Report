# E-commerce Beauty KPI Analytics & Reporting

**Tool:** Microsoft Power BI
**Live Report:** [View in Power BI](https://app.powerbi.com/view?r=eyJrIjoiNzA4MzA3ZGEtOTI0NC00N2Q5LTk5MjUtZTIyNmViMGU4MGViIiwidCI6ImNjZmM2ODA0LTI0MGYtNGJiZS04NTA5LWZjNjRhZTE1NzhmMSIsImMiOjEwfQ%3D%3D)

## Overview

An end-to-end Power BI analytics solution built for a global beauty e-commerce business, covering **Sales, Customer Insights, Product Performance, and Order Details** across five markets (APAC, Europe, USCA, LATAM, Africa). The dashboard combines executive KPI cards, trend analysis, discount-impact modeling, RFM customer segmentation, and drill-down pivot tables to support both strategic and operational decision-making.

## Dashboard Structure

| Page | Purpose |
|---|---|
| **Sales — Overview** | Global KPIs (profit, sales, margin, orders, AOV, unique customers), monthly trends, market/segment/category/city breakdowns, and a world sales map |
| **Sales — Regional (APAC / Europe / USCA / LATAM / Africa)** | Region-specific KPIs and a discount-vs-profit-margin scatter analysis for each market |
| **Customer Insights — Overview** | Customer base health: total/active/inactive customers, churn rate, repurchase and new customer trends, segment mix, geographic distribution |
| **Customer Insights — Inactive** | Inactive customer breakdown by duration, repurchase behavior, and a searchable customer detail table |
| **Customer Insights — RFM** | Recency-Frequency-Monetary segmentation into 11 behavioral segments (Champions, At Risk, Cannot Lose Them, Hibernating, etc.) with segment-level sales and repurchase metrics |
| **Product** | Category and SKU-level performance, quantity-sold trends, unit price elasticity, and discount sensitivity |
| **Order Details** | Drillable pivot tables for monthly/daily sales, segment, market, and order-level granularity |

## Key Findings (FY2023 vs LY)

- **Sales grew 23.8% YoY** to $2.19M, driven by a 27.1% increase in order volume — but **profit fell 12.2%** and **profit margin dropped nearly 5 points (18.0% → 12.77%)**, a 29% relative decline.
- **AOV slipped 2.5%** even as order count rose sharply, indicating growth is coming from more (smaller) orders rather than higher-value ones.
- **Europe is the most profitable market** ($100K profit, 18.45% margin) despite not having the highest sales volume, while **APAC generates the most sales but the thinnest margin** (7.21%), pointing to a discount- or cost-structure issue specific to that region.
- Every regional scatter chart shows a **strong negative correlation between discount rate and profit margin** — margins turn negative once discounts exceed roughly 40–50%, with APAC and LATAM showing the steepest drop-off.
- **Customer churn stands at 56.09%**, with 9,768 inactive members — most (9,768 of which the majority) have been inactive for **over one year**, signaling a retention gap larger than the acquisition gap.
- **RFM segmentation** shows a healthy "Promising" segment (2,043 customers, $808K in sales) but also a sizeable **"Cannot Lose Them"** segment (1,341 customers) and an **"At Risk"** segment with the highest average sales value ($485 average) — high-value customers who are disengaging.
- **Body Care is the top category** by both sales and quantity sold, but the product-level discount-sensitivity chart shows quantity sold is largely flat across discount levels — implying **discounting isn't actually driving incremental volume** in most categories.

## Strategic Recommendations

**1. Rebuild profit margin through discount governance**
- Cap promotional discounts at the threshold where each region's margin turns negative (from the discount-impact scatter charts), rather than applying a flat policy globally.
- Prioritize non-price levers (bundling, loyalty perks, free shipping thresholds) over blanket discounts, since the data shows discounting has limited effect on quantity sold.

**2. Fix the AOV decline**
- Introduce cross-category bundles anchored on Body Care (the top seller) paired with lower-penetration categories like Face Care and Hair Care to lift basket size.
- Set tiered free-shipping or gift thresholds just above the current $125 AOV to nudge order values up.

**3. Target APAC's margin problem specifically**
- Since APAC has the highest sales but the weakest margin, audit discount depth, shipping/fulfillment cost, and pricing by category in that market before scaling further marketing spend there.

**4. Reduce churn with segment-specific retention campaigns**
- **"Cannot Lose Them" and "At Risk"** segments (high historical value, going cold) should get win-back offers, personalized outreach, or replenishment reminders rather than generic promotions.
- **"Promising" and "Recent Customers"** should be moved into structured onboarding/loyalty flows to convert first purchases into repeat behavior before they lapse.

**5. Double down on what's working in Europe**
- Europe's higher margin at lower discount depth suggests a pricing/positioning model worth testing in USCA and LATAM, which have similar order volumes but weaker margins.

**6. Rebalance category strategy**
- Since discount depth doesn't meaningfully move volume, shift merchandising focus toward higher-margin categories (Hair Care, Face Care) and use Body Care primarily as a traffic driver rather than a discount-led volume driver.

## Tech Stack

- **Microsoft Power BI** — data modeling, DAX measures, and interactive report design
- Multi-market data model with drill-through and cross-page slicers (Year, Market, Segment, Inactive Range)
- RFM segmentation logic built via calculated columns/measures for Recency, Frequency, and Monetary scoring

---
*Dashboard and analysis created as part of an e-commerce beauty analytics portfolio project.*
