# ☕ Cafe Sales Analysis Project (Data Cleaning + EDA)

## 📌 Project Overview
This project is an **end-to-end cafe sales data analysis project** that demonstrates how raw transactional data is cleaned, processed, and analyzed to generate meaningful business insights.

The project simulates a **real-world data analytics workflow**, starting from unclean data and transforming it into an analysis-ready dataset, followed by **exploratory data analysis (EDA)** using Python.

---

## 🎯 Objectives
- Clean and preprocess raw cafe sales data  
- Handle missing values, duplicates, and inconsistent data  
- Detect and treat outliers using statistical techniques  
- Perform exploratory data analysis (EDA)  
- Identify sales patterns and business trends  
- Generate actionable insights for decision-making  

---

## 🗃️ Dataset Description
The dataset contains **cafe sales transaction data**, where each row represents a customer order.

### Key Columns
- Transaction details: `Transaction ID`, `Transaction Date`  
- Product details: `Item`, `Price Per Unit`, `Quantity`  
- Sales details: `Total Spent`  
- Customer behavior: `Payment Method`, `Location`  

---

## 🧹 Data Cleaning & Preparation
Data cleaning was performed using **Python (Pandas, NumPy)**.

### Key Steps Performed
- Converted data types (`datetime`, `numeric`) using `errors='coerce'`  
- Handled missing values:
  - Numerical columns → filled using mean  
  - Categorical columns → filled with `"UNKNOWN"`  
- Removed invalid entries (`ERROR` values replaced with nulls)  
- Dropped rows with missing `Transaction Date`  
- Removed duplicate transactions using `Transaction ID`  
- Standardized categorical values  
- Corrected data inconsistencies:
  - Rounded `Quantity` to integers  
  - Rounded `Price Per Unit` for realistic pricing  
- Recalculated `Total Spent = Quantity × Price Per Unit`  

---

## 📉 Outlier Detection & Treatment
Outliers were handled using the **IQR (Interquartile Range) method**:

- Calculated Q1, Q3, and IQR  
- Defined lower and upper bounds  
- Removed extreme values from:
  - `Quantity`  
  - `Price Per Unit`  

> Note: `Total Spent` was not directly treated since it is a derived column.

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed using **Pandas, Matplotlib, and Seaborn**.

### Key Analysis Performed
1. Data quality assessment (missing values, duplicates)  
2. Univariate analysis (categorical & numerical variables)  
3. Bivariate analysis (sales performance by item)  
4. Time series analysis (monthly trends)  
5. Correlation analysis (heatmap)  
6. Customer segmentation (Low, Medium, High value customers)  

---

## 📈 Key Insights
- A small number of products contribute to a large portion of revenue  
- Sales show clear patterns across different time periods  
- High-value customers generate the majority of revenue  
- Certain locations outperform others significantly  
- Payment methods indicate customer preferences  

---

## 💼 Business Impact
This analysis helps businesses to:

- Optimize product offerings and pricing strategy  
- Improve inventory management  
- Identify high-value customer segments  
- Plan staffing based on peak hours  
- Enhance customer experience  
- Make data-driven strategic decisions  

---

## 🛠️ Tools & Technologies Used
- Python (Pandas, NumPy)  
- Matplotlib & Seaborn (Visualization)  
- Jupyter Notebook  

---

## 🚀 How to Run the Project
1. Download the dataset (`cafe_sales.csv`)  
2. Open notebooks in Jupyter Notebook / VS Code  
3. Run:
   - `01_cafe_sales_data_cleaning.ipynb`  
   - `02_cafe_sales_EDA.ipynb`  
4. Cleaned dataset will be saved as:
   - `cafe_sales_cleaned.csv`  
5. Analysis summary will be saved as:
   - `eda_results_summary.csv`  

---

## 📊 Future Enhancements
- Build an **interactive dashboard using Power BI / Tableau**  
- Add KPI cards (Revenue, Orders, Average Order Value)  
- Create filters (Date, Category, Location, Payment Method)  
- Visualize:
  - Sales trends over time  
  - Top-performing products  
  - Customer segments  
- Deploy dashboard for business use  
- Integrate real-time data pipeline (advanced level)  

---

## 👤 Author
**Pravin Kamble**  
Aspiring Data Analyst  
Skills: Python | SQL | Excel | Data Cleaning | EDA | Visualization  

---

## ⭐ Why This Project Matters
This project demonstrates:
- End-to-end data analytics workflow  
- Real-world data cleaning challenges  
- Strong exploratory data analysis skills  
- Ability to transform raw data into business insights  
- Job-ready data analyst capabilities  

---
