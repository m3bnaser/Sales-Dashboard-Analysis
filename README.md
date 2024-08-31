# Sales Dashboard 📊

Welcome to the Sales Dashboard! This document provides an overview of the dashboard, insights gathered from the data, transformation processes, and explanations of key features and visuals. Whether you're a stakeholder, team member, or new user, this guide will help you understand and navigate the dashboard effectively.

## Overview 🌐

The Sales Dashboard is designed to provide comprehensive insights into sales performance across various territories and product lines. By transforming raw transaction data into a structured and interactive dashboard, users can easily analyze sales trends, identify top-performing regions and products, and make informed business decisions.

![image](https://github.com/user-attachments/assets/a40314a3-2da0-49bd-b6a7-0ad9e5b65b82)



## Source Data 🗂️

### Transaction Data

- **Format:** Excel File
- **Structure:** All transactions are consolidated into a single sheet.
- **Contents:** Each row represents a sales transaction, including details such as order ID, product, quantity, price, customer information, territory, and date.

## Data Transformation 🔄

To ensure efficient data analysis and reporting, the raw transaction data underwent a series of transformations using **Power Query** within **Power BI**. The transformation process involved:

1. **Cleaning:** Removing duplicates, handling missing values, and ensuring data consistency.
2. **Normalization:** Structuring data to eliminate redundancy and improve data integrity.
3. **Transformation:** Converting the flat transaction data into a star schema to facilitate easier analysis.

## Data Model 🗃️

The transformed data follows a **star schema**, which consists of a central fact table surrounded by dimension tables. This structure optimizes query performance and simplifies the reporting process.

![image](https://github.com/user-attachments/assets/fe03e813-9914-475b-af8c-bc32252ee917)


### Fact Table

- **FactSales:** Contains measurable, quantitative data related to sales transactions, such as sales amount, quantity sold, and total due.

### Dimension Tables

- **DimProduct:** Details about products, including product ID, name, category, and other attributes.
- **DimTerritory:** Data related to sales territories, including territory ID, name, and grouping information.
- **DimDate:** Date-related information to facilitate time-based analysis, including year, quarter, month, and day.
- **DimStatus:** Information about the status of orders such as approved, shipped, or canceled.
- **DimShip:** Data related to shipping methods, including method ID and name.

## Measures 📏

A dedicated **Measures** table was created to define all the necessary calculations used in the dashboard. These measures include:

- **Total Sales (Line Total):** Sum of sales amounts across all transactions.
- **Total Freight:** Sum of the freight costs for all orders.
- **Total Quantity Sold:** Sum of quantities sold.
- **Total Due:** Total amount due from all orders.
- **Top 3 Products:** Identifies the top three products based on sales within each territory.

## Dashboard Features & Insights 📈

The Sales Dashboard comprises various interactive visuals that provide a comprehensive view of sales performance. Below are the key features and insights derived from each visual and card.

### Key Metrics Cards

- **# Orders (1,465):** 📦 Total number of orders processed, indicating overall business volume.
- **# Order Details (23.6K):** 📝 Total number of line items, showing the breadth of products and transactions handled.
- **Total Freight ($915.97K):** 🚚 Total shipping costs associated with all orders, reflecting logistical expenses.
- **Total SubTotal ($30.1M):** 💰 The sum of all sales before taxes, a key indicator of revenue.
- **Total Due ($33.9M):** 💵 The total amount owed after taxes, including all financial commitments.
- **Total Tax ($2.9M):** 🏛️ The total tax collected from sales, important for compliance and reporting.

### Number of Orders by Status 📊

- **Insight:** **Approved Orders (396):** The highest number of orders, indicating strong customer demand and successful order processing.

### Orders by Territory Groups 🗺️

- **Insight:** **North America (56.31%):** Dominates with the largest share of orders, highlighting it as the top-performing region.

### Orders and Total Due by Territory 📊

- **Insight:** **Canada:** Generates the highest total due, making it the top revenue-generating territory.

### Total Order Quantity by Product Category 🛒

- **Insight:** **Bikes (28K):** The most popular product category, driving the highest volume of sales.

### Number of Orders by Date 📅

- **Insight:** **2013:** The peak year for orders, marking the highest point in sales performance over the years.

## Territory Tooltip 🗺️

One of the standout features of the dashboard is the **Territory Tooltip**, which enhances the interactivity and depth of the visuals related to territories.

### Orders and Total Due by Territory Visual

- **Number of Orders:** Displays the total number of orders placed in each territory.
- **Territory Group:** Categorizes territories into groups for better comparison.
- **Top 3 Products Ordered:** Highlights the top three products ordered within each territory, providing insights into regional product preferences.

**How It Works:**

- **Hover Interaction:** When users hover over a territory on the visual, the tooltip appears, showing detailed information such as the number of orders, territory group, and top 3 products.
- **Enhanced Insights:** This feature allows users to quickly grasp key metrics and product performance specific to each territory without cluttering the main visuals.

## Usage Instructions 🚀

1. **Opening the Dashboard:**
   - Access the Power BI file containing the Sales Dashboard.
   - Ensure that the Excel file with transaction data is available and correctly linked.

2. **Navigating the Dashboard:**
   - Use the slicers and filters to drill down into specific data segments.
   - Hover over visuals to access interactive tooltips and detailed information.
   - Click on specific data points to drill down into more granular details.

3. **Refreshing Data:**
   - To update the dashboard with the latest transaction data, go to the **Home** tab in Power BI and click **Refresh**.
   - Power BI will re-import and transform the latest data, updating all visuals accordingly.

## Contact Information 📞

For any questions, feedback, or support related to the Sales Dashboard, please contact:

- **Name:** Mohamed Abdelnaser
- **Email:** abonaser3401@gmail.com
- **Phone:** +20-1097734714
- **LinkedIn:** https://www.linkedin.com/in/3bnaser01
