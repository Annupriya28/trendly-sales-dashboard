# Power BI Trendy Ecommerce Sales Dashboard

Trendly is an interactive Power BI dashboard designed to help e-commerce businesses analyze their sales performance, identify top-performing products, and understand customer segments. This project showcases real-world BI development using SQL data integration, DAX calculations, and visually rich Power BI reports.

---

# Objectives

-    Visualize sales performance over time (daily, weekly, monthly)
-    Highlight top-selling products by revenue and quantity
-    Segment customers based on demographics and behavior
-    Enable data-driven business decisions using KPIs and filters

---

# Architecture Overview

- Data Source : SQL Database (Sales, Products, Customers)
- Processing Layer : Power BI Data Model using DAX
- Visualization Layer : Power BI Dashboard

> Daily refresh enabled via Import Mode  
> Role-based access can be configured using Power BI RLS

---

# Dashboard Features

- Sales Trends (Line/Bar Charts)
- Top Products (Table or Bar)
- Customer Segments (Region, Age, Spending)
- KPIs: Total Sales, Avg Order Value, Customer Count
- Slicers for Date, Category, Segment

# DAX Measures

Total Sales = SUM(Sales[Amount])
Average Order Value = DIVIDE(SUM(Sales[Amount]), COUNTROWS(Sales))
Top Products = TOPN(10, Products, [Total Sales], DESC)


# GitHub Link
https://github.com/Annupriya28/trendly-sales-dashboard/blob/main/E-commerce.pbix
