
# 📊 Sales Data Analysis with Power BI

**Author:** Anuriya Ravindran  
**Batch:** DA-DS Reinforcement 
**Project:** Power BI Data Visualization  


---

## 📝 Introduction

This project leverages **Power BI** to clean, transform, and visualize transactional sales data to derive **actionable business insights**. Advanced **DAX functions** are used to calculate key metrics, and dynamic dashboards were created to explore performance trends, KPIs, and profitability across countries and products.

---

## 🎯 Project Objectives

- To analyze, transform, and visualize sales data using Power BI
- To apply **DAX functions** for computing custom KPIs
- To design **interactive dashboards** for real-time reporting and data exploration

---

## 📁 Dataset Overview

The dataset includes transactional data with the following key fields:

- `TransactionNo`: Unique ID for each transaction  
- `Date`: Transaction date  
- `ProductNo` / `ProductName`: Product identifiers  
- `Price`: Price per unit  
- `Quantity`: Units sold  
- `CustomerNo`: Unique customer ID  
- `Country`: Region where the sale occurred  

---

## 🔧 Data Cleaning & Transformation (Power Query Editor)

1. Imported data into Power BI  
2. Handled missing and null values  
3. Removed duplicate entries  
4. Corrected and validated data types for accuracy

---

## 🧮 DAX Calculations

Below are some DAX measures created for enhanced analytical capability:

```DAX
sum_of_totalsales = SUM ( 'Sales Transaction v 4a (2)'[total sales] )
Average Price = AVERAGE ( 'Sales Transaction v 4a (2)'[Price] )
Avg Revenue per Transaction = AVERAGE ( 'Sales Transaction v 4a (2)'[Total Sales] )
Gross Margin % = DIVIDE (
    SUM ('Sales Transaction v 4a (2)'[Price]), 
    SUM ('Sales Transaction v 4a (2)'[Total Sales]), 
    0
)
Unique Products Sold = DISTINCTCOUNT ( 'Sales Transaction v 4a (2)'[ProductNo] )


📈 Dashboard Features
KPI Cards: Total Sales, Average Revenue per Transaction, Gross Margin %

Bar and Line Charts: Country-wise and time-based sales trends

Map Visualization: Geographical distribution of total sales

Dynamic Filters: For date, region, and product

📊 Key Insights
💰 Total Sales: ₹60.28M across all countries

🌍 Top Revenue Countries: United Kingdom, Netherlands, Germany

🛍️ Premium Sales Regions: Sweden and Japan showed highest average revenue per transaction

📉 Profitability Concern: Gross Margin is only 0.11, indicating scope for cost optimization

📌 Visual Impact: Dashboard effectively communicates business trends and highlights revenue gaps

📝 Conclusion
This Power BI project provided an in-depth view into global sales performance, helping identify:

High-performing countries and products

Revenue vs. profitability mismatches

Opportunities to optimize margins and reduce costs

The interactive dashboard enables stakeholders to make data-driven decisions with ease.



This project is a part of my journey in mastering Data Visualization with Power BI under the Data Science & Analytics track.

“Transforming raw data into smart decisions, one dashboard at a time.”
