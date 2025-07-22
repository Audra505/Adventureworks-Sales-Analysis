# AdventureWorks Analysis (2020-2022)
---

## Table of Contents
- [Project Summary](#project-summary)
- [Part 1: Sales Overview ](#part-1-Sales-Overview)
- [Part 2: Regional Performance](#part-2-Regional-Performance)
- [Part 3: Product Insights](#part-3-Product-Insights)
- [Part 4: Customer Insights](#part-4-Customer-Insights)
- [Part 5: Recommendations & Next Steps](#part-5-recommendations--next-steps)
- [Addendum: Notes on Data Modeling & Cleaning](#addendum-notes-on-data-modeling-cleaning)

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

---
## Part 1: Sales Overview
[Back to Table of Contents](#table-of-contents)
### Summary of Insights:
Revenue peaked in 2021 ($9.3M) and stabilized in 2022 ($9.2M). Profit mirrored revenue: $4.0M in 2021 to $3.9M in 2022. Orders steadily increased from 2.6K (2020) to 11.8K (2022) and Return rate improved 3.3% in 2020 to 2.1% in 2022.

### Seasonality:
Late 2021 saw the most substantial monthly growth reaching $1.6M in revenue likely strong seasonal demand or promotional activity. Revenue remained relatively flat throughout 2020, fluctuating between $585K and $326K. However, beginning in Q2 2021, growth became more pronounced, with monthly sales steadily increasing through 2022

### Category & Product Highlights:
Accessories had the highest order volume (17K orders) reflecting the high-frequency, low-cost nature of these products. Bikes drove the most revenue: $23.6M over 3 years, Clothing experienced a noticeable increase in orders over time, particularly in 2022, signaling growing interest in apparel. Water Bottle – 30 oz. was the most ordered product (4K orders) while Sport-100 Helmets had highest revenue but also highest return rates (>3.3%). At the subcategory level, Tires and Tubes contributed over a third of total orders (36.1% or 9.1K) while Shorts registered the highest return rate among all subcategories, making up 2.2% of total returns (40 returns).

<img width="1461" height="812" alt="image" src="https://github.com/user-attachments/assets/420bcbcf-5478-4cba-adfe-1c0a23712ab5" />

To explore the report further [Click here](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)

---

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

To explore the report further [Click here](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&pageName=ReportSectionaf772b59a4d5e4332319&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)

---
## Part 3: Product Insights
[Back to Table of Contents](#table-of-contents)

### Summary of Insights 
#### Highest Return Rate Product: **Sport-100 Helmet, Red**
A top-selling accessory product, it demonstrated strong overall performance from 2020 to 2022, securing a top-5 rank by orders. Over the observed period, $73.4K was generated in revenue, $46K in profit, and 2.1K in orders.

**Monthly analysis** revealed fluctuating revenue and order trends, with seasonality in both spikes and slowdowns. Despite this, the product met revenue targets in only 6 of the 12 tracked months, with performance dips often coinciding with lower order volumes. Highlighting a potential need to optimize inventory cycles or promotional timing to align with high-demand periods.

The **return rate averaged 3.33%, increasing slightly year over year**. While return spikes such as 5.31% in May 2022 raised expectation concerns, it’s notable that higher returns often occurred during periods of high sales. This suggests that increased returns may be a byproduct of higher volume rather than dissatisfaction.

A **regional comparison** brought further clarity:
- North America delivered the highest revenue ($32.1K) and profit, despite having one of the most volatile return trends and missing revenue targets in 6 months.
- Europe had the lowest return rate (2.79%), but missed targets the most often (8 months), suggesting weak demand despite low return friction.
- Pacific trailed in both revenue and orders and recorded the highest return rate (4.19%), indicating potential  unmet expectations in that market.

The interactive price adjustment tool can be used for strategic price changes and exploration to optimize profitability without sacrificing volume.

### Key Takeaways:
- Sales volume drives returns, but return spikes do not necessarily signal poor product performance
- Target misses are often tied to low order periods, not just return behavior
- Each region requires a tailored approach, with North America leaning into demand strength, Europe needing promotional improvements, and Pacific demanding a closer look at the customer experience.

<img width="1457" height="816" alt="image" src="https://github.com/user-attachments/assets/ddb89540-bd59-4c37-8835-9e1a2303744d" />

To explore the report further [Click here](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&pageName=ReportSectionaf772b59a4d5e4332319&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)

---
## Part 4: Customer Insights
[Back to Table of Contents](#table-of-contents)

### Summary of Insights: 
Between 2020 and 2022, AdventureWorks served over 17.4K customers, generating 25.2K orders with a customer retention rate of 33.63% and revenue per customer averaging $1.4K. Customer growth showed a steady upward trend, increasing from 3K in 2020 to over 11K by 2022, signaling successful customer acquisition efforts. However, revenue per customer declined over the same period from $2K in 2020 to $875 in 2022 indicating that while more customers are being acquired, their individual spending is decreasing.

#### Key customer segments include:
- **Income Tier:** Customers in the Average and Low income tiers generated the highest order volumes, while In contrast, high and very high income segments were underrepresented, pointing to an opportunity for targeted marketing or product bundling in those tiers. 
- **Occupation:** Professionals and skilled manual workers led the order volume, while management and clerical roles followed with moderate contributions. 
- **Educational Level:** Undergraduates dominated, accounting for more than half of all orders (14.5K), reinforcing the brand’s appeal to mid-education consumers.
- **Age Groups:** The most active buyers were aged 51–70, with those over 70 also contributing significantly, suggesting a strong middle-aged to senior customer base.
- **Gender:** Females slightly outperformed males in revenue per customer ($1.5K vs $1.4K), with similar ordering patterns across age and income tiers.
- **Marital Status:** Single customers had a higher average revenue per customer ($1.5K) than married ones ($1.4K), although married customers made up a larger proportion of the top spenders.

Finally, the top 100 customers led by individuals like Mr. Maurice Shan and Mrs. Janet Munoz consistently spent over $10K, reinforcing the importance of a loyal high-value customer and the potential to expand average order size across similar customer profiles.

<img width="1453" height="812" alt="image" src="https://github.com/user-attachments/assets/cda93178-5744-4aa8-a732-19726bfa45c6" />

To explore the report further [Click here](https://app.powerbi.com/reportEmbed?reportId=70d82fdb-7fcc-4580-bd4c-dd060f027cbd&pageName=ReportSectionaf772b59a4d5e4332319&autoAuth=true&ctid=f4e2981a-ee27-48df-9435-c46bbd4f1e7d)

 ---
 ## Part 5: Recommendations & Next Steps
[Back to Table of Contents](#table-of-contents)

### Executive Takeaways 
- **Customer acquisition efforts are succeeding but at the cost of profitability per customer.** The customer base nearly quadrupled from 3K to 11K, but revenue per customer dropped by 56% (from $2K to $875). This signals a shift to volume driven growth that may not be sustainable without improving customer value or targeting higher spending segments.

- **High volume products drive success but also carry return risks.** Best-selling items like the Sport-100 Helmet generated strong revenue but also had the highest return rates. Product level performance should be analyzed further to reduce return-related losses.

- **North America remains the strongest market, but future growth may come from the Pacific.** While North America leads in orders and revenue, the Pacific region showed the fastest MoM growth and emerging demand for clothing suggesting investment potential in product expansion and marketing in underpenetrated regions.

- **Targeted customer segmentation could unlock additional revenue.** Most purchases came from average and low-income customers aged 51–70, with undergraduates and professionals dominating. High-income tiers and younger segments are underrepresented highlighting a missed opportunity for product repositioning or bundling strategies. 

- **Operational improvements are driving better customer experience.** Return rates declined from 3.3% to 2.1% despite order growth  a sign of improved fulfillment processes or satisfaction levels that should be maintained and scaled.

  ### Next Steps
- **Enhance Customer Value:** By developing customer retention programs e.g., loyalty programs, cross-sell strategies, or premium tiers to increase revenue per customer.
- **Investigate High Return Products:** A deeper dive needs to be done into return drivers (e.g., sizing, quality, expectations) for best-sellers like the Sport-100 Helmet to reduce any avoidable losses. 
- **Invest in Pacific Region Expansion:** Pilot targeted apparel campaigns and localized promotions to capitalize on fast-growing demand, especially in underpenetrated markets like Australia.
- **Engage Untapped Segments:** Campaigns tailored to high-income and younger demographics can be utilized through product bundling, influencer partnerships, and rebranding offers to boost engagement and conversion.
- **Preserve Operational Gains:** Continue to optimize fulfillment and returns management to maintain low return rates and customer satisfaction.

---
## Part 5: Addendum: Notes on Data Modeling & Cleaning
[Back to Table of Contents](#table-of-contents)

The dataset was provided as flat .csv files covering Sales, Product, Customer, Category etc, data. Using Power Query, I cleaned column names and removed unnecessary fields to streamline the model. Calculated columns and DAX measures were created to support the analysis. Tables were connected using proper one-to-many relationships within Power BI’s data model view, ensuring accurate aggregation and filtering. 


