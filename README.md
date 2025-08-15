# Customer Segmentation with RFM (Python)

Turn raw retail transactions into clear, actionable customer segments using **RFM analysis** (Recency, Frequency, Monetary) and **K-Means clustering**. This project walks from **data cleaning** and **feature engineering** through **segmentation**, **profiling**, and **marketing recommendations**.

> Highlights: statistical analysis, RFM scoring, unsupervised clustering, returns analysis, time trends, and geography insights.

---

## 📊 Results at a glance

- **Dataset (post-cleaning):** 401,604 rows × 8 columns  
- **Time period:** 2010-12-01 to 2011-12-09  
- **Unique customers:** 4,372  
- **Return rate:** 2.21% of orders  
- **Top revenue product:** “REGENCY CAKESTAND 3 TIER” (~132,567.70)  
- **K-Means segments:** 4 clusters (Top, High, Medium, Low/Lost) via RFM

> Numbers above are computed directly in the notebook. Profitability uses a **simulated cost** assumption and payment methods are **randomly assigned** for demo purposes, so profit and payment-method insights are illustrative rather than financial truths.
---

## 🧠 What you’ll learn

- Clean and validate transactional data (null handling, deduping, typing)
- Engineer features (Total_Spend, OrderHour, DayOfWeek, YearMonth)
- Compute **Recency**, **Frequency**, **Monetary** per customer
- Normalize and combine into an **RFM Score**
- Cluster customers with **K-Means** and profile each segment
- Analyze **returns**, **time-of-day/day-of-week** patterns, and **country** trends
- Translate segments into **marketing recommendations**

---

## 🗂️ Repo structure
├─ data.csv
├─ Python_RFM_Analysis.ipynb
├─ README.md # this file



🔬 Methodology
Data cleaning & QA

Drop null CustomerID, remove duplicates, convert dtypes

Address negative quantities for returns analysis

Feature engineering

Total_Spend = UnitPrice * Quantity

Time features: OrderHour, DayOfWeek, YearMonth

(Demo-only) Payment Method is randomly assigned

RFM computation

Recency: days since last purchase

Frequency: number of unique invoices

Monetary: total spend per customer

Rank/normalize and combine into RFM Score

Clustering

Standardize RFM features

K-Means (k=4) chosen with elbow inspection

Assign segments and profile clusters

Evaluation & insights

Top products and revenue drivers

Returns (% and by product)

Time trends (by weekday/hour, monthly)

Geography (orders by country; avg order value)

Recommendations

Tailored actions for Top, High, Medium, Low/Lost segments

Loyalty, upsell, bundles, win-back, education

📈 Key figures (selected)
Most ordered products: e.g., WHITE HANGING HEART T-LIGHT HOLDER; REGENCY CAKESTAND 3 TIER

Return rate: 2.21% of orders

Illustrative total profit: ~568,057 (depends on simulated cost)

High-activity customers: clear long tail with a few heavy buyers

See notebook cells for exact plots: top products, monthly trends, orders by weekday/hour, cluster scatter, etc.


