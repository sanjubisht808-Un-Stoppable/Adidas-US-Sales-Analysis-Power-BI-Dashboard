# 👟 Adidas US Sales Analysis | Power BI Dashboard

An interactive Power BI dashboard that analyses two years of Adidas sales across the United States. It tracks the key business KPIs, surfaces seasonal patterns, and compares performance by region, state, retailer, product and sales channel, so stakeholders can make faster, data-backed decisions.

![Dashboard Preview](dashboard_preview.png)
<!-- Add a screenshot of your dashboard at images/dashboard_preview.png -->

---

## 📌 Table of Contents
- [Business Problem](#-business-problem)
- [Dataset](#-dataset)
- [KPIs](#-kpis)
- [Dashboard Features](#-dashboard-features)
- [Key Insights](#-key-insights)
- [Tools & Skills Used](#-tools--skills-used)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 🎯 Business Problem

Adidas sells through multiple retailers, regions and channels, but leadership lacks a single view of how the business is performing. The business needed an interactive dashboard that lets stakeholders:

- Monitor overall sales, profit, units sold, average selling price and profit margin
- Analyse monthly sales trends to spot seasonal patterns
- Compare performance across regions and states
- Evaluate the contribution of each retailer and product category
- Filter the data by region, sales method and invoice date
- Identify top-performing products and retailers to support strategic planning

---

## 🗂 Dataset

**File:** `Adidas_US_Sales_Datasets.xlsx` (sheet: `Data Sales Adidas`)

| Detail | Value |
|---|---|
| Records | 9,648 transactions (after removing 4 blank rows) |
| Time period | 1 Jan 2020 – 31 Dec 2021 |
| Retailers | 6 (Foot Locker, West Gear, Sports Direct, Kohl's, Amazon, Walmart) |
| Regions | 5 (West, Northeast, Southeast, South, Midwest) |
| Coverage | 50 states, 52 cities |
| Products | 6 categories (Men's / Women's × Street Footwear, Athletic Footwear, Apparel) |
| Sales methods | In-store, Online, Outlet |

**Columns:** `Retailer`, `Retailer ID`, `Invoice Date`, `Region`, `State`, `City`, `Product`, `Price per Unit`, `Units Sold`, `Operating Profit`, `Operating Margin`, `Sales Method`

---

## 📊 KPIs

| KPI | Definition |
|---|---|
| **Total Sales** | Total revenue generated (Price per Unit × Units Sold) |
| **Total Profit** | Sum of Operating Profit |
| **Total Units Sold** | Sum of units sold |
| **Average Price per Unit** | Average selling price across products |
| **Average Profit Margin (%)** | Percentage profit earned on sales |

---

## 🖥 Dashboard Features

**Visuals**
- **Monthly Sales Trend** (area chart): seasonal patterns over time
- **Sales by State** (shape map): geographical distribution across the US
- **Sales by Region** (donut chart): regional revenue contribution
- **Sales by Product** (bar chart): best-selling product categories
- **Sales by Retailer** (bar chart): retailer performance
- **KPI cards**: Total Sales, Total Profit, Units Sold, Avg Price, Avg Profit Margin

**Interactivity**
- Sales Method slicer (In-store / Online / Outlet)
- Month slicer and Year slicer
- Cross-filtering between all visuals

---

## 💡 Key Insights

> Figures below are calculated from the dataset (Sales = Price per Unit × Units Sold).

- **Total sales of about $899.9M** and **operating profit of about $332.1M** from **17.9M units** sold over 2020–2021, an overall profit margin of roughly **36.9%**.
- **West is the strongest region**, contributing about $269.7M, well ahead of Northeast (about $186.3M). Midwest is the lowest at about $135.8M.
- **West Gear and Foot Locker are the top retailers**, together generating over half of total sales. Walmart and Amazon sit at the bottom.
- **Men's Street Footwear is the best-selling product** (about $208.8M), followed by Women's Apparel (about $179.0M). Women's Athletic Footwear sells the least.
- **In-store is the largest sales channel** by revenue (about $356.6M), followed by Outlet (about $295.6M) and Online (about $247.7M), even though Online has the most transactions.
- **Top states are New York, California and Florida**, each above $59M.
- **Peak months are July 2021 and December 2021**, pointing to mid-year and holiday-season demand.

---

## 🛠 Tools & Skills Used

- **Power BI Desktop**: data modelling, DAX measures, interactive visuals
- **Power Query**: data cleaning and transformation
- **DAX**: calculated measures (`Total Sale`, `Total_Profit`) and the `Month Wise` column
- **Excel**: source data
- **Skills demonstrated:** KPI design, dashboard layout and UX, data storytelling, business-driven analysis

---

## 📁 Project Structure

```
Adidas-US-Sales-Analysis/
│
├── Adidas_US_Sales_Datasets.xlsx          # Raw dataset
├── First_Project.pbix                      # Power BI dashboard file
├── Adidas_Analysis_Problem_Statement.pptx  # Business requirements & KPIs
├── images/
│   └── dashboard_preview.png               # Dashboard screenshot
└── README.md
```

---

## 🚀 How to Use

1. Clone this repository
   ```bash
   git clone https://github.com/<your-username>/Adidas-US-Sales-Analysis.git
   ```
2. Open `First_Project.pbix` in **Power BI Desktop** (free to download from Microsoft).
3. If prompted, update the data source path to point to `Adidas_US_Sales_Datasets.xlsx`
   (*Home → Transform data → Data source settings*).
4. Use the slicers to explore the data by Sales Method, Month and Year.

---

## 🔮 Future Improvements

- Add year-over-year and month-over-month growth measures
- Add a retailer-wise profit margin comparison
- Add drill-through pages for state and city level analysis
- Publish to Power BI Service for easy sharing

---

## 👤 Author

**Sanjay Singh**


⭐ If you found this project useful, consider giving it a star!
