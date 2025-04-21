# Elevate-Labs

# Data Analyst Internship – Task 1  
**Mall Customer Data Cleaning & Analysis**

## 📄 Description  
This repository contains my work for Task 1 of the Data Analyst Internship: cleaning and preprocessing the Mall Customer Segmentation dataset, followed by exploratory data analysis and basic customer segmentation. The goal was to transform the raw data into a clean, analysis-ready form and extract actionable insights.

---

## 🗂️ File Structure  

---

## 📊 Dataset  
**Mall Customer Segmentation Data** (from Kaggle)  
- **Fields:**  
  - `CustomerID`  
  - `Gender`  
  - `Age`  
  - `Annual Income (k$)`  
  - `Spending Score (1–100)`

---

## 🎯 Objective  
- **Primary:** Clean and preprocess the raw dataset (handle nulls, duplicates, inconsistent formats, column names, data types).  
- **Secondary (extra credit):**  
  1. Exploratory Data Analysis (EDA)  
  2. Customer segmentation via K‑Means clustering  
  3. Derive customer personas and key insights

---

## 🛠️ Tools & Libraries  
- **Environment:** Jupyter Notebook  
- **Core Libraries:**  
  - `pandas` for data manipulation  
  - `matplotlib` & `seaborn` for visualization  
  - `scikit‑learn` for clustering  
- **Optional (if you re-run):**  
  - `numpy`  
  - `plotly` or `streamlit` for interactive dashboards

---

## ⚙️ Steps Performed

### 1. Data Cleaning & Preprocessing  
1. **Load data** with Pandas  
2. **Inspect structure** (`.shape`, `.info()`, `.describe()`)  
3. **Missing‐value check** (none found)  
4. **Duplicate removal** with `drop_duplicates()`  
5. **Text standardization**: `Gender` → lowercase, stripped  
6. **Column rename** → lowercase + underscores  
7. **Type conversion**:  
   - `age`, `annual_income_(k$)`, `spending_score_(1-100)` → `int`  
8. **Export** cleaned file as `Mall_customers_cleaned.csv`

### 2. Exploratory Data Analysis (EDA)  
- **Gender distribution** (bar chart)  
- **Age distribution** (histogram + KDE)  
- **Income distribution** (histogram + KDE)  
- **Spending Score distribution** (histogram + KDE)  
- **Bivariate plots:**  
  - Income vs. Spending Score (scatter, colored by gender)  
  - Age vs. Spending Score (scatter, colored by gender)  
- **Feature correlation** (heatmap of numeric fields)

### 3. Customer Segmentation (K‑Means)  
1. **Feature selection:** `age`, `annual_income_(k$)`, `spending_score_(1-100)`  
2. **Scaling:** StandardScaler → zero mean, unit variance  
3. **K‑Means clustering:** chosen **k = 5** (elbow method can be added)  
4. **Label assignment:** new column `cluster`  
5. **Cluster visualization:** scatterplots of income vs. score

---

## 💡 Key Insights & Takeaways  
- **Gender Split:** roughly balanced male/female customer base.  
- **Spending Patterns:** distinct groups emerge—“High income, low spender”, “Low income, high spender”, etc.  
- **Age Effect:** younger customers tend to have higher spending scores but lower incomes.  
- **Segmentation Personas:**  
  1. **“Big Spenders”** – Medium age, high income & spending  
  2. **“Budget Youth”** – Young, low income, moderate spending  
  3. **“Cautious Seniors”** – Older, moderate income, low spending  
  4. **…and two more clusters that can guide targeted marketing.**

---

## 🚀 How to Reproduce  
1. **Clone this repo**  
   ```bash
   git clone https://github.com/<your‑username>/mall-customer-cleaning.git
   cd mall-customer-cleaning
