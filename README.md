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

For a closer look at the dataset used in this project, you can explore the original files here
