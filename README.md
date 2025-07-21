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

## Part 1: Sales Overview Page
### Summary of Insights:
Revenue peaked in 2021 ($9.3M) and stabilized in 2022 ($9.2M)
Profit mirrored revenue: $4.0M in 2021 to $3.9M in 2022
Orders steadily increased from 2.6K (2020) to 11.8K (2022)
Return rate improved: 3.3% in 2020 to 2.1% in 2022

### Seasonality:
Late 2021 saw the most substantial monthly growth reaching $1.6M in revenue likely strong seasonal demand or promotional activity
Revenue remained relatively flat throughout 2020, fluctuating between $585K and $326K. However, beginning in Q2 2021, growth became more pronounced, with monthly sales steadily increasing through 2022

### Category & Product Highlights:
Accessories had the highest order volume (17K orders) reflecting the high-frequency, low-cost nature of these products.
Bikes drove most revenue: $23.6M over 3 years
Clothing experienced a noticeable increase in orders over time, particularly in 2022, signaling growing interest in apparel
Water Bottle – 30 oz. was the most ordered product (4K orders)
Sport-100 Helmets had highest revenue but also highest return rates (>3.3%)
At the subcategory level, Tires and Tubes contributed over a third of total orders (36.1% or 9.1K) while Shorts registered the highest return rate among all subcategories, making up 2.2% of total returns (40 returns).
