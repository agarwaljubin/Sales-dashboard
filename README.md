# ⚡ Electro-Hub Sales Analysis — Power BI Dashboard

> An end-to-end business intelligence solution built in Power BI, transforming raw retail transaction data into actionable sales insights for Electro-Hub — covering profitability, order trends, discount performance, and product-level analysis across Indian cities.

---

## 📊 Dashboard Preview

![Electro-Hub Sales Dashboard](Dashboard__Sales_annalysis.png)

---

## 📁 Data Source

- **Type:** Internal retail transaction data (structured tabular data)
- **Format:** Imported and modeled within Power BI Desktop (`.pbix`)
- **Coverage:** Sales records from **2020 to 2024**, spanning multiple Indian cities
- **Key fields:** Customer ID, Order ID, Order Date, Product, City, Net Sales, Discount, Discount Percentage, Profit, Quantity

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Data modeling, DAX, and dashboard development |
| **Power Query (M Language)** | Data profiling, cleaning & transformation |
| **DAX (Data Analysis Expressions)** | Custom measures, KPIs, and calculated columns |
| **Star Schema Modeling** | Relational data structure design |
| **TomTom / OpenStreetMap** | Geo-visual map rendering within Power BI |

---

## ✨ Features & Highlights

### 🔍 Business Requirements Analysis
- Identified key business questions around profitability, discount effectiveness, product performance, and regional sales trends before building any visuals
- Structured the project around stakeholder-relevant KPIs

### 🧹 Data Profiling & Transformation (Power Query)
- Performed thorough **data profiling** — checked column quality, distribution, and value errors
- Cleaned nulls, corrected data types, standardized date formats (`dd/mm/yyyy`)
- Removed duplicates and irrelevant columns to streamline the model

### 🗂️ Star Schema Design
- Designed a proper **Star Schema** with a central Fact Table (Sales/Orders) and surrounding Dimension Tables (Customers, Products, Dates, Cities, Promotions)
- Defined **cardinality** for all relationships (one-to-many) to ensure accurate filter propagation across the model

### 📐 DAX Measures & Calculations
Created custom DAX measures including:
- `Profit 1` & `Profit 2` — dual profit comparisons for period-over-period analysis
- `Qnty1` & `Qnty2` — quantity sold comparisons across segments
- `Total Net Sales`, `Sum of Discount Percentage` — aggregated KPIs
- **Time intelligence functions** for year-over-year sales trend analysis
- Filters using `CALCULATE()` with `FILTER()` to scope measures to specific contexts (e.g., promotions, cities, product categories)

### 📈 Dashboard Visuals
| Visual | Insight |
|--------|---------|
| **Map — Sales by City** | Geographic spread of orders across India (Delhi, Mumbai, Chennai, Hyderabad, etc.) |
| **KPI Card** | 3,510 total number of orders |
| **Bar Chart — Avg Discount by Promotion** | Weekend Flash Sale (23K) leads, followed by Clearance Sale (18K) |
| **Line Chart — Sales Trend (2020–2024)** | Peak sales reaching 0.65M; seasonal fluctuations visible |
| **Bar Chart — Bottom 5 Products by Profit** | Tupperware Lunch Box, L'Oreal Shampoo flagged as underperformers |
| **Scatter Plot — Profit vs Net Sales** | Strong positive correlation; outliers identified |
| **Stacked Bar — Total Profit** | ~12.2M combined across Profit 1 & Profit 2 |
| **Stacked Bar — Total Quantity Sold** | 7.1K each across Qnty1 & Qnty2 |
| **Data Table** | Granular transaction-level view with Customer ID, Order ID, Date, Discount & Net Sales |

### 🔗 Filters & Interactivity
- Applied **cross-filtering** across all visuals for interactive drill-down
- Used **slicers** and **visual-level, page-level, and report-level filters** to control context
- Enabled dynamic highlighting between the scatter plot, bar charts, and map

---

## 📌 Key Business Insights

- **Weekend Flash Sale** offers the highest average discount — worth reviewing for margin impact
- **Tupperware Lunch Box** and **L'Oreal Shampoo** are bottom performers by profit — candidates for discontinuation or repricing
- **Sales peaked in 2022–2023**, with a visible dip afterward suggesting a need for demand analysis
- **Profit and Net Sales** are strongly correlated, but some high-sales products show lower profit — potential pricing or cost issues

---

## 🚀 How to Open

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone or download this repository
3. Open `Electro-Hub__Sales_annalysis.pbix` in Power BI Desktop
4. Explore the dashboard and interact with the filters

---

## 👤 Author

**[Jubin Agarwal]**  
Aspiring Data Analyst | Power BI | SQL | DAX  
[LinkedIn]](https://www.linkedin.com/in/jubin-agrawal/)) • [GitHub](https://github.com/agarwaljubin)

---

> *Built as a personal portfolio project to demonstrate end-to-end Power BI development — from raw data to business-ready insights.*
