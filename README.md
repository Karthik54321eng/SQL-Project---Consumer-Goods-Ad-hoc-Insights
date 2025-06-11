
I recently completed a hands-on SQL challenge from Codebasics focused on real-world business scenarios in the consumer goods sector.
Challenge Link : 

 🏭a)AtliQ Hardware :

AtliQ Hardware is a rapidly growing global tech company that offers a wide range of high-quality hardware products — including desktops, laptops, mice, and storage devices — in Standard, Plus, and Premium variants. As the business expands, the leadership team is increasingly dependent on timely, data-driven decisions.

However, due to limitations in their existing data systems, deriving actionable insights has become a challenge. To address this, the analytics team was tasked with solving 10 specific business questions to provide clarity on key performance metrics.

💻b)Video Presentation:

🗒️c)PDF File :

📌d)Objective :

1)To analyze Atliq Hardware's customers and products, along with their respective sales quantities & gross sales across various regions.
2)This project focuses on answering those 10 ad-hoc business questions using structured data from the company's database. 
3)The goal is to deliver clear, actionable insights to support executive planning and strategic decision-making.

🛠️e)Tools :

1)SQL (MySQL) – For data exploration and transformation
2)DBMS – MySQL Workbench for querying and managing data
3)Power BI - To create charts & visuals.
4)Canva - For Making Presentation.
5)Veed - For Video Editing.

🗃️f)Database Overview :

The data is stored in a MySQL database named gdb023 (also referred to as atliq_hardware_db). It includes the following six key tables:

1. dim_customer
customer_code: Unique identifier for each customer.
customer: Name of the customer (e.g., Flipkart, Surface Stores).
platform: Sales channel (e.g., E-Commerce, Brick & Mortar).
channel: Type of distribution (e.g., Retailers, Direct, Distributors).
market: Country where the customer is located.
region: Geographic region (APAC, EU, NA, LATAM).
sub_zone: Sub-region such as India, ANZ, SE, NE.

2. dim_product
product_code: Unique identifier for each product.
division: Product group (e.g., P & A, N & S, PC).
segment: Product segment (e.g., Notebook, Desktop, Storage).
category: Specific category within a segment.
product: Product name.
variant: Product version (Standard, Plus, Premium).

3. fact_gross_price
product_code: Matches with dim_product.
fiscal_year: The fiscal year (starts in September; available data: 2020–2021).
gross_price: Initial price before discounts or taxes.

4. fact_manufacturing_cost
product_code: Product identifier.
cost_year: Fiscal year of manufacturing.
manufacturing_cost: Cost to produce the product (materials, labor, overhead).

5. fact_pre_invoice_deductions
customer_code: Matches with dim_customer.
fiscal_year: Year of the transaction.
pre_invoice_discount_pct: Discount applied before invoice generation.

6. fact_sales_monthly
date: Monthly date of sale.
product_code: Matches with dim_product.
customer_code: Matches with dim_customer.
sold_quantity: Number of units sold.
fiscal_year: Fiscal year of the sale.

🖥️g)Presentation contains:

1)About Atliq Company,
2)Problem Statement,
3)SQL Queries & Output
4)Insights.


🔍h)Insights :

1)Highest sales - 20.46M(Nov-2020),Lowest Sales - 0.77M(Mar-2020). 
2)The sold quantity in Q1 FY 2021 was nearly double that of Q1 FY 2020. 
3)Retailers like Amazon, Flipkart contributed the highest gross sales (73%), followed by direct and distributor channels.
4)In FY 2020, there are a total of 245 products, but in FY 2021, product count increased by 36% to 334 products. 
5)Notebook,Peripherals & Accessories contribute to 80% of total products.
6)In 2021,company offered nearly equal pre-invoice discount percentages to each of top 5 customers,given that Flipkart is the most discounted customer in the Indian market, which equals 30.83%.
7)The sold quantity decreased to 2.1M in Q3 of FY 2020, which was actually March, April,May when COVID-19 was at its peak.
 Recovery Phase Q4 - Online Mode.
8)The top 3 selling products in PC were personal laptops, which were around 25000 in quantity.
9)The top 3 selling products in P&A were mouse, which were around 6 lakh in quantity.
10)The top 3 selling products in PC were personal laptops, which were around 25000 in quantity.
