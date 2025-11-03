# 📊 Power BI Sales & Profit Dashboard  

## 📋 Project Overview  
This project presents an **interactive Power BI dashboard** designed to analyze **sales performance, profit margins, and year-over-year growth** across products, regions, and time.  
The goal was to turn raw transactional data into **clear, actionable insights** for business decision-making.

---

## 🎯 Objectives  
- Provide management with an overview of **total sales, profit, and margin trends**.  
- Identify **top-performing products and regions**, as well as underperforming areas.  
- Enable **dynamic filtering** and visual storytelling for better understanding of KPIs.  

---

## 🧩 Data Model  
The data model includes:  
- **Sales Table** – transactions with date, product, quantity, sales, and cost.  
- **Products Table** – product category and sub-category details.  
- **Date Table** – auto-generated calendar for time intelligence functions.  
- **Regions Table** – region and city data for geographical segmentation.  

Relationships were created to support DAX measures for time-based and category analysis.  

---

## 🧮 Key DAX Measures  
```DAX
Total Sales = SUM ( 'Sales'[SalesAmount] )
Total Cost  = SUM ( 'Sales'[Cost] )
Profit      = [Total Sales] - [Total Cost]
Profit Margin % = DIVIDE([Profit], [Total Sales])
YoY Sales   = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
```

---

## 🧠 Power Query Transformations  
- Imported and cleaned multiple CSV datasets.  
- Removed duplicates, fixed data types, and merged tables.  
- Created a Date table and ensured all fields were in a star schema.  
- Used parameters to control data loading and refresh options.  

---

## 📈 Dashboard Features  
- **KPI Cards:** Show total sales, profit, and margin %.  
- **Trend Analysis:** Line and column charts for sales and profit over time.  
- **Top Products & Categories:** Ranked by revenue and profitability.  
- **Regional Insights:** Bar chart comparing sales across regions.  
- **Slicers & Filters:** Interactivity for user-driven exploration.  
- **Navigation Bookmarks:** Smooth page transitions for presentation-style viewing.  

---

## 🎨 Design & Usability  
- Clean layout with consistent color palette and typography.  
- Visual hierarchy emphasizing KPIs and trends.  
- Tooltips and conditional formatting for better readability.  
- Focus on balance between analytics depth and visual clarity.  

---

## 🚀 Key Outcomes  
- Provided a full overview of sales and profit dynamics.  
- Reduced time for manual report preparation.  
- Improved understanding of which product lines contribute most to profitability.  
- Created a foundation for deeper RFM and forecasting analysis in future work.  

---

## 🧰 Tools & Technologies  
- **Power BI Desktop**  
- **Power Query**  
- **DAX**  
- **Excel / CSV data sources**

---

## 💡 What I Learned  
- Building a functional Power BI model from raw transactional data.  
- Applying DAX for KPIs and YoY comparisons.  
- Designing an intuitive analytical dashboard focused on business goals.  
- Enhancing presentation through user-friendly navigation and visuals.  

---

## 📸 Dashboard Preview

![Sales Dashboard](images/sales_dashboard.png)

---


> **Note:** This dashboard was built using Power BI’s sample dataset (“Financials”) available publicly within Power BI Desktop.  
> The dataset was used for learning and demonstration purposes only — all data are simulated.

---

📬 **Contact:**  
🔗 [LinkedIn — Olha Jarland](https://www.linkedin.com/in/olhajarland)  
💻 [GitHub — @olhajarland](https://github.com/olhajarland)
