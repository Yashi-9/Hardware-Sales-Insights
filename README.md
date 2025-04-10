# Hardware-Sales-Insights | SQL | Power BI
 
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
 - [Insights and Recommendations](#insights-and-recommendations)
 
 
 ### Project Overview:
 
 This project delivers a comprehensive Sales Insights solution for AtliQ Hardware, a B2B Indian Hardware company. The primary objective was to transform raw sales data into actionable intelligence, empowering
 data-driven strategic decision-making across sales, marketing, and finance departments. The solution encompassed data engineering, advanced analytics, interactive visualizations, and a financial simulation tool.

 Dataset: https://codebasics.io/resources/sales-insights-data-analysis-project
 
 #### Problem Statement:
   
 AtliQ Hardware is currently not fully leveraging its sales data to drive strategic decision-making. This results in missed opportunities for revenue growth, profit margin improvement, and optimized customer 
 engagement.
 
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
 
   #### Data Cleaning
 
   1.Missing Value Treatement:
   
   The transaction table has a ton of 0 and negative values in the sales_amount column . Since the % of these records compared to total dataset is very low ie <=1% , it is safe to filter it out.
   
   2.Sales amount column in transcation table has a few USD currency, converted it to INR.
   
   3.The market table has two international markets with no zones allocated. Filtering it out using the dropdown.

   4. Removed and hide columns not required for processing.

 ### Sales Analysis Dashboard:
 
 1. **Description:** Provides insights into sales trends, key performance indicators, and monthly sales targets.
   
 2. **Key Visuals:**
 
    2.1. Visualized overall sales trends, performance against targets, and key performance indicators (KPIs).
 
    2.2. Employed Pareto analysis to identify top-selling products and their contribution to revenue.
 
 
    2.3. Analyzed the correlation between sales and other business metrics to understand key drivers and inhibitors.
 
 
    2.4. Included dynamic rolling averages to smooth out fluctuations and reveal underlying trends.

 
3. **Insights:**
   
   3.1. Overall Sales Trends
   
    - Strong Overall Sales: Total sales show a positive trend across the year, peaking in January, July, and notably in October & November indicating seasonal or campaign-driven uplift.

    - Significant Drop in September: A sharp decline in sales, possibly due to supply chain issues or demand fluctuation.

    - Volatile Growth: Month-over-month % fluctuates considerably.
 
   - Roughly 17.7% of products account for ~80% of revenue.

   3.2. Channel Performance:
 
   - Brick & Mortar Dominance: Brick & Mortar sales consistently contribute the largest share of the total sales throughout the year.

   - E-Commerce Growth: E-Commerce sales show a significant upward trend, becoming a more substantial contributor to overall sales, especially towards the end of the year  suggesting increased online engagement 
     or effective digital campaigns.

4. 🎯 Target Gap Analysis
   
   - Monthly Target: ₹90M

   - Performance: Missed in multiple months.

   - Cumulative Shortfall: Approx. ₹8M – Indicates missed opportunities or forecasting issues.


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

    - Monthly Target: ₹90M

    - Performance: Missed in multiple months.

    - Cumulative Shortfall: Approx. ₹8M – Indicates missed opportunities or forecasting issues.



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

   - roughly 17.7% of products account for ~80% of revenue

   - Prod334 needs attention — very high transaction count but lower sales

   - Q1 &Q4 leads in sales as well as GP Margin- cluster 1 dominates sales in both the quaters.

   - Q2 lags behind in overall  all KPIs

   -  overall cluster 1  of products dominates both channels


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

 - High Value Customers are concentrated in markets such as Ahmedabad, Kochi, Chennai, Patna, Lucknow, Surat, Bhubaneshwar, and Bengaluru, highlighting these regions as strategic for premium offerings and 
  retention efforts.

 - Mid Value Customers dominate in Mumbai, Bhopal, Nagpur, and Hyderabad, presenting opportunities to upsell or cross-sell.

- Low Value Segments are seen in Delhi NCR and Kanpur, which may be driven by high transaction volumes of lower-priced items.

- South Zone underperforms in both sales and margin—deserves strategic expansion and market research


![Screenshot 2025-04-09 203502](https://github.com/user-attachments/assets/f33f6e5c-0fea-4c6e-9f09-d7968ea222a7)

### Customer Analysis Dashboard:

1.**Description:** Uses segmentation (RFM analysis) and predictive CLV modeling to understand customer behavior.

2.**Key Visuals:**

  2.1. Implemented RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behavior. Each customer is scored on a scale of 1 (lowest) to 5 (highest) across the three dimensions:

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

4. **Customer Behavior Insights**

  4.1. Hibernating Customers (11)

    - Behavior: Previously high-value customers who are now inactive. Represents a significant lost opportunity.
   
    - Product Preference: Primarily purchase from Cluster 3 & 1 products, contributing both revenue and gross profit.
   
    - Channel: Slight dominance by E-Commerce customers.

    - Sales Trend: Average MoM growth in sales and orders, with positive signals in Cluster 4.

    - CLV vs LTV: CLV is ~₹10M higher than LTV, indicating untapped future potential.


4.2. Promising Customers

   - These customers are showing early signs of increased activity and spending. With the right engagement strategies, they have the potential to become loyal customers.
 
   - Product Preference: Primarily purchase products from Cluster 3 and Cluster 1.
  
   - Channel: All customers in this segment are from the E-Commerce channel.
  
   - Sales Trend: Month-over-month (MoM) sales growth is approximately 2%, with particularly strong performance in Cluster 5.
  
   - Customer Value:CLV is ~₹2M higher than LTV

3. Need Attention (3)
   
    - Behavior: Good past monetary value but a drop in frequency and recency. Highest sales but only ranks 3rd in total orders.
  
    - Product Preference: Majorly 1 &3 product clusters.
  
    - Channel: Exclusively Brick & Mortar.
  
    - Sales Trend: Low overall MoM growth across sales and orders; 
    
    - CLV vs LTV: CLV is ~₹26M higher than LTV 

5. Loyal Customers (1)
   
   - Behavior: Consistent and frequent purchasers. Strong repeat buying patterns.
   
   - Product Preference: Heavy spenders in Cluster 3 & 1 products.
   
   - Channel: Exclusively E-Commerce.

   - Sales Trend: Lowest overall MoM growth in  sales among all segments but high overall orders growth.
     
   - CLV vs LTV: CLV is ~₹1M higher than LTV.

7. Champions (1)

   - Behavior: Top-tier customer with the best RFM scores. Ideal for brand advocacy.

   - Product Preference: Heavy spenders in Cluster 3 & 1 & 4 products.
   
   - Channel: Exclusively Brick & Motor.

   - Sales Trend: Highest Order MoM% among all segments.

   - Growth Concern: Avg overall Sales and order MoM growth.
     
   - CLV vs LTV: CLV is ~₹2M higher than LTV.
 
8. New Customers(2)
   
   - Behavior: Recently acquired with early signs of strong engagement.

   -  Product Preference: Heavy spenders in Cluster 3 & 1 products.
   
   - Channel:  Brick & Motor as well as E-Commerce.

   - Sales Trend: least revenue drivers and orders and low overall sales as well as orders MoM growth.

   - CLV vs LTV: CLV is ~₹18M higher than LTV.



7. Potential Loyalists(1)

   - Behavior: Increasing order frequency; on the path to becoming loyal customers.

   -  Product Preference: Heavy spenders in Cluster 3 & 1 &4 products.
   
   - Channel:Exclusively E-Commerce.

   - Sales Trend:Low overall MoM trends but highest overall order MoM trensd across sales, orders,

   - CLV vs LTV: CLV is ~₹7M higher than LTV.

9. Declining Segments (At-Risk, Lost, About to Sleep, Don’t Lose Them)
    
   - Behavior: Small segments showing signs of disengagement or churn.

   - Sales Trend: Negative MoM trends across sales, orders, and GP.

   - Cluster Insights: Cluster 4 shows some positive Sales MoM% for “About to Sleep”.

   - Most segments show low or declining metrics across all clusters.



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





