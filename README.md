# Hardware-Sales-Insights | SQL | Power BI
 
 ## Table of Contents
 - [Project Overview](#project-overview)
 - [Problem Statement](#problem-statement)
 - [AIMS Grid](#aims-grid)
 - [ER Diagram](#er-diagram)
 - [Power BI Analysis and Dashboard](#power-bi-analysis-and-dashboard)
   - [Sales Analysis Dashboard](#sales-analysis-dashboard)
   - [Product Analysis Dashboard](#product-analysis-dashboard)
   - [Market Analysis Dashboard](#market-analysis-dashboard)
   - [Customer Analysis Dashboard](#customer-analysis-dashboard)
   - [Financial Simulator](#financial-simulator)
   - [Revenue and Gross Profit Breakdown Dashboards](#revenue-and-gross-profit-breakdown-dashboards)
   - [Enhanced User Experience](#enhanced-user-experience)
 - [Insights and Recommendations](#insights-and-recommendations)
 
 
 ### Project Overview:
 
 This project deliverers a comprehensive Sales Insights solution for AtliQ Hardware, a B2B Indian Hardware company. The primary objective was to transform raw sales data into actionable intelligence, empowering
 data-driven strategic decision-making across sales, marketing, and finance departments. The solution encompassed data engineering, advanced analytics, interactive visualizations, and a financial simulation tool.
 
 #### Problem Statement:
   
 AtliQ Hardware is currently not fully leveraging its sales data to drive strategic decision-making. This results in missed opportunities for revenue growth, profit margin improvement, and optimized customer engagement.
 
 Key challenges include:
 
 - Suboptimal sales strategies due to a lack of granular insights into product and customer performance.
 
 - Inefficient resource allocation due to insufficient understanding of regional sales patterns.
 
 - Reactive rather than proactive decision-making due to limited 'What-If' scenario planning capabilities."
 
 #### AIMS Grid
 
 1. **Purpose:**  
    The primary aim of this project is to develop and implement a data-driven sales analytics solution that empowers AtliQ Hardware to:  
    - Enhance strategic decision-making through accessible and interactive sales insights dashboards.  
    - Improve financial forecasting and planning by providing a Financial Simulator for scenario analysis.  
    - Optimize sales performance by facilitating data-backed strategies across product, customer, and market domains.
 
 2. **Stakeholders:**  
    - Sales Department  
    - Marketing Department  
    - Finance Department  
    - Sales Operations Team  
    - Data & Analytics Department  
    - IT Department
 Strong gains in both Brick & Mortar and E-Commerce
 
 3. **End Result:**  

    The primary deliverable of this project is a suite of interactive and automated sales analytics dashboards, accompanied by a Financial Simulator tool, designed to provide timely and actionable insights that 
    support data-driven decision-making.
 
 5. **Success Criteria:**  

    - **Decision-Making Impact:**  
    
      The sales team demonstrates improved decision-making, leading to a measurable reduction in operational costs (e.g., 10% reduction in sales-related expenses) and/or increased revenue.
    
    - **Efficiency Gains:**  

      Automation of sales analysis tasks results in a significant reduction in manual data gathering and reporting efforts (e.g., 20% time savings for the sales analysis team), allowing reallocation to strategic 
      activities.

    - **User Adoption:**  
      High user adoption of the dashboards and Financial Simulator across the defined stakeholder groups, measured by usage metrics (e.g., dashboard views, report downloads).

    - **Improved Forecast Accuracy:**  
      Increased accuracy in sales forecasts due to the insights gained from the dashboards.
 
 
 ### ER Diagram![Screenshot 2025-03-01 151702](https://github.com/user-attachments/assets/ebee9822-f620-4b83-8c0e-2e853b89ed00)
 
 ### Power BI Analysis and Dashboard
 
 ### Sales Analysis Dashboard:
 - **Description:** Provides insights into sales trends, key performance indicators, and monthly sales targets.
   
 - **Key Visuals:**
 
 1. Visualized overall sales trends, performance against targets, and key performance indicators (KPIs).
 📦 E-Commerce Momentum: Accelerated toward the end of the year, indicating:
 
 2. Employed Pareto analysis to identify top-selling products and their contribution to revenue.
 
 
 3. Analyzed the correlation between sales and other business metrics to understand key drivers and inhibitors.
 
 
 4. Included dynamic rolling averages to smooth out fluctuations and reveal underlying trends.

 
 - **Insights:**
1. Overall Sales Trends
   
   Strong Overall Sales: Total sales show a positive trend across the year, peaking in January, July, and notably in October & November indicating seasonal or campaign-driven uplift.

   Significant Drop in September: A sharp decline in sales, possibly due to supply chain issues or demand fluctuation.

   Volatile Growth: Month-over-month % fluctuates considerably.

    Roughly 17.7% of products account for ~80% of revenue.
   
3. Channel Performance:
 
 Brick & Mortar Dominance: Brick & Mortar sales consistently contribute the largest share of the total sales throughout the year.

 E-Commerce Growth: E-Commerce sales show a significant upward trend, becoming a more substantial contributor to overall sales, especially towards the end of the year  suggesting increased online engagement or 
 effective digital campaigns.

🎯 Target Gap Analysis
Monthly Target: ₹90M

Performance: Missed in multiple months.

Cumulative Shortfall: Approx. ₹8M – Indicates missed opportunities or forecasting issues.


3. Specific Observations:
 
 January Surge: All three channels and all three MoM% KPIs show strong positive performance in January.
 September & feb Slump: September experienced a significant downturn across bricks & motor Stores 27.5%, same with feb 16.7% and a sharp negative swing in all MoM% KPIs.
 October Peak: October stands out with the highest overall sales mom Growth , driven by substantial growth in all channels and a massive surge in order volume.
 E-Commerce Momentum: The increasing contribution of E-Commerce suggests a growing online customer base or successful online sales initiatives.% of Revenue
 approximately 17.70% of products are responsible for 80% of revenue
 The rolling average shows a smoothing effect, indicating whether recent sales are above or below the general trend."
   :
🚀 October Peak: Highest MoM sales growth, driven by:

Strong gains in both Brick & Mortar and E-Commerce

Massive surge in order volume

📦 E-Commerce Momentum: Accelerated toward the end of the year, indicating:

A growing online customer base

Success of digital sales strategies

4. 🎯 Target Gap Analysis

Monthly Target: ₹90M

Performance: Missed in multiple months.

Cumulative Shortfall: Approx. ₹8M – Indicates missed opportunities or forecasting issues.



![Screenshot 2025-04-09 203122](https://github.com/user-attachments/assets/df5226e1-c765-47b1-a50e-2c9821217dec)

### Product Analysis Dashboard:

- **Description:** Focuses on product segmentation to identify star products and underperformers.

- **Key Visuals:**

1. Segmented products based on sales and profitability to identify "star" products and "leaky" products.

2. Provided a detailed breakdown of product performance by category and individual SKU.

3. Enabled filtering and drill-down capabilities to explore product-level insights.

4. Explanation of Cluters:

   Cluster5: Indicates a niche, premium cluster that, despite low sales, carries high margins and low COGS. It should be promoted carefully.

   Cluster4: Suggests high sales with medium margins – your key volume drivers, so efficiency is crucial.

   Cluster3: Represents hidden gems that might be underperforming in volume but offer high margins. Consider expanding their reach.

   Cluster2: Warns about clusters with low sales, negative margins even tho with low COGS; these might be candidates for discontinuation.

   Cluster1: Depicts a steady-performing segment with slight margins where there’s potential for margin improvement.
 Insights:

🔹 Sales Consistency: Clusters 1 maintained steady sales throughout the year, representing reliable performers.
Quantity mom% dec in Q2 mainly due dec in quantity in cluster 1 products

 Cluster 4 is our key drivers of sales with medium profits and cogs

 2. Channel-Wise Sales by Cluster
Brick & Mortar:

Dominated by Cluster1 (51.11%) 

E-Commerce:

More balanced spread:

Cluster4 (26.74%) and Cluster5 (27.30%) together make up over 50%, indicating E-Commerce favors high-margin SKUs.

E-Commerce is a high-potential, profitable channel.

![Screenshot 2025-04-09 203418](https://github.com/user-attachments/assets/9dbb533b-71f2-4463-b0fc-170e6e8dba55)


### Market Analysis Dashboard:

- **Description:** Analyzes market performance across different regions.

- **Key Visuals:**
  
1. Visualized sales and profitability across different geographical regions using interactive maps.

2. Segmented customers within each market to understand regional customer behavior.

3. Identified high-growth potential markets and opportunities for expansion.


🔹 Top-Performing States: South and West zones delivered highest sales and profitability—potential for deeper market penetration.
🔹 Growth Opportunity: East zone has low revenue but decent customer base, suggesting untapped potential with targeted campaigns.
🔹 Market Share by Profitability: Not all high-sales zones contribute to profit equally—pricing and cost strategies may need recalibration.

🛠️ Insight:
Resource allocation should favor the South for expansion, while East presents a conversion opportunity via pricing and regional partnerships.

![Screenshot 2025-04-09 203502](https://github.com/user-attachments/assets/f33f6e5c-0fea-4c6e-9f09-d7968ea222a7)

### Customer Analysis Dashboard:

- **Description:** Uses segmentation (RFM analysis) and predictive CLV modeling to understand customer behavior.

- **Key Visuals:**

1. Implemented RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behavior.

2. Calculated and visualized Customer Lifetime Value (CLTV) and compared it with predicted CLTV to assess customer value and retention effectiveness.

3. Analyzed customer behavior patterns to inform personalized marketing and communication strategies.


**RFM Segmentation:**
        "We have a large segment of 'Loyal Customers,' which are our most valuable customers. We should focus on retaining them."
         "The 'At Risk' segment is growing, indicating a potential problem with customer churn. We need to address this."
      **Customer Lifetime Value (CLV):**
         "The average CLV is \[Amount], which is \[above/below] our target. We need to implement strategies to increase customer lifetime value."
    **Order Trends:**
        "The number of orders is declining in the \[Customer Segment], which is concerning."

![Screenshot 2025-04-09 203544](https://github.com/user-attachments/assets/11772110-0810-41bb-902f-edd120b9b168)

### Financial Simulator:

- **Description:** A "what-if" tool to explore pricing, cost optimization, and forecast scenarios.

- **Key Visuals:**
  
1. Developed a dynamic "What-If" analysis tool using DAX to model the impact of changes in pricing, costs, and sales volume on profitability.

2. Enabled scenario planning to evaluate different financial strategies and optimize decision-making.

![Screenshot 2025-04-09 203625](https://github.com/user-attachments/assets/dc0fd731-d394-4591-a838-ca79090a6d44)

### Revenue and Gross Profit Breakdown Dashboards:

- **Description:** Breaks down overall revenue and gross profit by segments such as region and product category.

- **Key Visuals:**
  
1. Provided a hierarchical breakdown of revenue and gross profit by various dimensions (region, product category, customer segment, etc.).

2. Identified key profit drivers and areas for margin improvement.
![Screenshot 2025-04-09 203659](https://github.com/user-attachments/assets/933bcb00-4a81-4464-a083-3fda0c83ae6e)
![Screenshot 2025-04-09 204932](https://github.com/user-attachments/assets/153da911-0b9f-4221-a5cf-f7975a5219c5)

### Enhanced User Experience:

- **Description:** Focuses on the dashboard’s interactivity and design enhancements.

 
- **Features:**

1. Implemented custom tooltips for interactive data exploration.

2. Designed user-friendly filter panes for efficient data slicing and dicing.

3. Employed data storytelling techniques to present insights clearly and concisely.


![Screenshot 2025-04-09 205118](https://github.com/user-attachments/assets/1cfa18c0-8e17-43cc-a31f-fd8d284cf2cd)


