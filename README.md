# Olist E-Commerce Data Analysis Project

## Project Overview
This project conducts an end-to-end analysis of the Brazilian Olist e-commerce dataset to generate actionable business insights regarding sales performance, customer behavior, seller efficiency, and delivery operations.

The project demonstrates a complete analytics workflow using Excel, Python, SQL, Power BI, Power Query, and DAX.

---

## Dataset
- Source: Brazilian E-Commerce Public Dataset by Olist [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce/data)
- Approx. 100,000 orders
- Multiple relational tables, including orders, customers, sellers, products, payments, reviews, and geolocation

---

## Business Objectives
- Analyze revenue and order trends
- Evaluate seller and product category performance
- Understand regional sales distribution
- Measure delivery performance and delays
- Analyze customer satisfaction using review scores
- Build interactive dashboards for business decision-making

---

## Tools and Technologies

- Excel – Initial data exploration and validation
- Python (Pandas, NumPy) – Data cleaning, transformation, and EDA
- SQL – Data modeling, joins, aggregations, analytical queries
- Power BI – Interactive dashboards and reporting
- Power Query – ETL and data transformation
- DAX – KPI creation and business calculations

---

## Data Modeling
A star schema was implemented in Power BI to support scalable reporting.

Fact Tables:
- Orders
- Order Items
- Payments

Dimension Tables:
- Customers
- Sellers
- Products
- Date
- Geography

---

## Key Metrics and KPIs
- Total Revenue
- Total Orders
- Average Order Value (AOV)
- Revenue by Region and State
- Revenue by Seller and Category
- On-Time vs Delayed Deliveries
- Average Delivery Time
- Customer Review Score
- Estimated Profit and Profit Margin

---

## Power BI Dashboards
The Power BI report includes:
- Sales Performance Overview
- Regional and Geographic Analysis
- Seller Performance Analysis
- Delivery and Logistics Analysis
- Customer Satisfaction Dashboard

Note: Due to file size limitations, the Power BI (.pbix) file is shared via an external link. Dashboard screenshots are included in the repository.

---

## Sample DAX Measures

Total Revenue =
SUMX(
    order_items,
    order_items[price] + order_items[freight_value]
)

Average Order Value =
DIVIDE(
    [Total Revenue],
    DISTINCTCOUNT(orders[order_id])
)

---

## SQL Analysis Performed
- Revenue and order trends by month
- Seller and category contribution analysis
- Regional sales performance
- Delivery delay analysis
- Customer review score correlation with delivery time

---

## Project Structure

olist-ecommerce-analysis/ data/#Raw and cleaned datasets|sql/#SQL queries and views|python/#Python notebooks for EDA|excel/#Excel analysis files|powerbi/#Power BI documentation and links|dashboards/#Dashboard screenshots──README.md

---

## Key Insights
- A small group of sellers contributes disproportionately to total revenue
- Delivery delays negatively impact customer review scores
- Some regions show high order volume but lower operational efficiency
- Certain categories generate high revenue but lower profitability

---

## Future Enhancements
- Incorporate actual cost data for accurate profit calculation
- Build sales forecasting models
- Perform customer segmentation (RFM analysis)
- Predict delivery delays using machine learning

---

## Author
Soumi Mukherjee  
Data Analyst 
![LinkedIN](www.linkedin.com/in/soumimukherjeeofficial)
![Email](soumi.mukherjee2003@gmail.com)

Skills: SQL, Python, Power BI, Excel, DAX, Power Query

## Screenshots / Demos
Overview: ![Dashboard Preview](https://github.com/soumimukherjee22/data-analysis-olist-e_commerce-analysis-python-sql-power-bi/blob/main/Olist_Overview.png)
Summary: ![Project Summary](https://github.com/soumimukherjee22/data-analysis-olist-e_commerce-analysis-python-sql-power-bi/blob/main/Olist%20Brazilian%20E-Commerce%20Dashboard%20Summary.jpg)
