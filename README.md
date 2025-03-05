# Hardware-Sales-Insights | SQL | Power BI
### Table of contents
#### Problem Statement:
  
  An India-based computer hardware company, struggles with acquiring more customers and tracking its sales and growth in a competitive market.Currently, the company struggles with limited data visibility and 
  relies on verbal reports, making it difficult to assess performance. Implementing a Power BI sales dashboard will provide real-time insights, enabling data-driven decisions to optimize sales strategies and drive
  growth.
  
#### AIMS Grid

1.  Purpose: Improve sales tracking, enhance data-driven decision-End result - An automated dashboard providing quick and latest sights to support Data-driven decision making.making, and optimize sales   
    strategies to drive business growth.

2. Stakeholder:
       - Sales Director
       - Marketing Team
       - Customer Service Team
       - Data & Analytics Tea
       -  IT
 
 3. End result:An automated dashboard providing quick and latest sights to support Data-driven decision making.
    
 4. Success Criteria
      - Dashboard uncovering sales order insights with the latest data available.
      - Sales team able to make better decisions and prove 10% cost saving of total spend.
      - Sales analysis stops data gathering manually to save 20% of business time and reinvest it value added activity.
  
### ER Diagram![Screenshot 2025-03-01 151702](https://github.com/user-attachments/assets/ebee9822-f620-4b83-8c0e-2e853b89ed00)

### Analysis using MySQL

 1. Basic query to retrieve all customer data:

 ~~~
SELECT * from customers;
~~~
To identify types of customers
                                 
 2. Total Number of Customers:
 ~~~
SELECT distinct count(*) AS total_customers 
from customers;
~~~

There are 38 unique customers

3.Top Customer Segments by Revenue

~~~
SELECT 
    customer_code,
    SUM(CASE
        WHEN t.currency = 'USD' THEN sales_amount * 87.4
        ELSE sales_amount
    END) AS total_sales,
    RANK() OVER (ORDER BY SUM(CASE 
        WHEN t.currency = 'USD' THEN sales_amount * 87.4
        ELSE sales_amount 
    END) DESC) AS sales_rank
FROM transactions
GROUP BY customer_code;

~~~
To  ranks customers based on their total sales.

4. Customer segmentation by types
~~~
SELECT customer_type, COUNT(*) AS customer_count
FROM customers
GROUP BY customer_type;
~~~
5.Top Customer Segments by Revenue
~~~
SELECT 
    customer_code,
    SUM(CASE
        WHEN t.currency = 'USD' THEN sales_amount * 83 
        ELSE sales_amount
    END) AS total_spent,
    CASE
        WHEN SUM(CASE 
            WHEN t.currency = 'USD' THEN sales_amount * 83 
            ELSE sales_amount 
        END) > 100000000 THEN 'High Value'
        WHEN SUM(CASE 
            WHEN t.currency = 'USD' THEN sales_amount * 83 
            ELSE sales_amount 
        END) BETWEEN 1000000 AND 100000000 THEN 'Medium Value'
        ELSE 'Low Value'
    END AS customer_segment,
    RANK() OVER (ORDER BY SUM(CASE 
        WHEN t.currency = 'USD' THEN sales_amount * 83 
        ELSE sales_amount 
    END) DESC) AS spending_rank
FROM transactions
GROUP BY customer_code
ORDER BY total_spent DESC;

   ~~~
To distribute customers into segments based on sales.

6. Sales Distribution by Customer Segment
~~~
SELECT 
    customer_segment,
    COUNT(customer_code) AS total_customers,
    SUM(total_spent) AS segment_revenue,
    (SUM(total_spent) * 100.0) / SUM(SUM(total_spent)) OVER () AS revenue_share
FROM (
    SELECT 
        customer_code,
        SUM(CASE
            WHEN t.currency = 'USD' THEN sales_amount * 87.4
            ELSE sales_amount
        END) AS total_spent,
        CASE 
            WHEN SUM(CASE 
                WHEN t.currency = 'USD' THEN sales_amount * 87.4
                ELSE sales_amount
            END) > 100000000 THEN 'High Value'
            WHEN SUM(CASE 
                WHEN t.currency = 'USD' THEN sales_amount * 87.4
                ELSE sales_amount
            END) BETWEEN 1000000 AND 100000000 THEN 'Medium Value'
            ELSE 'Low Value'
        END AS customer_segment
    FROM transactions
    GROUP BY customer_code
) AS customer_segments
GROUP BY customer_segment
ORDER BY segment_revenue DESC;

~~~
To find out which customer segment brings in the most revenue.



6.Sales Trend by Market Location
~~~
SELECT 
    m.markets_name, 
    SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) AS total_sales,
    RANK() OVER (ORDER BY SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) DESC) AS sales_rank,
    (SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) * 100.0) / SUM(SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END)) OVER () AS sales_share
FROM sales.transactions t
JOIN sales.markets m
ON m.markets_code = t.market_code
GROUP BY m.markets_name
ORDER BY total_sales DESC;
 
~~~

Identifies which market  performs the  best.

7.Sales Trend by Market Zones
~~~
SELECT 
    m.zone,
    SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) AS total_revenue,
    COUNT(DISTINCT t.customer_code) AS unique_customers,
    RANK() OVER (ORDER BY SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) DESC) AS revenue_rank,
    (SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END) * 100.0) / SUM(SUM(CASE 
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4 
        ELSE t.sales_amount 
    END)) OVER () AS revenue_share
FROM transactions t
JOIN markets m 
ON t.market_code = m.markets_code
GROUP BY m.zone
ORDER BY total_revenue DESC;

~~~

8.
~~~
SELECT 
    p.product_type,
    SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) AS total_sales,
    RANK() OVER (ORDER BY SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) DESC) AS sales_rank,
    (SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) * 100.0) / SUM(SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END)) OVER () AS sales_share
FROM sales.transactions t
JOIN sales.products p ON p.product_code = t.product_code
GROUP BY p.product_type
ORDER BY total_sales DESC;

~~~
9. Sales Trend by Product
 ~~~
SELECT 
    p.product_type,
    SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 83 
        ELSE t.sales_amount
    END) AS total_sales,
    RANK() OVER (ORDER BY SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 83 
        ELSE t.sales_amount
    END) DESC) AS sales_rank,
    (SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 83 
        ELSE t.sales_amount
    END) * 100.0) / SUM(SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 83 
        ELSE t.sales_amount
    END)) OVER () AS sales_share
FROM sales.transactions t
JOIN sales.products p ON p.product_code = t.product_code
GROUP BY p.product_type
ORDER BY total_sales DESC;

~~~
10
~~~
SELECT 
    d.year,
    d.month_name,
    SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) AS monthly_revenue,
    RANK() OVER (PARTITION BY d.year ORDER BY SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) DESC) AS revenue_rank,
    (SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END) * 100.0) / SUM(SUM(CASE
        WHEN t.currency = 'USD' THEN t.sales_amount * 87.4
        ELSE t.sales_amount
    END)) OVER (PARTITION BY d.year) AS monthly_revenue_share
FROM transactions t
INNER JOIN date d ON t.order_date = d.date
GROUP BY d.year, d.month_name, d.month
ORDER BY d.year, d.month;

~~~
