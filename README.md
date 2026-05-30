📊 Task 4 – Advanced Business Intelligence Dashboard
📌 Project Overview

This project was completed as part of a Data Analytics & Business Intelligence Internship. The objective was to build an advanced Business Intelligence solution using Excel, PostgreSQL, Power BI, and DAX to analyze retail sales data and generate actionable business insights.

The project focuses on data modeling, KPI development, time intelligence calculations, dashboard creation, and executive-level business reporting.

🎯 Project Objectives
Build a professional Power BI data model using a Star Schema.
Create relationships between fact and dimension tables.
Implement DAX measures for KPI calculations.
Perform time intelligence analysis using a Calendar table.
Design an interactive executive dashboard.
Generate business recommendations from data insights.
🛠️ Tools & Technologies Used
Microsoft Excel
Data cleaning and preparation
Data validation
Preliminary analysis
PostgreSQL
Data import and transformation
SQL querying and aggregation
Business analysis using SQL
Power BI
Data modeling
Interactive dashboard development
KPI visualization
Slicers and filters
DAX (Data Analysis Expressions)
KPI calculations
Profit Margin analysis
Time Intelligence calculations
Growth analysis
📂 Data Model
Fact Table

Orders Table

Order_ID
Order_Date
Customer_ID
Product_ID
Sales
Quantity
Profit
Discount
Dimension Tables

Customers

Customer_ID
Customer_Name
Region
Segment

Products

Product_ID
Product_Name
Product_Category

Calendar

Date
Year
Month Name
Month Number
🔗 Data Modeling

Implemented a Star Schema Model:

Calendar → Orders
Customers → Orders
Products → Orders

Relationship Type:

One-to-Many (1:*)
📈 DAX Measures Created
Core Measures
Total Sales = SUM(Orders[Sales])

Total Profit = SUM(Orders[Profit])

Profit Margin = DIVIDE([Total Profit],[Total Sales],0)
Time Intelligence Measures
Previous Month Sales =
CALCULATE(
    [Total Sales],
    PREVIOUSMONTH(Calendar[Date])
)

Growth % =
DIVIDE(
    [Total Sales]-[Previous Month Sales],
    [Previous Month Sales],
    0
)
📊 Dashboard Features
KPI Cards
Total Sales
Total Profit
Profit Margin
Previous Month Sales
Total Orders
Visualizations
Monthly Sales Trend
Profit by Product Category
Sales by Region
Sales by Customer Segment
Top Customers Analysis
Interactive Filters
Year Filter
Month Filter
Region Filter
Product Category Filter
Segment Filter
🔍 Key Business Insights
Strong overall sales and profitability performance.
Consumer segment contributes the highest share of revenue.
Certain product categories generate significantly higher profits.
Regional sales performance varies across locations.
Monthly sales trends reveal seasonal demand patterns.
💡 Business Recommendations
Revenue Growth
Expand high-performing product categories.
Improve performance in lower-performing regions.
Strengthen customer acquisition efforts.
Profit Optimization
Focus on high-margin products.
Optimize pricing strategies.
Monitor category-wise profitability.
Customer Strategy
Improve customer retention initiatives.
Increase personalized marketing campaigns.
Develop stronger relationships with key customer segments.
Operational Improvements
Improve demand forecasting.
Optimize inventory planning.
Continuously monitor KPIs using dashboards.
📁 Repository Contents
Cleaned Dataset Files
SQL Scripts
Power BI Dashboard (.pbix)
Dashboard Screenshots
Business Insight Report
Project Documentation
🚀 Learning Outcomes

Through this project, I gained practical experience in:

Business Intelligence Development
Data Modeling
DAX Calculations
Time Intelligence Analysis
Dashboard Design
KPI Development
Data Storytelling
Business Insight Generation
👨‍💻 Author

Abhradeep Auddy
Data Analytics & Business Intelligence Intern
