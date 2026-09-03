# SaaS Co Marketing Insights - Project Overview
Campaign performance and future budget allocation

## The project's goal is to investigate the performance of SaaS Co's marketing campaign categories and surface evidence-based recommendations for allocating future marketing budget.

SaaS Co is a subscription-based analytics and reporting software company serving business customers across the United States and other international markets. From 2021 onward, the company ran 19 marketing campaigns across six categories: Paid Search, Organic, Outbound, Events, Partner and Referral. Prospects move from campaign engagement to leads and trial signups before entering the sales opportunity pipeline, where successful outcomes become new customer acquisitions or reactivations.

Preparing the next annual marketing budget, SaaS Co wants a clearer view of how each campaign category performed and how campaign activity relates to signups, Won customer outcomes (New/Reactivated) and the initial recurring revenue attached to those customers. The budget supports two primary objectives: 1) increase qualified trial signups and new customer acquisitions, and 2) expand awareness of SaaS Co's analytics platform across its target markets. This project describes the performance observed in the available data and uses those results to propose a measured allocation of future campaign spending.

## Dataset structure
Only two raw tables are required. Their relationship is logical rather than a physical join, because joining campaign-month spend to touch-level rows would repeat spending.

<img width="953" height="410" alt="image" src="https://github.com/user-attachments/assets/064e9f29-ddfe-4a8d-9afa-610dc5760f55" />

**raw_fact_marketing_campaign_spend:** Grain: one row per campaign_id and campaign_month. Source rows: 729. Period: January 2021-December 2025.

**raw_fact_marketing_touches:** Grain: one row per touch_id. Source rows: 19,528. Touch period: March 2021-March 2026; conversion outcomes run through December 2025.

## Insights Summary
#### In order to evaluate campaign performance, I focused on the following key metrics. Together they show budget deployed, signup response, first-time customer outcomes and the initial recurring value attached to those outcomes.
- **Marketing Spend**: Shows how much budget was used. Budget allocation cannot be evaluated without the size of the investment.
- **Signups**: Measures the campaign response volume that entered the product trial stage.
- **New Customers**: Counts first-time customers won. Reactivations are excluded so acquisition performance is not overstated.
- **New Customer Initial MRR**: Adds economic value to the acquisition count. Nine small customers and nine high-value customers should not be treated as equal.
