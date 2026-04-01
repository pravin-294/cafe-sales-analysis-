# ☕ Cafe Sales Analysis Project (Data Cleaning + EDA + Business Insights)

## 📌 Project Overview
This project is an **end-to-end data analytics case study** focused on analyzing cafe sales data. It demonstrates how raw, unstructured transactional data is transformed into meaningful insights through **data cleaning, preprocessing, and exploratory data analysis (EDA)**.

The workflow replicates a **real-world business scenario**, where data is often incomplete, inconsistent, and requires careful handling before analysis.

---

## 🎯 Objectives
- Clean and preprocess raw transactional data  
- Handle missing values, duplicates, and inconsistencies  
- Detect and treat outliers using statistical methods  
- Perform exploratory data analysis (EDA)  
- Identify key sales patterns and customer behavior  
- Generate actionable business insights  

---

## 🗃️ Dataset Description
The dataset contains **cafe transaction-level data**, where each row represents a customer purchase.

### Key Columns
- **Transaction Details:** `Transaction ID`, `Transaction Date`  
- **Product Details:** `Item`, `Price Per Unit`, `Quantity`  
- **Sales Metrics:** `Total Spent`  
- **Customer Behavior:** `Payment Method`, `Location`  

---

## 🧹 Data Cleaning & Preparation
Data preprocessing was performed using **Python (Pandas, NumPy)**.

### Key Steps Performed
- Converted data types using `errors='coerce'` to safely handle invalid entries  
- Handled missing values:
  - Numerical columns → filled using mean  
  - Categorical columns → filled with `"UNKNOWN"` to avoid bias  
- Replaced invalid values (`ERROR`) with nulls before processing  
- Removed rows with missing `Transaction Date`  
- Eliminated duplicate records using `Transaction ID`  
- Standardized categorical values  
- Fixed inconsistencies:
  - Rounded `Quantity` to integer values  
  - Adjusted `Price Per Unit` to realistic formats  
- Recalculated: Total Spent = Quantity × Price Per Unit
  
---

### ⚠️ Handling Missing Categorical Data
Instead of using mode imputation, missing categorical values were replaced with `"UNKNOWN"` to:
- Preserve data integrity  
- Avoid introducing artificial bias  
- Reflect real-world data collection issues  

---

## 📉 Outlier Detection & Treatment
Outliers were treated using the **IQR (Interquartile Range) method**:

- Calculated Q1, Q3, and IQR  
- Defined lower and upper bounds  
- Removed extreme values from:
- `Quantity`  
- `Price Per Unit`  

> Note: `Total Spent` was not directly modified as it is a derived metric.

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed using **Pandas, Matplotlib, and Seaborn**.

### Key Analysis Performed
1. Data quality assessment (missing values, duplicates)  
2. Univariate analysis (categorical & numerical distributions)  
3. Bivariate analysis (item-wise sales performance)  
4. Time series analysis (monthly revenue trends)  
5. Correlation analysis (heatmap)  
6. Customer segmentation:
 - Low Value  
 - Medium Value  
 - High Value  

---

## 📈 Key Insights
- A small set of products contributes significantly to total revenue  
- Monthly trends reveal fluctuations in sales performance  
- High-value customers generate a large share of revenue  
- Certain locations outperform others in terms of sales  
- A noticeable portion of transactions contains `"UNKNOWN"` values, indicating potential data collection gaps  

---

## 💼 Business Impact
This analysis can help businesses:

- Optimize product offerings and pricing strategies  
- Improve inventory planning  
- Identify and target high-value customers  
- Enhance operational planning (peak sales periods)  
- Detect data quality issues affecting decision-making  
- Enable data-driven strategic decisions  

---

## 📊 Dashboard (Planned Enhancement)
An interactive dashboard will be developed using **Power BI / Tableau** to present insights visually.

### Planned Features
- KPI Cards:
- Total Revenue  
- Total Orders  
- Average Order Value  
- Sales Trends (Time Series)  
- Top-Selling Products  
- Customer Segmentation  
- Payment Method Distribution  
- Filters:
- Date  
- Location  
- Item  
- Customer Segment  

---

## 🛠️ Tools & Technologies Used
- **Python:** Pandas, NumPy  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook / VS Code  

---

## 🚀 How to Run the Project
1. Download dataset: `cafe_sales.csv`  
2. Open project in Jupyter Notebook / VS Code  
3. Execute notebooks in order:
 - `01_cafe_sales_data_cleaning.ipynb`  
 - `02_cafe_sales_EDA.ipynb`  
4. Outputs generated:
 - Cleaned dataset → `cafe_sales_cleaned.csv`  
 - Analysis summary → `eda_results_summary.csv`  

---

## 🔮 Future Enhancements
- Build interactive BI dashboard (Power BI / Tableau)  
- Add sales forecasting models  
- Perform customer behavior analysis  
- Integrate real-time data pipeline (advanced)  

---

## 👤 Author
**Pravin Kamble**  
Aspiring Data Analyst  

**Skills:** Python | SQL | Excel | Data Cleaning | EDA | Data Visualization  

---

## ⭐ Why This Project Matters
This project demonstrates:
- End-to-end data analytics workflow  
- Real-world data cleaning and preprocessing  
- Strong exploratory data analysis skills  
- Business-oriented thinking and insights generation  
- Readiness for entry-level data analyst roles  
