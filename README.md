# [Power BI] Customer Segmentation for A Manufacture Business
## I. Introduction

### Key Focus Areas
### Dataset
## II. Design Thinking Steps
### Step 1 - Empathize

| 5W1H                                                          |                                           |
| ------------------------------------------------------------------ |--------------------------------------------- |
| Who will be viewing this Dashboard?                                | Marketing team, Sales team, CRM team<br> |
| If we had to choose only one key Stakeholder, who would it be?<br> | Marketing team |
| What problem does this Dashboard solve?                            | It addresses the need to understand diverse customer behaviors and preferences to adjust personalized marketing and sales strategies, thereby helping to increase sales/customer engagement.<br> |
| Describe the problem in one sentence                               | Customer segmentation and developing appropriate strategies for each segment.<br> |
| When and where will Stakeholders view this Dashboard?<br>          | The Dashboard can be viewed during monthly marketing strategy meetings or when presenting to stakeholders.<br> |
| Why do stakeholders need this Dashboard?<br><br>                   | Understand customer segments<br>Evaluate performance and make strategic decisions<br>Develop personalized strategies<br>Predict trends |
| How have stakeholders been achieving their goals so far?           | Relying on fragmented data sources, manual reporting processes, and periodic customer surveys to understand customer segments and make marketing decisions |


|Stakeholder Empathy Mapping                                                         |                                                          |
| ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pains                                                      | Fragmented data sources, manual reporting processes, lack of clear customer insights for strategic decision-making.                                                      |
| Thinking and feeling                                       | Need to better understand customer behavior and preferences to optimize marketing and sales strategies. Feel limited by current data and reporting capabilities.         |
| Seeing                                                    | Diverse customer segments with varying behaviors, challenges in tailoring marketing strategies to different segments effectively.                                        |
| Saying and doing                                          | "We need more data-driven insights." "Our strategies need to be more targeted." Actively seeking better tools and processes for data analysis and customer segmentation. |
| Gains                                                     | Improved customer understanding, better-targeted marketing campaigns, increased sales and engagement, streamlined decision-making processes.                             |


| Fact table<br>                        | Dim table<br>                                                 |
| -------------------------------------- | -------------------------------------------------------------- |
| Sale Order Detail,<br>SalesOrderHeader | Customer, Location, Dim_Date, DimProduct, Segment, SalesReason |

### Step 2 - Define POV

|                            | NORTHSTAR METRIC                         |
|----------------------------|--------------------------------------|
| **What VALUE you want to measure?** | Revenue                              |
| **WHEN the value DELIVERY SUCCESS?** | When the revenue meets or exceeds the predefined target, indicating successful sales and profitability. |
| **Northstar Metric Name**  | Revenue                              |
| **WHY do you choose this metric?** | Revenue is a key indicator of business growth and success, as it measures the total sales generated and reflects the company's financial health. |


Dimension Group
| Group 1 | Group 2  | Group 3 | Group 4       |
| ------- | -------- | ------- | ------------- |
| segment | location | product | buying reason |

Define Point of View
| View                     | Description                                                                                       | Why                                                                                                                     |
|--------------------------|---------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| Customer Segmentation Overview         | Overview of revenue (total, segment, location, purchase reason) and customer segments (Avg R, F, M). | To provide a high-level view of overall business performance and customer behavior, aiding strategic decision-making.    |
| Monthly Segment Analysis | Revenue analysis by day, region, reason, and subcategory by month for each customer segment.       | To monitor detailed performance trends and understand the impact of different factors on each segment's revenue growth. |
### Step 3 - Ideate
Brainstorming
| Idea Name               | Layer 0 Dimension: Total Metrics              | Layer 1 Dimension: Breakdown by 1 Dimension                                   | Layer 2 Dimension: Breakdown by 2 Dimensions                                           |
|-------------------------|-----------------------------------------------|--------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| Customer Segmentation Overview        | Total revenue<br>Total customers<br>Total orders | % revenue by continent, country<br>% revenue by segment<br>% customers by segment<br>% orders by purchase reason<br>Avg RFM by segment | % revenue by segment and country<br>% revenue by segment and purchase reason           |
| Monthly Segment Analysis| Slicer: month, year, segment                   | % revenue by country<br>Top 5 revenue by subcategory<br>% orders by reason<br>Table of revenue by day/revenue LM/MTD | % revenue by subcategory and segment<br>% orders by reason and segment                 |


#### Next, I proceeded with **Step 4 - Prototype and Review** multiple times and achieved the final result, which will be presented in the following section as a dashboard.

## III. Dashboard
### Data modeling
![image](https://github.com/user-attachments/assets/2cf4d42a-fbb5-4253-8d36-89912af3b5e2)

### View 1: Customer Segmentation Overview  
![image](https://github.com/user-attachments/assets/e286a2f5-8cbc-4bb5-8d1e-2c141b3fb1d4)

### View 2: Monthly Segment Analysis
![image](https://github.com/user-attachments/assets/49b999af-f0ee-4139-99f9-09bc76f4d99d)

## IV. Insights
### Geographic Distribution:
- North America dominates revenue generation, accounting for over 72% of total revenue.
- Key regions within North America include the Southwest, Northwest, and Canada, each contributing significantly.
### Order Drivers:
- Price and promotions are the primary factors driving orders.
- Advertising channels appear underutilized, suggesting potential for growth in this area. This indicates recent marketing activities have been effective in attracting new customers, though they haven't yet translated into significant revenue.
### Segment Performance:
- Champions (10% of customers) and Loyal customers (9% of customers) generate 75% of total revenue.This concentration highlights the critical importance of these segments to the business.
- 20% of customers fall into the "At Risk" and "Cannot Lose Them" segments. These groups require targeted retention strategies to prevent churn and maintain engagement.
- The "Cannot Lose Them" segment (11% of customers, 15% of revenue) shows high value but potential disengagement, given their high recency score.
- The Promising segment (12% of customers, 3% of revenue) represents a significant opportunity for revenue growth.
## V. Recommendations
| Segment | Strategy | Suggestions |
|---------|----------|-------------|
| Champions | Retention | - Implement a VIP program with exclusive benefits and early access to new products/services<br>- Personalized communication and dedicated account managers<br>- Seek feedback and involve them in product development |
| Loyal | Retention & Development | - Create a tiered loyalty program to encourage increased spending<br>- Cross-sell and upsell complementary products<br>- Offer referral bonuses to leverage their positive sentiment |
| Cannot Lose Them | Retention | - Conduct surveys to understand their current needs and pain points<br>- Offer tailored incentives to re-engage them<br>- Provide premium customer service to address any issues promptly |
| At Risk | Retention | - Implement a win-back campaign with personalized offers<br>- Reach out proactively to address potential issues<br>- Offer a loyalty program to incentivize continued engagement |
| Promising | Development | - Create targeted upselling campaigns to increase order value<br>- Provide educational content about product benefits to encourage more frequent purchases<br>- Offer bundle deals to increase average order value |
| New Customers | Development | - Implement an onboarding program to familiarize them with all product offerings<br>- Offer a "new customer" discount on their next purchase<br>- Provide excellent customer support to ensure a positive first experience |
| Hibernating/About to Sleep | Re-activation | - Launch a re-engagement email campaign with special offers<br>- Showcase new products or improvements since their last purchase<br>- Offer a time-limited incentive to encourage immediate action |
| Potential Loyalist | Development | - Implement a fast-track program to quickly reward increased engagement<br>- Personalize product recommendations based on past purchases<br>- Offer exclusive "members-only" deals to encourage loyalty |
| Need Attention | Development | - Conduct a survey to understand their specific needs and preferences<br>- Offer a tailored product bundle based on their past purchases<br>- Provide additional support or training if product complexity is an issue |
| Lost Customers | Re-attraction | - Analyze reasons for loss and address them in win-back campaigns<br>- Offer a "welcome back" package with competitive incentives<br>- Showcase new features or improvements that address potential past issues |
