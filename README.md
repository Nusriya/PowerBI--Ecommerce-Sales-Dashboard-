# eCommerce Sales Dashboard in Power BI

This project demonstrates the creation of an **eCommerce Sales Dashboard** in Power BI. The dashboard visualizes key performance metrics, including **Year-to-Date (YTD) Sales**, **YTD Profit**, and **YTD Quantity** 

## Project Overview

The goal of this project is to build an interactive dashboard that helps monitor and analyze eCommerce sales performance. Key features of the dashboard include:

1. **YTD Sales**: 
   - Displays the total sales amount year-to-date.

2. **YTD Profit**: 
   - Shows the total profit for the year so far.

3. **Top 5 Products by YTD Quantity**: 
   - Highlights the top 5 products based on the quantity sold year-to-date.

4. **Interactive Visualizations**:
   - Provides drill-down capabilities for users to explore specific metrics like product categories, regions, or sales channels.
   - Interactive slicers and filters for dynamic analysis.


## Steps to Reproduce the Dashboard

1. **Load the dataset into Power BI**:
   - Open Power BI Desktop and load the `ecommerce_sales_data.csv` file.
   - Transform the data (if necessary) to ensure correct formats for columns like `Order Date`, `Product Name`, and `Sales Amount`.

2. **Create YTD Calculations**:
   - Use DAX (Data Analysis Expressions) to calculate the Year-to-Date (YTD) values:
     - `YTD Sales = TOTALYTD(SUM('Sales'[Sales Amount]), 'Sales'[Order Date])`
     - `YTD Profit = TOTALYTD(SUM('Sales'[Profit]), 'Sales'[Order Date])`
     - `YTD Quantity = TOTALYTD(SUM('Sales'[Quantity]), 'Sales'[Order Date])`

3. **Visualize Key Metrics**:
   - Create visualizations for:
     - **YTD Sales**: Use a card visualization or bar chart.
     - **YTD Profit**: Use a card visualization or bar chart.
     - **Top 5 Products by YTD Quantity**: Create a bar chart with a filter to show the top 5 products.

4. **Design the Dashboard**:
   - Arrange the visualizations in a clean and interactive layout.
   - Add slicers for filtering by product category, region, or time period.
   - Include tooltips or drill-through capabilities to allow users to explore the data in more detail.

5. **Publish the Dashboard**:
   - Once the dashboard is ready, publish it to Power BI Service for sharing and collaboration (optional).



 
