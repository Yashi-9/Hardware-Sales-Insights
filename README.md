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
from customers;Top Customer Segments by Revenue
~~~

There are 38 unique customers

3.Top Customer Segments by Revenue

~~~
SELECT 
customer_code,
SUM(sales_amount) AS total_sales,
RANK() OVER (ORDER BY SUM(sales_amount) DESC) AS sales_rank
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
SUM(sales_amount) AS total_spent,
CASE
        WHEN SUM(sales_amount) > 100000000 THEN 'High Value'
        WHEN SUM(sales_amount) BETWEEN 1000000 AND 100000000 THEN 'Medium Value'
        ELSE 'Low Value'
END AS customer_segment
FROM transactions
GROUP BY customer_code
ORDER BY total_spent DESC;
   ~~~
To identify which segment contributes most to revenue.                                            

6. Sales Distribution by Customer Segment
~~~
SELECT 
    customer_segment,
    COUNT(customer_code) AS total_customers,
    SUM(total_spent) AS segment_revenue,
    (SUM(total_spent) * 100) / (SELECT SUM(sales_amount) FROM transactions) AS revenue_share
FROM (
    SELECT 
        customer_code,
        SUM(sales_amount) AS total_spent,
        CASE 
            WHEN SUM(sales_amount) > 100000000 THEN 'High Value'
            WHEN SUM(sales_amount) BETWEEN 1000000 AND 100000000 THEN 'Medium Value'
            ELSE 'Low Value'
        END AS customer_segment
    FROM transactions
    GROUP BY customer_code
) AS customer_segments
GROUP BY customer_segment;
~~~
To find out which segment brings in the most revenue.



6.Sales Trend by Market Location
~~~
SELECT markets_name, sum(sales_amount) AS sales_amount
FROM sales.transactions t
JOIN sales.markets m
ON m.markets_code = t.market_code
GROUP BY market_code
ORDER BY sales_amount DESC; 
~~~

Identifies which market  performs the  best.

7.Sales Trend by Market Zones
~~~
SELECT 
    markets.zone,
    SUM(transactions.sales_amount) AS total_revenue,
    COUNT(DISTINCT transactions.customer_code) AS unique_customers
FROM transactions
join markets 
on transactions.market_code=markets.markets_code
GROUP BY markets.zone
ORDER BY total_revenue DESC;
~~~

8.
~~~
SELECT product_type,
    SUM(CASE
        WHEN t.currency = 'USD' THEN sales_amount * 83 
        ELSE sales_amount
    END) AS sales_amount
FROM sales.transactions t
JOIN sales.products p ON p.product_code = t.product_code
GROUP BY product_type
ORDER BY sales_amount DESC;
~~~
9. Sales Trend by Product
 ~~~
 SELECT product_type,
 SUM(CASE
        WHEN t.currency = 'USD' THEN sales_amount * 83 
        ELSE sales_amount
    END) AS sales_amount
FROM sales.transactions t
JOIN sales.products p ON p.product_code = t.product_code
GROUP BY product_type
ORDER BY sales_amount DESC;
~~~
10
~~~
SELECT 
    date.year,
    date.month_name,
    SUM(transactions.sales_amount) AS monthly_revenue
FROM transactions
INNER JOIN date ON transactions.order_date = date.date
GROUP BY date.year, date.month_name
ORDER BY date.year, date.month;
~~~
