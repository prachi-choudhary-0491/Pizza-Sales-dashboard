🍕 Pizza Sales Analysis Dashboard (SQL + Power BI)
Overview

This project is a complete walkthrough of how I built an end-to-end data analytics project using MS SQL Server and Power BI.
It covers everything from importing raw data, cleaning and validating it with SQL, to building an interactive sales dashboard in Power BI.

The main goal was to analyze the performance of a pizza business and understand sales patterns, customer behavior, and revenue trends.

**Objectives**

    Import and organize sales data in SQL Server
    Clean and transform the data for better analysis
    Validate Power BI results with SQL queries
    Build a dynamic Power BI dashboard showing key business metrics

**Tools & Technologies**

    MS SQL Server for database setup and querying
    SQL (joins, group by, aggregates, cast, date functions)
    Power BI for data visualization
    Power Query and DAX for transformations and calculations
    CSV files as the primary data source

**SQL Work**

I started by creating a new database in SQL Server and importing the CSV file.
After checking data types and missing values, I wrote queries to calculate key metrics such as:

    Total Revenue: SUM(total_price)
    Average Order Value: SUM(total_price) / COUNT(DISTINCT order_id)
    Category-wise Sales: Using GROUP BY pizza_category
    Monthly Sales Trends: Using DATENAME(MONTH, order_date)
    Top and Bottom Selling Pizzas: Using ORDER BY and LIMIT
    I also used the CAST() function to convert values into decimals for accurate financial reporting.

**Power BI Work**

After validating the SQL results, I imported the same data into Power BI and created visuals to represent insights clearly.
The dashboard includes:

    KPI cards for Total Revenue, Average Order Value, Total Orders, and Pizzas per Order
    Line chart for monthly sales trends
    Funnel chart showing sales by pizza category
    Conditional formatting for highlighting top and bottom performers
    Slicers to filter by category, month, and pizza type
    I also added navigation buttons and basic formatting to make the dashboard more interactive and easy to use.
