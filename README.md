# Hardware-Sales-Insights | SQL | Power BI
### Table of contents

### Project Overview:

This project deliverers a comprehensive Sales Insights solution for AtliQ Hardware, a B2B Indian Hardware company. The primary objective was to transform raw sales data into actionable intelligence, empowering

data-driven strategic decision-making across sales, marketing, and finance departments. The solution encompassed data engineering, advanced analytics, interactive visualizations, and a financial simulation tool.

#### Problem Statement:
  
AtliQ Hardware is currently not fully leveraging its sales data to drive strategic decision-making. This results in missed opportunities for revenue growth, profit margin improvement, and optimized customer engagement.

Key challenges include:

Suboptimal sales strategies due to a lack of granular insights into product and customer performance.

Inefficient resource allocation due to insufficient understanding of regional sales patterns.

Reactive rather than proactive decision-making due to limited 'What-If' scenario planning capabilities."
  
#### AIMS Grid

1.  Purpose: The primary aim of this project is to develop and implement a data-driven sales analytics solution that empowers AtliQ Hardware to:
   
             Enhance strategic decision-making through accessible and interactive sales insights dashboards.

             Improve financial forecasting and planning by providing a Financial Simulator for scenario analysis.

             Optimize sales performance by facilitating data-backed strategies across product, customer, and market domains.

3. Stakeholder:
           - Sales Departent
   
           - Marketing Department

           - Finance Department 

           - Sales Operations Team

           - Data & Analytics Department

           - IT Department 

 
 5. End result: The primary deliverable of this project is a suite of interactive and automated sales analytics dashboards, accompanied by a Financial Simulator tool, designed to provide timely and actionable 

             insights that support data-driven decision-making.

 6. Success Criteria:
    
            Decision-Making Impact: The sales team demonstrates improved decision-making, leading to a measurable reduction in operational costs (e.g., 10% reduction in sales-related expenses) and/or increased 
            revenue.

            Efficiency Gains: Automation of sales analysis tasks results in a significant reduction in manual data gathering and reporting efforts (e.g., 20% time savings for the sales analysis team), allowing 
            for reallocation to strategic activities.

            User Adoption: High user adoption of the dashboards and Financial Simulator across the defined stakeholder groups, measured by usage metrics (e.g., dashboard views, report downloads).

            Improved Forecast Accuracy: Increased accuracy in sales forecasts due to the insights gained from the dashboards

 ### Data Engineering and Technology Stack:

           
          Data Source: 
          ~~~
          https://codebasics.io/resources/sales-insights-data-analysis-project
          ~~~
 
          Data Wrangling: MySQL was used for data extraction, cleaning, transformation, and aggregation. SQL queries were optimized for performance to handle large datasets.
          
          Data Visualization and Analysis: Power BI was employed to create interactive and insightful dashboards.

          Financial Modeling: DAX (Data Analysis Expressions) was utilized within Power BI to build a dynamic Financial Simulator.
          
          Data Modeling: Relational database principles and dimensional modeling techniques were applied to ensure data integrity and efficient querying.


### ER Diagram![Screenshot 2025-03-01 151702](https://github.com/user-attachments/assets/ebee9822-f620-4b83-8c0e-2e853b89ed00)

### Key Analytical Features and Deliverables:

### Sales Analysis Dashboard:

1. Visualized overall sales trends, performance against targets, and key performance indicators (KPIs).

2. Employed Pareto analysis to identify top-selling products and their contribution to revenue.

3. Analyzed the correlation between sales and other business metrics to understand key drivers and inhibitors.

4. Included dynamic rolling averages to smooth out fluctuations and reveal underlying trends.

### Product Analysis Dashboard:

1. Segmented products based on sales and profitability to identify "star" products and "leaky" products.

2. Provided a detailed breakdown of product performance by category and individual SKU.

3. Enabled filtering and drill-down capabilities to explore product-level insights.

4. Explanation of Cluters:

   Cluster5: Indicates a niche, premium cluster that, despite low sales, carries high margins and low COGS. It should be promoted carefully.

   Cluster4: Suggests high sales with medium margins – your key volume drivers, so efficiency is crucial.

   Cluster3: Represents hidden gems that might be underperforming in volume but offer high margins. Consider expanding their reach.

   Cluster2: Warns about clusters with low sales, negative margins, and high COGS; these might be candidates for discontinuation.

   Cluster1: Depicts a steady-performing segment with slight margins where there’s potential for margin improvement

### Market Analysis Dashboard:

1. Visualized sales and profitability across different geographical regions using interactive maps.

2. Segmented customers within each market to understand regional customer behavior.

3. Identified high-growth potential markets and opportunities for expansion.

### Customer Analysis Dashboard:

1. Implemented RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behavior.

2. Calculated and visualized Customer Lifetime Value (CLTV) and compared it with predicted CLTV to assess customer value and retention effectiveness.

3. Analyzed customer behavior patterns to inform personalized marketing and communication strategies.

### Financial Simulator:

1. Developed a dynamic "What-If" analysis tool using DAX to model the impact of changes in pricing, costs, and sales volume on profitability.

2. Enabled scenario planning to evaluate different financial strategies and optimize decision-making.

### Revenue and Gross Profit Breakdown Dashboards:

1. Provided a hierarchical breakdown of revenue and gross profit by various dimensions (region, product category, customer segment, etc.).

2. Identified key profit drivers and areas for margin improvement.

### Enhanced User Experience:

1. Implemented custom tooltips for interactive data exploration.

2. Designed user-friendly filter panes for efficient data slicing and dicing.

3. Employed data storytelling techniques to present insights clearly and concisely.


