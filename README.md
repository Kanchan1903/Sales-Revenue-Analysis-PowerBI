# Sales & Revenue Analysis | Power BI Dashboard

## 📊 Project Overview

This project is an interactive **Sales & Revenue Analysis Dashboard** developed using Microsoft Power BI.

The dashboard transforms financial sales data into meaningful business insights by analyzing revenue performance across time, countries, customer segments, and products.

## 🎯 Objectives

- Track key sales and financial KPIs
- Analyze revenue trends over time
- Compare revenue across countries and customer segments
- Identify top-performing products
- Enable interactive analysis using slicers
- Generate business insights and recommendations

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query** – Data cleaning and transformation
- **DAX** – KPI calculations and analysis
- **Microsoft Excel** – Source dataset

## 📁 Dataset

The project uses the **Financial Sample** dataset containing information about:

- Sales
- Profit
- Units Sold
- Products
- Countries
- Customer Segments
- Dates
- Discounts
- Cost of Goods Sold (COGS)

## 🔄 Data Preparation

The data was imported into Power BI and prepared using Power Query.

Key steps included:

- Cleaning and renaming columns
- Correcting data types
- Preparing date, month, and year fields
- Renaming the data table to `Financial_Data`
- Preparing the dataset for analysis

## 📐 DAX Measures

### Total Revenue

```DAX
Total Revenue = SUM(Financial_Data[Sales])
Total Units Sold = SUM(Financial_Data[Units Sold])
Total Profit = SUM(Financial_Data[Profit])
Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)
Revenue Growth % =
VAR Revenue2013 =
    CALCULATE(
        [Total Revenue],
        Financial_Data[Year] = 2013
    )
VAR Revenue2014 =
    CALCULATE(
        [Total Revenue],
        Financial_Data[Year] = 2014
    )
RETURN
    DIVIDE(Revenue2014 - Revenue2013, Revenue2013)
