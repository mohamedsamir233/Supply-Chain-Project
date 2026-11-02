# Supply Chain Project

# Northwind Marketing & Supply Chain Analysis

> What do 830 orders and $1.27M in net revenue tell us about our next marketing priorities?

An end-to-end analysis of the Northwind sales dataset (July 1996 - May 1998), built in **Power BI** and presented as a 17-slide Arabic/English deck. It covers growth, customers, products, markets, discounts, sales team performance, and delivery, and ends with six actionable marketing priorities.

## Project Overview

| Item | Detail |
|---|---|
| Source file | `Supply_chain_Report.pbix` |
| Dataset | Northwind sample model, 7 tables |
| Scale | 830 orders, 2,155 order lines, 77 products, 91 customers (89 active), 9 sales reps |
| Period | 4 Jul 1996 - 6 May 1998 |
| Net revenue | $1,265,793 (after discounts) |
| Tools | Power BI, DAX, RFM segmentation |

## Key Findings

**Growth**
- Revenue grew in every full quarter and peaked at **$298K in Q1 1998**.
- Jan-Apr 1998 revenue is up **+121%** vs the same period in 1997, and order count is up +108%.

**Customers**
- Customer acquisition has stalled: only **22 of 89** customers joined after 1996, and just 2 since Q4 1997.
- **92%** of 1997 customers ordered again in 1998, so growth comes from loyal customers spending more.
- Top 3 customers generate **25.2%** of revenue; top 10 generate 45%.

**Products & Pricing**
- Top 10 products drive **44%** of revenue; 8 discontinued products account for $185K (14.6%).
- Seafood is the fastest-growing category (+285%), Grains the slowest (+32%).
- Only two products priced above $100 generate 17.5% of revenue, and one of them (Thüringer Rostbratwurst) is now discontinued.

**Markets**
- USA, Germany, and Austria generate **48%** of revenue.
- Biggest gains: USA, Germany, Brazil. Declining (small) markets: Denmark, Canada, Mexico.

**Customer Segments (RFM)**
- 21 "Champions" generate **62%** of revenue.
- 16 customers have not ordered in 90+ days, including 4 high-value accounts worth $89K.

**Cross-selling**
- Customers buying all 8 categories spend an average of **$26.6K**, vs $10.4K for those buying 7 (correlation, not proof of causation).

**Discounts**
- Discounts cost **$88.7K**. 91% of that cost sits in the 10-25% tiers, which sell about the same units per line as the 5% tier.

**Delivery**
- **95%** of shipped orders arrive on time; average 8.5 days from order to shipment.

## Recommendations

1. **Reopen customer acquisition**, targeting high-value markets (Germany, USA, Sweden) and activating the 2 accounts that never ordered.
2. **Protect the top 3 accounts** with named owners and account plans.
3. **Win back silent customers**, starting with the 4 high-value accounts worth $89K.
4. **Cross-sell across categories** with bundles aimed at the 32 customers buying 6 or fewer categories.
5. **Cap discounts** between 5% and 10%.
6. **Replace discontinued products** and back the fast-growing seafood category.

## Methodology Notes

- **Net revenue** = Unit Price x Quantity x (1 - Discount). The report's `Total Amount` column ignores discounts ($1,354,459).
- Because data ends on 6 May 1998, year-over-year comparisons use **Jan-Apr** of each year. Q2 1998 is partial and is not a decline.
- Country = customer country. Sales reps are attributed per order.
- RFM segments are based on Recency, Frequency, and Revenue, calculated up to 6 May 1998.

## Limitations

The dataset has no costs, margins, marketing spend, campaigns, or channels. This analysis therefore does **not** measure ROI, profit, or campaign attribution, and the discount analysis covers volume effects only.

## Repository Structure

```
├── Supply_chain_Report.pbix      # Power BI report
├── Marketing_Analysis.pdf        # Presentation deck (17 slides)
└── README.md
```

## How to Use

1. Clone the repo.
2. Open `Supply_chain_Report.pbix` in Power BI Desktop.
3. Browse the pages or read the deck for the full story.

## Author

**[Mohamed Samir]** - [LinkedIn](https://www.linkedin.com/in/mohamedsamir233/) | [Email](mailto:mohamedsamir272001@gmail.com)