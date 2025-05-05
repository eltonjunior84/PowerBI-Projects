
# 📊 Sales Dashboard – Power BI Project

This project presents a dynamic **Sales Dashboard** developed in Power BI, aimed at analysing profitability, sales performance, and shipping behaviour across multiple markets.

## 🧾 Overview

The dashboard allows users to explore key business metrics interactively, with visual insights on:

- 💸 **Average Profit per Product Category**
- 🚚 **Total Sales by Shipping Method**
- 🧮 **KPI – Average Sales Value**
- 🌍 **Average Shipping Cost by Market** (EU, EMEA, US, LATAM, AFRICA, etc.)
- 📈 **Profit Margin Over Time**

Users can filter the data by **year** and **month** using slicers, allowing for temporal analysis of performance.

## 🔧 Data & ETL

The data model is built from **four separate `.csv` files**:

- `customers.csv`
- `products.csv`
- `orders.csv`
- `sales.csv`

> ⚠️ **Note**: The original dataset was provided in Portuguese and was transformed (column renaming and standardisation) for usability within this project.

Data preparation was done in Power Query, including:
- Data cleaning and type transformations
- Merging related tables
- Creating a date table for filtering and time-based analysis

## 📐 Key Metrics & DAX Measures

The following custom DAX calculations were created to support insights:

- **Profit**  
  `Profit = Sales[Order Total] - Sales[Shipping Cost]`

- **Profit Margin**  
  `Profit Margin = DIVIDE(Sales[Profit], Sales[Order Total]) * 100`

- **Average Sales Value** – displayed as a KPI card

## 📁 Files Included

- `Sales Dashboard.pbix` – Power BI dashboard file  
- `data/` folder – Contains the four `.csv` files used as data sources  
- `README.md` – This documentation

## 🚀 How to Use

1. Download or clone this repository
2. Open `Sales Dashboard.pbix` in Power BI Desktop
3. Explore the report using the filters and visuals

## 🎯 Purpose

This dashboard was built as part of a data analysis portfolio to demonstrate the use of Power BI in transforming raw sales data into actionable business insights through effective ETL, DAX calculations, and visual design.
