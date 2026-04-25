# power_bi_dashboard_project
A collection of real-world data cleaning projects using MySql, MS Excel, Power Bi including missing value handling, outlier treatment, and data preprocessing.
# 🛍️ E-Commerce Orders Dashboard (Power BI)

An interactive Power BI dashboard for monitoring e-commerce sales performance across time, geography, product categories, and customer segments — with year-over-year growth tracking.

---

## 📊 Dashboard Overview

This Power BI report provides a single-page, fully interactive dashboard titled **"E-COMMERCE ORDERS DASHBOARD"**. It consolidates key sales metrics, trend lines, and breakdowns to give a comprehensive view of business performance.

![Dashboard Preview](dashboard_preview.png)
> *Add a screenshot of your dashboard here*

---

## 📁 File

| File | Description |
|------|-------------|
| `E-commerce_dashboard_1.pbix` | Power BI Desktop report file |

---

## 📈 KPIs & Metrics Tracked

The dashboard features the following KPI cards with current-period values and prior-year (PY) comparisons:

| KPI Card | Description |
|----------|-------------|
| **Total Sales** | Overall revenue with prior year reference |
| **Total Orders Sold** | Count of orders with prior year reference |
| **Total Quantity Sold** | Units sold with prior year reference |
| **Average Order Value (AOV)** | Average revenue per order |
| **Sales Growth KPI** | Year-over-year sales growth indicator |
| **Orders Growth KPI** | Year-over-year orders growth indicator |
| **Quantity Growth KPI** | Year-over-year quantity growth indicator |
| **AOV Growth KPI** | Year-over-year AOV growth indicator |

---

## 📉 Visuals & Charts

| Visual Type | What It Shows |
|-------------|---------------|
| **Line Chart** | Total Sales trend over time (by Year-Month) |
| **Line Chart** | Total Orders trend over time (by Year-Month) |
| **Line Chart** | Average Order Value trend (by Year-Month) |
| **Line Chart** | Max Quantity trend (by Year-Month) |
| **Clustered Bar Chart** | Sales / Orders / Quantity by category (with parameter toggle) |
| **Donut Chart** | Orders breakdown by Customer Segment |
| **Donut Chart** | Orders breakdown by Quarter |
| **Shape Map** | Total Sales by Country (world map) |
| **Table** | Country-level breakdown: Sales, Total Sales, Sales % |
| **Slicer** | Filter by Country |
| **Slicer** | Filter by Year |
| **Parameter Slicer** | Toggle metric displayed in bar chart |

---

## 🔢 Measures & Calculated Fields

The following DAX measures power the dashboard:

| Measure | Description |
|---------|-------------|
| `Total Sales` | Sum of revenue |
| `Total Orders` | Count of transactions |
| `Total Quantity Sold` | Sum of units sold |
| `Average Order Value` | Revenue ÷ Orders |
| `Sales PY` | Total Sales in the prior year |
| `Orders Sold PY` | Total Orders in the prior year |
| `Sales Year over Year Growth` | % change in sales vs. prior year |
| `Sales Growth KPI` | KPI indicator for sales growth |
| `Orders Growth KPI` | KPI indicator for orders growth |
| `Quantity Growth KPI` | KPI indicator for quantity growth |
| `AOV Growth KPI` | KPI indicator for AOV growth |
| `Max_Sales` / `Min_Sales` | Reference lines for sales chart |
| `Max_Orders` / `Min_Orders` | Reference lines for orders chart |
| `Max_AOV` / `Min_AOV` | Reference lines for AOV chart |
| `Max_Quantity` | Reference line for quantity chart |
| `Sales %` | Country's share of total sales |

---

## 🗂️ Data Fields Used

| Field | Description |
|-------|-------------|
| `country` | Customer's country |
| `customer_segment` | Customer segment/category |
| `category` | Product category |
| `Year-Month` | Time dimension for trend charts |
| `Year` | Year filter |
| `Quarter` | Quarter grouping |
| `Parameter` | Dynamic metric selector (Sales / Orders / Quantity) |

---

## 🌍 Geography

The dashboard includes a **world shape map** visualizing sales distribution across countries, with a country-level summary table showing each country's sales amount and percentage share.

---

## 🎨 Theme & Design

- Custom Power BI theme applied via `Power_BI_Theme_Generator` JSON
- Dark background (`#0B1215`) with accent color purple (`#8A2BE2`) and green (`#07D94D`) / red (`#F22525`) for growth indicators
- Smooth monotone line charts for trend visuals
- Rounded shapes for KPI card containers

---

## 🛠️ Tools & Requirements

| Tool | Version |
|------|---------|
| **Power BI Desktop** | March 2025 or later recommended |
| **Data Source** | Embedded in the `.pbix` file |

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open `E-commerce_dashboard_1.pbix` in **Power BI Desktop**.
3. Use the **Year** slicer to filter by a specific year.
4. Use the **Country** slicer to focus on a specific market.
5. Use the **Parameter** slicer to toggle the bar chart between Sales, Orders, and Quantity views.
6. Hover over any chart for detailed tooltips.
7. To publish: Go to **Home → Publish** and select your Power BI workspace.

> ⚠️ The data is embedded in the `.pbix` file. If you want to connect a live data source, go to **Home → Transform Data → Data Source Settings**.

---

## 📁 Repository Contents

```
📦 ecommerce-powerbi-dashboard
 ┣ 📊 E-commerce_dashboard_1.pbix
 ┗ 📄 README.md
```

---
## 📬 Contact

Feel free to open an issue or reach out if you have questions or suggestions!
