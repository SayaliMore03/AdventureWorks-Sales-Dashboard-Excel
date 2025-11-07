This project is a comprehensive analysis of the AdventureWorks retail company, built entirely within Excel. It transforms 7 disconnected raw data files into a fully interactive, 3-part "Hub and Spoke" dashboard. The report analyzes performance from three perspectives: a high-level Executive Hub, a Salesperson Performance deep-dive, and a Product & Reseller Analysis.

Dashboards
1. The "Home" Hub (Executive Overview)
This dashboard is the main landing page, providing a high-level "health check" of the entire business. It tracks top-level KPIs and serves as the navigation center for the detailed "spoke" reports.

2. Spoke 1: Salesperson Performance
This report is for Sales Managers. It provides a detailed breakdown of team performance against targets, allowing for interactive filtering by individual salesperson, region, and year.

3. Spoke 2: Product & Reseller Analysis
This report is for Product and Marketing Managers. It identifies the most (and least) profitable products, categories, and customer segments.

🎯 Project Objective
To develop a comprehensive Retail Sales & Performance dashboard, built on a centralized data model, that provides actionable insights into key performance metrics (KPIs) and time-based trends. This enables stakeholders to effectively monitor company-wide sales, analyze product profitability, and track team performance against targets.

🛠️ My Data Analyst Workflow
This project was built from the ground up, following the complete data analysis workflow:

Extract (Power Query):

Connected to 7 different raw CSV files (Sales, Targets, Product, Region, Reseller, etc.).

Performed extensive data cleaning and transformation. This included correcting data types, handling nulls/errors, and formatting keys for modeling.

Model (Power Pivot):

Built a relational "Galaxy Schema" by linking 2 fact tables (Sales, Targets) and 5 dimension tables.

This data model is the core of the project, enabling scalable analysis across all 7 tables without a single VLOOKUP.

Created a Calendar table to support all time-intelligence calculations.

Analyze (DAX):

Wrote over 10 custom DAX measures to create advanced, contextual KPIs that don't exist in the raw data.

Key Measures Include:

Total Sales

Total Profit

[Sales vs Target %]

[Sales PY] (Previous Year Sales)

[YoY Sales Growth %]

Visualize (PivotCharts & Slicers):

Built all 3 dashboard sheets using interactive PivotCharts and Slicers.

Established a "Hub and Spoke" design, using navigation buttons to create a user-friendly experience that feels like a web application.

💡 Key Findings & Recommendations
This analysis revealed three critical insights that can lead to immediate business action.

1. Unlocking Profit in High-Margin Categories
Finding: The "Bikes" category drives 81% of all sales, but the "Product Profitability" analysis shows that "Mountain Frames" and "Accessories" are significantly more profitable.

Recommendation: Launch a "cross-sell" campaign to bundle high-margin accessories (like helmets, gloves) with every bike purchase. Shift marketing focus to the high-profit "custom-builder" market that buys frames and components.

2. Our Sales Targets Are Unrealistic
Finding: The Sales_Performance dashboard revealed that not a single salesperson is hitting 100% of their target. The top performer is only at 71%.

Recommendation: The sales quota methodology must be re-evaluated. When top performers can't reach their goals, it demotivates the team. I recommend using this dashboard to set challenging but achievable data-driven goals for the next fiscal year.

3. Explosive Growth Followed by a Decline
Finding: The YoY Growth % card shows an explosive, unsustainable 201% growth in 2018, followed by a sharp decline in 2020 and a full data drop-off in 2021.

Recommendation: Investigate the cause of the 2018 spike (e.g., a specific new product or a one-time marketing campaign) to see if that success can be replicated. The 2021 data drop also highlights a potential data pipeline issue that needs immediate investigation.
