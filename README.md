# 📊 Sales Forecasting & Demand Prediction Analysis

An end-to-end **Data Analytics and Business Intelligence project** focused on analyzing historical retail sales, identifying demand patterns, evaluating product and store performance, and supporting future demand planning through trend-based forecasting.

The project uses **Excel, SQL (MySQL), and Power BI** to transform raw sales data into actionable business insights and an interactive dashboard.

---

## 📌 Project Overview

Retail businesses need accurate demand planning to maintain inventory, prepare for peak periods, optimize promotions, and make better business decisions.

This project analyzes historical sales data to answer key business questions such as:

- Which months have the highest sales?
- Are there recurring seasonal demand patterns?
- What is the overall sales trend?
- Which product families have the strongest demand?
- How do promotions and holidays affect sales?
- Which stores generate the highest sales?
- How can historical trends and forecasts support demand planning?

The project was designed around a real-world **Data Analyst business problem** involving sales planning and demand prediction.

---

## 🎯 Objectives

- Clean and preprocess historical retail sales data
- Analyze daily, monthly, and yearly sales trends
- Identify seasonal patterns and peak sales periods
- Analyze product-family and store-level performance
- Evaluate promotion and holiday sales impact
- Perform trend-based sales forecasting
- Build an interactive Power BI dashboard
- Generate business insights and recommendations for demand planning

The original project requirements specifically included data cleaning, historical trend analysis, seasonal analysis, basic forecasting, dashboard creation, and business recommendations.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Data cleaning, preprocessing and exploratory analysis |
| **MySQL** | Data storage, SQL analysis and business queries |
| **Power BI** | Interactive dashboard and data visualization |
| **Power Query** | Data transformation and preparation |
| **DAX** | KPI calculations and analytical measures |
| **GitHub** | Project documentation and version control |

---

## 📂 Dataset

The project uses a retail sales dataset containing historical sales information across multiple stores, product families, dates, promotions and holidays.

### Key Fields

- `id`
- `date`
- `store_nbr`
- `family`
- `sales`
- `onpromotion`
- `Year`
- `Month_number`
- `Month Name`
- `Quarter`
- `Day Name`
- `Promotion_Status`

Additional holiday information was incorporated to analyze the relationship between holidays and sales performance.

---

## 🔄 Project Workflow

```text
Raw Sales Dataset
       ↓
Data Cleaning & Preprocessing
       ↓
Excel Exploratory Analysis
       ↓
SQL Data Import
       ↓
SQL Business Analysis
       ↓
Power BI Data Modeling
       ↓
DAX Measures & KPIs
       ↓
Interactive Dashboard
       ↓
Trend & Forecast Analysis
       ↓
Business Insights & Recommendations
```

---

# 🧹 1. Data Cleaning & Preprocessing

The raw sales data was prepared before performing analysis.

### Cleaning activities included:

- Handling date fields
- Converting columns into appropriate data types
- Creating Year and Month attributes
- Creating Month Name and Quarter fields
- Creating Day Name fields
- Creating promotion status
- Preparing holiday-related information
- Checking numerical and categorical fields
- Preparing the dataset for SQL and Power BI analysis

The project requirements specifically included data cleaning and preprocessing before analysis.

---

# 📗 2. Excel Analysis

Excel was used for the initial analysis and preparation of the complete available dataset.

### Analysis Performed

- Monthly sales analysis
- Yearly sales analysis
- Product-family performance
- Promotion vs non-promotion sales
- Holiday vs non-holiday sales
- Sales trend analysis
- Peak-period identification
- Preliminary forecasting analysis

### Excel Scope

The Excel workbook contains the **full available dataset**, while the SQL and Power BI workflow uses a **100K-record subset** for analysis and dashboard development.

---

# 🗄️ 3. SQL Analysis

MySQL was used to perform structured business analysis on the cleaned sales dataset.

### SQL Analysis Areas

- Total sales analysis
- Yearly sales performance
- Monthly sales trends
- Product-family sales
- Store-level sales
- Promotion analysis
- Holiday analysis
- Sales aggregation
- Top-performing products
- Top-performing stores
- Demand-related analysis

### Example Business Questions

```sql
-- Total Sales
SELECT SUM(sales) AS total_sales
FROM sales_data;
```

```sql
-- Sales by Year
SELECT 
    Year,
    SUM(sales) AS total_sales
FROM sales_data
GROUP BY Year
ORDER BY Year;
```

```sql
-- Sales by Product Family
SELECT 
    family,
    SUM(sales) AS total_sales
FROM sales_data
GROUP BY family
ORDER BY total_sales DESC;
```

---

# 📊 4. Power BI Dashboard

An interactive Power BI dashboard was developed to provide a business-oriented view of sales performance and demand patterns.

### Dashboard Areas

#### 📌 Sales Overview

- Total Sales
- Total Records
- Yearly Sales
- Monthly Sales Trend
- Best Sales Year

#### 📌 Product & Store Analysis

- Sales by Product Family
- Top-performing Stores
- Product demand patterns
- Store-level performance

#### 📌 Promotion & Holiday Impact

- Promotion Sales
- Non-Promotion Sales
- Holiday Sales
- Non-Holiday Sales
- Promotion impact analysis

#### 📌 Forecast Analysis

- Historical Sales
- Forecasted Sales
- Actual vs Forecast
- Demand trend
- Forecast uncertainty

The dashboard structure addresses the project's required KPIs, monthly trend, product/category analysis, peak periods, and forecasted sales trend.

---

# 📈 5. Key Performance Indicators

| KPI | Result |
|---|---:|
| **Total Sales** | 77.96M |
| **Total Records** | 100.03K |
| **Promotion Sales** | 53.89M |
| **Holiday Sales** | 6.60M |
| **Non-Holiday Sales** | 71.36M |
| **Best Sales Year** | 2016 |

These SQL/Power BI KPI values are based on the **100K-record analysis subset**.

---

# 🔍 6. Key Insights

### 📅 Sales Trend

Sales increased from 2013 and reached the strongest annual performance in **2016**, followed by a decline in 2017.

### 🛒 Product Performance

**GROCERY I** was the highest-performing product family, followed by **BEVERAGES** and **PRODUCE**.

### 🏪 Store Performance

**Store 44** was the leading store within the Top 10 store analysis.

### 🎯 Promotion Impact

Promotion-related sales were approximately **53.89M**, compared with approximately **24.07M** for non-promotion sales.

### 🎉 Holiday Impact

Holiday sales accounted for approximately **6.60M**, while non-holiday sales accounted for approximately **71.36M**.

### 📆 Seasonal Patterns

Monthly sales showed noticeable peaks and fluctuations, with the pattern varying across different years.

### 🔮 Forecast

The trend-based forecast indicates continued demand with uncertainty. Forecast values should therefore be treated as **planning guidance rather than guaranteed future sales**. 

---

# 💡 7. Business Recommendations

### 1. Focus on High-Demand Products

Maintain sufficient inventory availability for consistently high-performing product families.

### 2. Improve Store-Level Planning

Give additional inventory-planning attention to high-performing stores.

### 3. Optimize Promotions

Evaluate promotional performance across products, stores and time periods.

### 4. Prepare for Peak Periods

Increase inventory readiness during historically strong sales periods.

### 5. Use Forecasts for Planning

Use forecast ranges as a planning input rather than treating forecast values as guaranteed future demand.

### 6. Investigate Sales Decline

Further investigate the factors contributing to the sales decline after the 2016 peak.

These recommendations are based on the project's final insights and recommendations analysis.

---

# 🎯 Business Questions Answered

| Business Question | Analysis |
|---|---|
| Which months have the highest sales? | Monthly sales trend analysis |
| Is there a seasonal pattern? | Monthly and yearly comparison |
| What is the overall sales trend? | Year-over-year analysis |
| Which products have strong future demand? | Product-family historical performance |
| How can demand planning be improved? | Forecast + product + store + promotion analysis |

These questions directly align with the final-project requirements.

---

# 📊 Project Deliverables

- ✅ Cleaned Dataset
- ✅ Excel Analysis
- ✅ SQL Analysis
- ✅ Power BI Dashboard
- ✅ Sales Trend Analysis
- ✅ Forecast Analysis
- ✅ Business Insights
- ✅ Recommendations

The original project deliverables required a dataset, cleaned data file, analysis file, dashboard, and final insights/recommendations summary.

---

# 🧠 Skills Demonstrated

### Data Analytics
- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Trend Analysis
- Seasonal Analysis
- Business Analysis

### SQL
- Data Aggregation
- GROUP BY
- ORDER BY
- Filtering
- Date-based Analysis
- Business KPI Queries

### Power BI
- Data Modeling
- DAX Measures
- KPI Cards
- Interactive Visualizations
- Slicers
- Dashboard Design
- Forecast Visualization

### Business Intelligence
- Demand Planning
- Inventory Planning
- Promotion Analysis
- Store Performance Analysis
- Product Performance Analysis
- Data-driven Decision Making

---

# 📌 Important Data Scope Note

The project uses two analytical scopes:

**Excel:** Full available dataset.

**SQL + Power BI:** 100K-record subset used for SQL analysis and dashboard development.

Therefore, totals and KPIs calculated in Excel may differ from the SQL/Power BI results. The reported **77.96M total sales and 100.03K records** specifically refer to the SQL/Power BI analysis scope.

---

# 🚀 Future Enhancements

Possible future improvements include:

- Machine-learning-based demand forecasting
- Product-level forecasting
- Store-level forecasting
- Automated Power BI refresh
- Advanced time-series models
- Forecast accuracy metrics such as MAE and RMSE
- Automated inventory-reorder recommendations
- Promotion uplift analysis

---

# 👨‍💻 Author

**Nandhan Mothukuri**

B.Tech – Computer Science & Engineering (AIML)

**Skills:**  
`Excel` `SQL` `Power BI` `Python` `Data Analytics` `Data Visualization`

---

## ⭐ Project Summary

This project demonstrates an end-to-end **Data Analyst workflow**, from raw sales data preparation and SQL analysis to Power BI dashboard development and business-oriented demand insights. It focuses on transforming historical retail data into actionable information for **sales planning, inventory management, promotion optimization, and demand planning**.
