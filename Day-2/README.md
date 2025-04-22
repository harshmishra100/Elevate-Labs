# Data Visualization & Storytelling – Superstore Analysis

## 📂 Dataset
- **File:** `Sample - superstore.csv`  
- **Rows:** ~10,000  
- **Fields:** Order‑, Customer‑, Product‑, Sales, Quantity, Discount, Profit, etc.

## 🧹 Data Preprocessing
1. **Load & inspect** raw data.  
2. **No nulls** detected → no imputation needed.  
3. **Converted** order and ship dates to proper date format.  
4. **Derived columns:**  
   - `Shipping Time` (days between order and ship)  
   - `Order Year`, `Order Month`  
5. **Removed duplicates** and verified final dataset.

## 📊 Visualizations & Key Insights

| # | Chart                                    | Insight                                                                                  |
|:-:|-----------------------------------------|------------------------------------------------------------------------------------------|
| 1 | **Sales & Profit by Category**          | - Technology drives the highest profit margin.  <br>- Furniture shows high sales but slimmer profits, suggesting price optimization. |
| 2 | **Sales & Profit by Sub‑Category**      | - Phones and Chairs lead in sales.  <br>- Tables occasionally run negative profit, indicating heavy discounts or returns. |
| 3 | **Monthly Sales Trend**                 | - Seasonal peaks in November–December.  <br>- Steady growth year‑over‑year; promotions could target slower months (Jan–Mar). |
| 4 | **Sales & Profit by Region**            | - West region leads in total sales, while South achieves the best profit margin.         |
| 5 | **Shipping Time Distribution**          | - Majority of orders ship within 2–5 days.  <br>- A few outliers at 10+ days—operations should investigate bottlenecks. |
| 6 | **Discount vs Profit**                  | - Discounts above ~40% correlate with sharp profit declines.  <br>- Capping discounts around 20% could protect margins. |
| 7 | **Top 10 Products by Sales**            | - Best‑selling items are high‑volume office supplies and phones.  <br>- Bundling these with lower‑margin items can boost overall profitability. |

*(Place each chart image here or reference screenshots in an `images/` folder.)*

## 🧩 Storyboard / Executive Summary

1. **Overall Performance**  
   - Technology category and Phones sub‑category are primary profit drivers.  
   - Furniture sales strong, but profit margins lag—review pricing strategy.  
2. **Seasonality**  
   - November–December sales peaks → align inventory and staffing accordingly.  
3. **Regional Opportunities**  
   - Focus marketing spend in the West to capitalize on volume.  
   - Replicate South’s profitability tactics in other regions.  
4. **Operational Efficiency**  
   - Address shipping outliers to improve delivery consistency.  
5. **Pricing & Promotions**  
   - Implement a discount cap of around 20% to safeguard profits.  
   - Use targeted promotions during slower months to smooth revenue.

---

## 📤 Submission Instructions
1. **Notebook:** `Superstore.ipynb`  
2. **Charts:** Export each figure as PNG and include in an `images/` folder.  
3. **README.md:** This file.  
4. **GitHub:** Create a new repository named `data-viz-superstore` and push all files. Then submit the repository link via the assignment portal.
