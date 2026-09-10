Sales & Revenue Analysis | Power BI Dashboard
📊 Project Overview

This project is an interactive Sales & Revenue Analysis Dashboard developed using Microsoft Power BI.

The dashboard transforms financial sales data into meaningful business insights by analyzing revenue performance across time, countries, customer segments, and products.

🎯 Objectives
Track key sales and financial KPIs
Analyze revenue trends over time
Compare revenue across countries and customer segments
Identify top-performing products
Enable interactive analysis using slicers
Generate business insights and recommendations
🛠️ Tools & Technologies
Microsoft Power BI
Power Query – Data cleaning and transformation
DAX – KPI calculations and analysis
Microsoft Excel – Source dataset
📁 Dataset

The project uses the Financial Sample dataset containing information about:

Sales
Profit
Units Sold
Products
Countries
Customer Segments
Dates
Discounts
Cost of Goods Sold (COGS)
🔄 Data Preparation

The data was imported into Power BI and prepared using Power Query.

Key steps included:

Cleaning and renaming columns
Correcting data types
Preparing date, month, and year fields
Renaming the data table to Financial_Data
Preparing the dataset for analysis
📐 DAX Measures
Total Revenue

Total Revenue = SUM(Financial_Data[Sales])

Total Units Sold

Total Units Sold = SUM(Financial_Data[Units Sold])

Total Profit

Total Profit = SUM(Financial_Data[Profit])

Profit Margin

Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)

Revenue Growth

Revenue Growth % was calculated by comparing 2014 revenue with 2013 revenue.

📈 Dashboard Features

The dashboard includes:

Total Revenue KPI
Total Units Sold KPI
Total Profit KPI
Profit Margin KPI
Revenue Growth indicator
Revenue Trend analysis
Revenue by Country
Revenue by Customer Segment
Top 5 Products by Revenue
Interactive slicers for:
Year
Country
Segment
Product

🔍 Key Business Insights
Paseo is the top-performing product with approximately $33.01M in revenue.
The United States generated the highest revenue at approximately $25.03M.
The Government segment generated the highest revenue at approximately $52.50M.
Revenue increased significantly from 2013 to 2014.
Overall revenue was approximately $118.73M.
Overall profit was approximately $16.89M.
Overall profit margin was approximately 14.23%.

💡 Recommendations
Prioritize Paseo for inventory & marketing — $33.01M revenue.
Target Government with focused offerings — $52.50M revenue.

📸 Dashboard Preview
Overall Dashboard

Interactive Filtering

The dashboard includes interactive slicers that allow users to analyze the data by year, country, customer segment, and product.

📂 Project Files
Sales_Revenue_Analysis_Dashboard.pbix – Power BI dashboard
Financial Sample.xlsx – Source dataset
dashboard-overview.png – Final dashboard screenshot
dashboard-interactive-filter.png – Interactive filtering screenshot
README.md – Project documentation

🚀 Conclusion

This project demonstrates the use of Power BI, Power Query, and DAX to transform raw financial data into an interactive business intelligence dashboard.
The dashboard combines KPI tracking, trend analysis, product and segment comparisons, interactive filtering, business insights, and recommendations to support data-driven decision-making.
