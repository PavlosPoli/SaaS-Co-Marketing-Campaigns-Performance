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
- **New Customer Initial MRR**: The economic value of the acquisition count. Nine small customers and nine high-value customers should not be treated as equal.

#### Marketing Spend
**Latest month:** The business spent €70,667 in December. That was €35,336 less than November, a 33.3% drop. Even after that monthly fall, December spending was €2,715, or 4.0%, higher than in December 2024.

**Where the budget went:** Paid Search received the largest share of marketing money across the full period: 39.1% of the total. Outbound was next at 19.3%, followed by Events at 15.2%. Together, these three categories accounted for almost three quarters of the marketing cost.

**What changed in the latest month:** Most of the month-over-month spending drop came from Events and Organic. Events fell from €29,627 in November to €6,411 in December. Organic fell from €16,045 to €7,762.

#### Signups
**Latest month:** December generated 2,019 signups. This was 1,012 fewer than November, a 33.4% decline and 619 fewer than December 2024, a 23.5% decline.

**Where signups came from:** Paid Search generated 1,414 of the 2,019 December signups, or 70.0%. This means seven out of every ten signups came from one category, so signup volume was heavily dependent on Paid Search.

**Cost and signup progress:** Paid Search recorded the lowest December cost per signup at €18.27. Partner moved the largest part of its leads into signups, with a 49.7% lead-to-signup rate. Organic had the lowest rate at 23.3%.

#### New Customers
**Latest month:** The business gained 9 new customers in December, the same number as in November. December 2024 had 18, so the latest month was 50.0% lower year over year.

**Latest month mix:** There were 10 Won outcomes in December: 9 first-time customers and 1 returning customer. Outbound brought in 4 of the 9 new customers, the largest contribution from any campaign category that month.

**Full-period comparison:** Partner accounted for 22.0% of all new customers while using 10.8% of marketing cost. Referral accounted for 18.0% of new customers while using only 1.8% of cost. Both categories produced a larger share of customers than their share of spending.

#### New Customer Initial MRR
**Latest month:** New customers added €17,261 of initial MRR in December. That was €9,405, or 119.7%, more than November. It was still €11,345, or 39.7%, below December 2024.

**Value per new customer:** The average new customer added €1,918 of initial MRR in December. This was more than double November's €873 and above the €1,589 average in December 2024.

**Budget share versus customer value:** Paid Search used 39.1% of marketing cost but produced 15.0% of acquired initial MRR across the full period. Partner and Referral each produced about 18.4% of acquired initial MRR while using much smaller part of the budget.

## Recommendations
- **Reduce Paid Search gradually**: Keep Paid Search as the main source of signup volume but move some of its budget to categories that produced a stronger share of new customers and recurring value.

- **Scale back Events:** Keep Events active for testing but focus spending on the formats that consistently contribute to customer acquisition.

- **Increase Partner investment:** Give Partner more budget slowly because it produced a strong share of new customers and recurring value from a relatively small share of spend.

- **Give Organic a larger budget:** Expand the Organic campaigns and content that repeatedly turn leads into signups and new customers.

- **Test Referral growth and keep Outbound stable:** Grow Referral carefully because its strong efficiency may be harder to maintain at scale. Keep Outbound as a steady acquisition channel.

## Dashboard
The dashboard can be found in Tableau Public [here] <provide link>

## Presentation
The presentation created for the marketing team walks through the insights and recommendations above and can be found [here] <provide link>


