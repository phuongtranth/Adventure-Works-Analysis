# [Power BI] Superstore Sales and Expansion Strategy Analysis
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
| Business Overview        | Overview of revenue (total, segment, location, purchase reason) and customer segments (Avg R, F, M). | To provide a high-level view of overall business performance and customer behavior, aiding strategic decision-making.    |
| Monthly Segment Analysis | Revenue analysis by day, region, reason, and subcategory by month for each customer segment.       | To monitor detailed performance trends and understand the impact of different factors on each segment's revenue growth. |
### Step 3 - Ideate

### Step 4 - Prototype
### Step 5 - Review

## III. Dashboard
## IV. Insights
## V. Recommendations
