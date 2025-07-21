# AdventureWorks Analysis (2020-2022)
---

## Table of Contents
- [Project Summary](#project-summary)
- [Part 1: Sales Overview ](#part-1-Sales-Overview)
- [Part 2: Regional Performance](#part-2-Regional-Performance)
- [Part 3: Product Insights](#part-3-Product-Insights)
- [Part 4: Customer Insights](#part-4-Customer-Insights)
- [Part 5: Recommendations & Next Steps](#part-5-recommendations--next-steps)
- [Addendum: Notes on Data Modeling](#addendum-notes-on-data-modeling)

---
## Project Summary
**AdventureWorks** is a fictional global manufacturing company that produces cycling equipments, clothing, and accessories. In this project, I stepped into the role of a Business Intelligence Analyst tasked with helping management track KPIs, monitor product and customer trends, and evaluate regional performance.

This Power BI dashboard was built to:
- Track KPIs like revenue, profit, order volume, and return rate
- Explore product-level performance and profitability
- Evaluate regional sales differences
- Analyze customer retention and value trends

**Tools used:**  Power BI Desktop | DAX | Power Query  
**Dataset:** [Maven Analytics Power BI Desktop course](https://mavenanalytics.io/course/microsoft-power-bi-desktop) | Derived from the [AdventureWorks sample databases](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver17&tabs=ssms) from Microsoft

### Data Model
To support analysis and accurate relationships between tables, I built a **star schema data model** in Power BI. This model connects core fact tables (e.g., sales, returns) with supporting dimension tables (e.g. product, customers, territories), enabling efficient filtering and aggregation across various dimensions (dimension tables on the top while fact tables on the bottom for a cleaner apperance).

Here’s a view of the data model used for this project:
<img width="961" height="628" alt="image" src="https://github.com/user-attachments/assets/c691d2c8-606b-48a8-99d0-dc60b754ec86" />

For a closer look at the dataset used in this project, you can explore the original files [here](data)

## Part 1: Sales Overview
[Back to Table of Contents](#table-of-contents)
### Summary of Insights:
Revenue peaked in 2021 ($9.3M) and stabilized in 2022 ($9.2M). Profit mirrored revenue: $4.0M in 2021 to $3.9M in 2022. Orders steadily increased from 2.6K (2020) to 11.8K (2022) and Return rate improved 3.3% in 2020 to 2.1% in 2022.

### Seasonality:
Late 2021 saw the most substantial monthly growth reaching $1.6M in revenue likely strong seasonal demand or promotional activity. Revenue remained relatively flat throughout 2020, fluctuating between $585K and $326K. However, beginning in Q2 2021, growth became more pronounced, with monthly sales steadily increasing through 2022

### Category & Product Highlights:
Accessories had the highest order volume (17K orders) reflecting the high-frequency, low-cost nature of these products. Bikes drove the most revenue: $23.6M over 3 years, Clothing experienced a noticeable increase in orders over time, particularly in 2022, signaling growing interest in apparel. Water Bottle – 30 oz. was the most ordered product (4K orders) while Sport-100 Helmets had highest revenue but also highest return rates (>3.3%). At the subcategory level, Tires and Tubes contributed over a third of total orders (36.1% or 9.1K) while Shorts registered the highest return rate among all subcategories, making up 2.2% of total returns (40 returns).

<img width="1461" height="812" alt="image" src="https://github.com/user-attachments/assets/420bcbcf-5478-4cba-adfe-1c0a23712ab5" />

To explore the report further [Click here to view the interactive Sales Overview](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)

## Part 2: Regional Performance
[Back to Table of Contents](#table-of-contents)

### Summary of Insights: 

### North America
- Orders: 11.7K (United States: 8.7K | Canada: 3K)
- Revenue: $9.7M
- Profit: $4.1M
- Return Rate: 2.1%

### Category Highlights:
- Bikes: Highest revenue driver ($683.8K), strong profit ($281.6K) with a modest return rate (2.58%)
- Accessories: Most ordered (810 orders), best profit margin (62.85%)
- Clothing: Lower volume but promising growth (+12.4% MoM)

**Top Products:** Mountain-200 Silver, Water Bottle – 30 oz., AWC Logo Cap

**Trend Insight:** Revenue declined slightly (-7.5% MoM), possibly due to market saturation or seasonal cooling.

### Europe
- Orders: 7.4K (United Kingdom: 2.7K | France: 2.3K | Germany: 2.2K
- Revenue: $7.8M
- Profit: $3.3M
- Return Rate: 2.2%

### Category Highlights:
- Bikes dominated in revenue and profit, but had the highest return rate at 3.51%
- Accessories maintained strong margins and demand.
- Clothing experienced stable growth (+4.8% MoM), but was still the lowest revenue contributor.

**Top Products:** Consistent with North America – Mountain-200 Silver, Water Bottle – 30 oz., AWC Logo Cap

**Trend Insight:** Europe had the strongest positive revenue momentum (+13.9% MoM) demand growth.

### Pacific
- Orders: 6.1K (Australia: 6.1K)
- Revenue: $7.4M
- Profit: $3.1M
- Return Rate: Highest for the regions at 2.3%

### Category Highlights:
- Bikes led in value ($424.7K)
-  Clothing had the strongest MoM growth (+17.4%), showing late-cycle traction
- Accessories had stable contribution with slightly increased return rates

**Top Products:** Road-750 Black, Water Bottle – 30 oz., AWC Logo Cap

**Trend Insight:** Despite being the smallest region, Pacific outperformed in monthly growth, with all three categories seeing revenue upticks.

### Key Takeaways
Over the three-year period, North America emerged as the **largest market by both volume and revenue**, with the United States leading in orders though the region is beginning to show early signs of plateauing in 2022. **Europe offers strong revenue and profit performance** but also records the highest return rate primarily driven by bike sales highlighting the need to address product quality, sizing, or fulfillment. In contrast, the Pacific region, represented solely by Australia, brought in 6.1K orders and **is exhibiting emerging growth trends, particularly in clothing, suggesting potential for market expansion strategies or targeted campaigns**. Across all regions, Accessories continue to deliver the strongest profit margins, establishing them as high-value contributors to the overall portfolio.

<img width="1459" height="819" alt="image" src="https://github.com/user-attachments/assets/9a696087-ada5-423b-88cd-fdb99be6ffe0" />

To explore the report further [Click here to view the interactive Territory Overview](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&pageName=ReportSectionaf772b59a4d5e4332319&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)
