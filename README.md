# ecommerce-sales-customer-product-analytics-powerbi

## Project Overview

This project presents an end-to-end **Power BI analytics solution** for an e-commerce business.

The objective of the project is to analyze sales performance, customer behavior, product demand, order and payment patterns, and customer retention. The analysis transforms raw transactional data into interactive dashboards and business insights that can support management decision-making.

## Business Objectives

- Analyze sales performance and revenue trends.
- Understand customer behavior and purchasing patterns.
- Identify high-performing and low-performing products and categories.
- Analyze order status and payment patterns.
- Identify repeat and high-value customers.
- Monitor product stock levels and low-stock products.
- Identify business issues and growth opportunities.
- Provide data-driven recommendations for management.

## Dataset

The project uses four main business tables:

| Table | Records | Description |
|---|---:|---|
| Customers | 100 | Customer details and registration information |
| Products | 50 | Product, category, price, and stock information |
| Orders | 500 | Order dates, status, and payment information |
| Order Items | 1,500 | Products and quantities included in each order |

A dedicated **DateTable** was created in Power BI for date filtering, monthly analysis, and time-intelligence calculations.

A disconnected **Customer Type** helper table was also created for customer segmentation analysis.

## Data Preparation & Quality Checks

The data was validated and prepared before dashboard development.

Key checks included:

- Data type validation.
- Duplicate record checks.
- Missing value checks.
- Unique ID validation.
- Customer and product ID relationship validation.
- Product price and order-item unit price validation.
- Product stock and quantity validation.
- Order date validation.

During validation, the following data-quality issues were identified:

- 115 orders had order dates earlier than the related customer signup dates.
- 26 orders did not have corresponding Order Item records.
- 1 customer had no associated orders.

These records were retained for analysis and further investigation rather than being arbitrarily deleted or modified.

## Data Model

The Power BI data model contains relationships between:

- Customers → Orders
- Orders → Order Items
- Products → Order Items
- DateTable → Orders

The DateTable was created to support consistent date-based analysis and time intelligence.

## Data Transformation

The following transformations and calculations were performed:

- Standardized and validated data types.
- Validated categorical values.
- Created an **Order Value** calculated column.
- Created a dedicated **DateTable**.
- Created Year, Month, and Month Number fields.
- Created DAX measures for business KPIs and analysis.

## Key DAX Measures

Some of the major measures created include:

- Total Revenue
- Total Orders
- Average Order Value
- Total Quantity Sold
- Revenue Growth %
- Total Customers
- New Customers
- Repeat Customers
- Repeat Rate %
- Average Revenue per Customer
- Orders per Customer
- Delivered Orders
- Cancelled Orders
- Cancellation Rate %
- Delivery Rate %
- Top Product by Revenue
- Top Category by Revenue

## Dashboard Pages

### 1. Sales Performance

Analyzes:

- Revenue
- Orders
- Average Order Value
- Revenue trends
- Category performance
- Product performance
- City performance
- Revenue growth
- Order status
- Payment methods

### 2. Customer Analysis

Analyzes:

- Total customers
- New customers
- Repeat customers
- Customer registrations
- Customer distribution by city
- Customer revenue
- Top customers
- Repeat vs one-time customers

### 3. Product & Category Analysis

Analyzes:

- Revenue by category
- Top products by revenue
- Top and bottom products by quantity sold
- Average Order Value by category
- Product price vs quantity sold
- Product stock levels
- Low-stock products

### 4. Orders & Payment Analysis

Analyzes:

- Total orders
- Delivered orders
- Cancelled orders
- Cancellation rate
- Orders by payment method
- Revenue by payment method
- Cancellation rate by payment method
- Order status trends
- Cancellation patterns by city

### 5. Customer Value & Retention

Analyzes:

- Repeat customer rate
- Average revenue per customer
- Orders per customer
- Customer segments
- High-value customers
- Customer purchasing frequency
- Revenue contribution by customer type

### 6. Executive Summary

Provides management-level KPIs, key business insights, and recommendations in a single view.

## Key Business Insights

- Total revenue reached approximately **₹116.15M** across **500 orders**.
- **Electronics** generated the highest revenue among the categories.
- **Repeat customers account for 95% of the customer base**.
- Average revenue per customer is approximately **₹1.16M**.
- Overall cancellation rate is **10.60%**.
- A small group of customers contributes a significant share of total revenue.
- Several products require monitoring because of low stock levels.
- Payment method and city-level cancellation patterns provide opportunities for operational improvement.

## Business Recommendations

- Focus on retaining repeat and high-value customers through targeted offers and loyalty initiatives.
- Monitor cancellation patterns by payment method and city to identify operational issues.
- Maintain appropriate inventory levels for low-stock products.
- Review low-performing products for pricing and demand-related issues.
- Support high-revenue categories with appropriate inventory and promotional strategies.
- Continue engaging high-value customers to sustain their revenue contribution.

## Tools & Technologies

- **Power BI**
- **Power Query**
- **DAX**
- **Data Modeling**
- **Data Visualization**
- **Excel / CSV-based transactional data**

## Project Workflow

The project followed an end-to-end analytics workflow:

**Business Understanding → Data Understanding → Data Validation → Data Cleaning → Data Modeling → KPI Definition → DAX → Dashboard Development → Business Insights → Recommendations**

## Repository Contents

This repository contains:

- Power BI `.pbix` project file
- Project documentation
- Dashboard screenshots
- Data model / ER diagram
- Supporting project materials

## Project Outcome

The project demonstrates how raw e-commerce transactional data can be transformed into an interactive Power BI reporting solution that helps management understand sales, customers, products, orders, payments, and customer retention.


## Project Documentation & Dashboard Screenshots

### Project Documentation



### Dashboard Screenshots

#### Sales Performance


#### Customer Analysis


#### Product & Category Analysis


#### Orders & Payment Analysis


#### Customer Value & Retention


#### Executive Summary

---

## Author

**Bhavani Bollepelli**

Data Science | Data Analytics | Power BI | SQL | Python

### Connect with me

- LinkedIn: https://www.linkedin.com/in/bhavani-bollepelli-1a7ba0422/
- GitHub: https://github.com/bhavani-bollepelli
