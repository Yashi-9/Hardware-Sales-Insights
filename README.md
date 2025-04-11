# Brick & Mortar-Sales-Insights |  Power BI
 
 ## Table of Contents
 - [Project Overview](#project-overview)
 - [Problem Statement](#problem-statement)
 - [AIMS Grid](#aims-grid)
 - [ER Diagram](#er-diagram)
 - [Power BI Analysis and Dashboard](#power-bi-analysis-and-dashboard)
   - [Data Cleaning](#Data-Cleaning)
   - [Sales Analysis Dashboard](#sales-analysis-dashboard)
   - [Product Analysis Dashboard](#product-analysis-dashboard)
   - [Market Analysis Dashboard](#market-analysis-dashboard)
   - [Customer Analysis Dashboard](#customer-analysis-dashboard)
   - [Financial Simulator](#financial-simulator)
   - [Revenue and Gross Profit Breakdown Dashboards](#revenue-and-gross-profit-breakdown-dashboards)
   - [Enhanced User Experience](#enhanced-user-experience)
   - [Recommendations](#recommendations)
 
 
 ### Project Overview:
 
 This project delivers a comprehensive Sales Insights solution for AtliQ Hardware, a B2B Indian Hardware company. The primary objective was to transform raw sales data into actionable intelligence, empowering data-driven strategic decision-making across sales, marketing, and finance departments. The solution encompassed data engineering, advanced analytics, interactive 
 visualizations, and a financial simulation tool.

 Dataset: https://codebasics.io/resources/sales-insights-data-analysis-project
 
 #### Problem Statement:
   
 AtliQ Hardware is currently not fully leveraging its sales data to drive strategic decision-making. This results in missed opportunities for revenue growth, profit margin improvement, and 
 optimized customer engagement.
 
 Key challenges include:
 
 - Suboptimal sales strategies due to a lack of granular insights into product and customer performance.
 
 - Inefficient resource allocation due to insufficient understanding of regional sales patterns.
 
 - Reactive rather than proactive decision-making due to limited 'What-If' scenario planning capabilities.
 
 #### AIMS Grid
 
 1. **Purpose:**  

    The primary aim of this project is to develop and implement a data-driven sales analytics solution that empowers AtliQ Hardware to:  

    - Enhance strategic decision-making through accessible and interactive sales insights dashboards.  

    - Improve financial forecasting and planning by providing a Financial Simulator for scenario analysis.  

    - Optimize sales performance by facilitating data-backed strategies across product, customer, and market domains.
 
 3. **Stakeholders:**  

    - Sales Department  

    - Marketing Department  

    - Finance Department  

    - Sales Operations Team  

    - Data & Analytics Department  

    - IT Department
 
 5. **End Result:**  

    The primary deliverable of this project is a suite of interactive and automated sales analytics dashboards, accompanied by a Financial Simulator tool, designed to provide timely and 
    actionable insights that support data-driven decision-making.
 
 7. **Success Criteria:**
    
    - **Decision-Making Impact:**  
    
      The sales team demonstrates improved decision-making, leading to a measurable increased monthly revenue by 10%.
    
    - **Efficiency Gains:**  

      Automation of sales analysis tasks results in a significant reduction in reporting efforts ( 20% of the time saved for the sales analysis team), allowing 
      reallocation to strategic activities.

    - **Improved Forecast Accuracy:**  
      Increased accuracy in sales forecasts due to the insights gained from the dashboards.
 
 
 ### ER Diagram
 
 The Entity-Relationship (ER) Diagram outlines the relationships between different entities within the sales data. Here’s the ER diagram that visually represents the data model:
 
 ![Screenshot 2025-03-01 151702](https://github.com/user-attachments/assets/ebee9822-f620-4b83-8c0e-2e853b89ed00)
 
 ### Power BI Analysis and Dashboard
 
 #### Data Cleaning
      To ensure the data is clean and ready for analysis, the following steps were taken:

1. **Missing Values**: Filtered out rows where sales values were 0 or negative (less than 1% of the dataset).

2. **Currency Conversion**: All USD sales values were converted into INR for consistency.

3. **Market Data**: Removed any markets that had no associated zones.

4. **Unnecessary Columns**: Removed irrelevant columns that did not contribute to the analysis.

 ### Sales Analysis Dashboard:
 
 1. **Description:** Provides insights into sales trends, key performance indicators, and monthly sales targets.
   
 2. **Key Visuals:**
 
    2.1. Visualized overall sales trends, performance against targets, and key performance indicators (KPIs).
 
    2.2. Employed Pareto analysis to identify top-selling products and their contribution to revenue.
 
 
    2.3. Analyzed the correlation between sales and other business metrics to understand key drivers and inhibitors.
 
 
    2.4. Included dynamic rolling averages to smooth out fluctuations and reveal underlying trends.

 
3. **Insights:**

   3.1 Overall Performance Highlights
    
    - Total Sales: Reached ₹985M, backed by 146K orders, indicating strong customer traction.
    
    - Gross Profit: ₹24.67M.
    
    - Gross Profit Margin: Low at 2.5%, signaling high costs.
    
    - Cost of Goods Sold (COGS): ₹960M, indicating a significant portion of revenue is consumed by operational expenses.
    
    - MoM Sales Growth: +1.5%, with January being the top-performing month for sales volume.
    
    - October Spike: Shows a significant 52.93% increase in performance metrics.
    
    - Sales Volatility: Sales revenue fluctuates considerably compared to the more stable rolling average.
    
    - Approximately 17.70% of products account for 80% of revenue.
    
    - The gap between actual sales and the rolling average suggests inconsistencies in monthly performance.
  
    - "Need Attention" Cluster: Contributes the highest revenue at ₹442M.
    
    - "Loyal" and "New Customers": Generate significantly lower revenue (₹45M and ₹26M respectively).

    
   3.2. Channel-Specific Insights
    
     - Brick & Mortar:
     
       North Zone Dominance: Leads in sales through both owned stores and distribution (₹193.2M).

       Central Underperformance: Distribution channel is under-leveraged (₹75.4M sales).

       South : Low physical footprint success (₹13.2M sales), requiring market analysis.
    
     - E-Commerce

       Central Leadership: Demonstrates strong online revenue generation.

       North Potential: Significant opportunity to grow by replicating Central's online strategies.

       South : Requires urgent action including campaigns.

   3.3 Temporal Trends

    - Strongest Quarters: Quarter 3 and 4 typically exhibit the highest sales across all zones.
   
    - January Surge: Strong positive performance across all channels and MoM% KPIs.
   
    - September & February Slump: Significant downturn in Brick & Mortar stores (September: -27.5%, February: -16.7%) and sharp negative swings in all MoM% KPIs.
   
    - October Peak: Highest overall sales MoM Growth, driven by substantial growth in all channels and a massive surge in order volume.
   
    - E-Commerce Momentum: Increasing contribution towards the end of the year.

  3.4. Target Gap Analysis
  
    - Monthly Target: ₹90M.
    
    - Performance: Missed in multiple months.
  
    - Cumulative shortfall of approximately ₹8M, suggesting missed opportunities or forecasting issues, potentially linked to seasonal promotions or marketing campaigns.

![Screenshot 2025-04-10 183303](https://github.com/user-attachments/assets/0b645f72-1ba0-4f46-994b-24d26dfeabfb)


### Product Analysis Dashboard:

1. **Description:** Focuses on product segmentation to identify star products and underperformers.

2. **Key Visuals:**

  - Segmented products based on sales and profitability to identify "star" products and "leaky" products.

  - Provided a detailed breakdown of product performance by category and individual SKU.

  - Enabled filtering and drill-down capabilities to explore product-level insights.

3. Explanation of Cluters:

  - Cluster5: Indicates a niche, premium cluster that, despite low sales, carries high margins and low COGS. It should be promoted carefully.
   
  - Cluster4: Suggests high sales with medium margins – your key volume drivers, so efficiency is crucial.
   
  - Cluster3: Represents hidden gems that might be underperforming in volume but offer high margins. Consider expanding their reach.
   
  - Cluster2: Warns about clusters with low sales, negative margins even tho with low COGS; these might be candidates for discontinuation.
   
  - Cluster1: Depicts a steady-performing segment with slight margins where there’s potential for margin improvement.
 
4. Insights:

 4.1. Overall Sales Trends

   - Sales Consistency: Clusters 1 maintained steady  total sales throughout the year, representing reliable performers.
   
   - Cluster 4 is has high sales with medium profits and cogs but only few products losing to cluster 1 in overall sales.

   - Roughly 17.7% of products account for ~80% of revenue

   - Prod334 needs attention — very high transaction count but lower sales

   - Q1 &Q4 leads in sales as well as GP Margin- cluster 1 dominates sales in both the quaters.

   - Q2 lags behind in overall  all KPIs
     
 4.2. Channel-Wise Sales by Cluster

   Brick & Mortar:
   
   - Highest sales share in North (51.15%) and Central (51.88%)

   - Product mix varies, but includes large shares of Cluster1 ( Slight margin)

   E-Commerce:

   - South (48.74%) is the dominant contributor — interestingly, it has ~90% Cluster3 products

   - Central and North have higher shares of Cluster1 ,3 & 4  indicating higher-margin mix
   
   - E-commerce comparatively have lesser share of leaky cluster of products (product 2) than Bricks & Motor.
  
![Screenshot 2025-04-10 183351](https://github.com/user-attachments/assets/4cc048f4-9cad-4312-b0b9-d7bb832467e2)

### Market Analysis Dashboard:

1. **Description:** Analyzes market performance across different regions.

2. **Key Visuals:**
  
  -  Visualized sales and profitability across different geographical regions using interactive maps.

  -  Segmented customers within each market to understand regional customer behavior.

  -  Identified high-growth potential markets and opportunities for expansion.

3. **Insights**
   
 - Delhi NCR and Mumbai are the top performers in terms of total sales despite having low value and mid value segments of customers respectively .

 - Bhubaneshwar shows the highest Sales MoM growth at 6.1% followed by Patna at 3.7% and high order MoM growth. This indicates a strong positive trend in sales for this market.

 - Lucknow and Bengaluru show 0.0% both Sales and Orders MoM growth. This suggests stagnant sales in these markets compared to the previous month.

 - Nagpur has the highest number of orders despite being 5th highest in sales followed by Delhi.

 - January is a standout month for multiple regions, including Delhi NCR, Chennai, Kanpur, and Patna, reflecting seasonal peaks or successful campaigns.

 - February also shows strong performance for Bhopal, Nagpur, and Lucknow, indicating early-quarter momentum

 - Surat leads with the highest GP Margin at 4.86%, indicating strong profitability per sale followed by Patna (4.12%) and Bhopal (3.90%)

 - Bengaluru (-20.78%) and Kanpur (-0.49%) presents a significant concern with a highly negative GP Margin, Bengaluru despite having high value customers.

 - High Value Customers are concentrated in markets such as Ahmedabad, Kochi, Chennai, Patna, Lucknow, Surat, Bhubaneshwar, and Bengaluru, highlighting these regions as strategic for premium 
  offerings and  retention efforts.

 - Mid Value Customers dominate in Mumbai, Bhopal, Nagpur, and Hyderabad, presenting opportunities to upsell or cross-sell.

- Low Value Segments are seen in Delhi NCR and Kanpur, which may be driven by high transaction volumes of lower-priced items.

- South Zone underperforms in both sales and margin—deserves strategic expansion and market research

![Screenshot 2025-04-09 203502](https://github.com/user-attachments/assets/f33f6e5c-0fea-4c6e-9f09-d7968ea222a7)

### Customer Analysis Dashboard:

1.**Description:** Uses segmentation (RFM analysis) and predictive CLV modeling to understand customer behavior.

2.**Key Visuals:**

  2.1. Implemented RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behavior. Each customer is scored on a scale of 1 (lowest) to 5 (highest) across 
       the three dimensions:
   
    - Recency: How recently a customer made a purchase

    - Frequency: How often they purchase

   - Monetary: How much they spend

     Based on these scores, customers are categorized into actionable segments.

 2.2. Calculated and visualized Customer Lifetime Value (CLTV) and compared it with predicted CLTV to assess customer value and retention effectiveness.

 2.3. Analyzed customer behavior patterns to inform personalized marketing and communication strategies.

3. **Segment Description**

   Champions                   – recent, frequent, and high spenders.

   Loyal Customers            	-Consistent buyers with high engagement.

   High-Spending New Customers	- Recently acquired and already spending well.

   Potential Loyalists         -		Early signs of becoming loyal; nurture them.

   New Customers	              - 	Recently acquired, yet to build frequency.

   Promising	                  -	Recent purchasers with potential for upsell.

   Need Attention	             - may need re-engagement.

   About to Sleep	             - Previously active, now losing interest.

   At Risk	                    -	High-value customers slipping away; urgent action needed.

   Cannot Lose Them	           -	Previously top-tier; win-back is crucial.

   Hibernating Customers	      - Low recent engagement and value.

   Lost Customers	             - Fully inactive with low lifetime value.

   Other                       -	Does not match above criteria	Requires further review or segmentation refinement.

4.**Customer Behavior Insights**
  
  4.1 Hibernating (11)
 
  - Behavior: These customers are beginning to show early signs of increased activity and spending. With the right engagement strategies, they hold strong potential to evolve into loyal, 
               long-term customers.
  
  - Product Preference: Their purchases are mainly focused on products from Cluster 3 and Cluster 1.
  
  - Channel: This entire segment consists of customers from the E-Commerce channel.
  
  - Sales Trend: There is a steady month-over-month sales growth of around 2%, with particularly strong traction seen in Cluster 5.
  
  - Customer Value: The Customer Lifetime Value (CLV) is approximately ₹2 million higher than the current Lifetime Value (LTV), indicating room for further growth and engagement.

4.2. Promising Customer

     - Behavior: These customers are beginning to show early signs of increased activity and spending. With the right engagement strategies, they hold strong potential to evolve into loyal, 
                long-term customers.
                
    - Product Preference: Their purchases are mainly focused on products from Cluster 3 and Cluster 1.
    
    - Channel: This entire segment consists of customers from the E-Commerce channel.
    
    - Sales Trend: There is a steady month-over-month sales growth of around 2%, with particularly strong traction seen in Cluster 5.
    
    - Customer Value: The Customer Lifetime Value (CLV) is approximately ₹2 million higher than the current Lifetime Value (LTV), indicating room for further growth and engagement.

4.3. Need Attention (3)
   
    - Behavior: Good past monetary value but a drop in frequency and recency. Highest sales but only ranks 3rd in total orders.
  
    - Product Preference: Majorly 1 &3 product clusters.
  
    - Channel: Exclusively Brick & Mortar.
  
    - Sales Trend: Low overall MoM growth across sales and orders; 
    
    - CLV vs LTV: CLV is ~₹26M higher than LTV 

4.4. Loyal Customers (1)
   
   - Behavior: Consistent and frequent purchasers. Strong repeat buying patterns.
   
   - Product Preference: Heavy spenders in Cluster 3 & 1 products.
   
   - Channel: Exclusively E-Commerce.

   - Sales Trend: Lowest overall MoM growth in  sales among all segments but high overall orders growth.
     
   - CLV vs LTV: CLV is ~₹1M higher than LTV.

4.6. Champions (1)

   - Behavior: Top-tier customer with the best RFM scores. Ideal for brand advocacy.

   - Product Preference: Heavy spenders in Cluster 3 & 1 & 4 products.
   
   - Channel: Exclusively Brick & Motor.

   - Sales Trend: Highest Order MoM% among all segments.

   - Growth Concern: Avg overall Sales and order MoM growth.
     
   - CLV vs LTV: CLV is ~₹2M higher than LTV.
 
4.7. New Customers(2)
   
   - Behavior: Recently acquired with early signs of strong engagement.

   -  Product Preference: Heavy spenders in Cluster 3 & 1 products.
   
   - Channel:  Brick & Motor as well as E-Commerce.

   - Sales Trend: least revenue drivers and orders and low overall sales as well as orders MoM growth.

   - CLV vs LTV: CLV is ~₹18M higher than LTV.

4.8. Potential Loyalists(1)

   - Behavior: Increasing order frequency; on the path to becoming loyal customers.

   -  Product Preference: Heavy spenders in Cluster 3 & 1 &4 products.
   
   - Channel:Exclusively E-Commerce.

   - Sales Trend:Low overall MoM trends but highest overall order MoM trensd across sales, orders,

   - CLV vs LTV: CLV is ~₹7M higher than LTV.

4.9. Declining Segments (At-Risk, Lost, About to Sleep, Don’t Lose Them)
    
   - Behavior: Small segments showing signs of disengagement or churn.

   - Sales Trend: Negative MoM trends across sales, orders, and GP.

   - Cluster Insights: Cluster 4 shows some positive Sales MoM% for “About to Sleep”.

   - Most segments show low or declining metrics across all clusters.
   - 
![image](https://github.com/user-attachments/assets/755dbf89-45d2-471e-9950-3d21f5666714)

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
   
![Screenshot 2025-04-09 205118](https://github.com/user-attachments/assets/1cfa18c0-8e17-43cc-a31f-fd8d284cf2cd)

3. Designed user-friendly filter panes for efficient data slicing and dicing.
   
![Screenshot 2025-04-10 184316](https://github.com/user-attachments/assets/44f00f66-abda-4fbc-b356-2ad58ec3f6ad)

4. Employed data storytelling techniques to present insights clearly and concisely.

### Recommendations   

1. Profitability & Cost Optimization:

- COGS Analysis: Break down ₹960M COGS to identify key cost drivers and negotiate better pricing with suppliers. Optimize production processes and logistics.

- Strategic Pricing Review: Analyze product margins and consider value-based pricing for high-margin products, while benchmarking against competitors.

- Focus on High-Margin Clusters: Promote Cluster 3 and 5 through targeted marketing, and assess Cluster 2’s profitability for potential discontinuation.

- Address Low Margin Products: Improve margins in Cluster 1 via cost optimization or price adjustments.

2. Sales Growth & Channel Strategy:

- E-Commerce Expansion: Replicate Central zone’s success in the North and implement interventions in the South zone for better conversion rates.

- Brick & Mortar Strategy: Analyze underperformance in specific regions and address sales slumps in September and February.

- Capitalize on Regional Strengths: Invest in high-growth markets like Bhubaneswar and Patna, and target premium products in key cities.

3. Customer Relationship Management (CRM):

- Re-engage “Need Attention” Customers: Implement campaigns to boost frequency and recency in Brick & Mortar segments.

- Loyal Customer Growth: Introduce loyalty programs with personalized offers to increase spending.

- Convert New Customers: Focus on onboarding and engaging new customers through personalized recommendations.

- Reactivation of Declining Segments: Address disengagement with targeted reactivation campaigns.

- Optimize Inventory: Focus on the 17.7% of products that drive 80% of revenue and manage slower-moving items carefully.

- Investigate Prod334: Understand why it has high transactions but low sales, and consider strategies to boost its value.

- Capitalize on January Surge: Replicate successful January strategies in future months.



