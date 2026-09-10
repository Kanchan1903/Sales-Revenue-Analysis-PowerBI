# Sales & Revenue Analysis | Power BI Dashboard

## 📊 Project Overview

This project is a Sales & Revenue Analysis dashboard built using Microsoft Power BI. The dashboard analyzes sales performance across products, countries, customer segments, and time periods.

The objective is to transform raw financial data into an interactive dashboard that helps identify key business trends, top-performing products, high-revenue markets, and major customer segments.

## 🎯 Objectives

- Analyze overall sales and revenue performance
- Track key performance indicators (KPIs)
- Identify revenue trends over time
- Compare revenue across countries and customer segments
- Identify the top-performing products
- Provide actionable business insights and recommendations
- Create an interactive dashboard using Power BI slicers

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query** – Data cleaning and transformation
- **DAX** – Calculated measures and KPI analysis
- **Microsoft Excel** – Source dataset

## 📁 Dataset

The project uses the **Financial Sample** dataset containing sales and financial information such as:

- Segment
- Country
- Product
- Units Sold
- Manufacturing Price
- Sale Price
- Gross Sales
- Discounts
- Sales
- COGS
- Profit
- Date
- Year
- Month

## 🔄 Data Preparation

The dataset was imported into Power BI and prepared using Power Query.

Key preparation steps included:

- Reviewing and cleaning column names
- Correcting data types
- Renaming the data table to `Financial_Data`
- Preparing date, month, and year fields for analysis
- Creating a clean data model for dashboard reporting

## 📐 DAX Measures

The following measures were created:

```DAX
Total Revenue = SUM(Financial_Data[Sales])

Total Units Sold = SUM(Financial_Data[Units Sold])

Total Profit = SUM(Financial_Data[Profit])

Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)
