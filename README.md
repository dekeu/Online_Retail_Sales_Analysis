# 📊 Online Retail Sales Analysis (Python)

## 📌 Project Overview
This project analyzes transactional data from an online retail company to understand **sales performance**, **product contribution**, **geographic distribution**, and **transaction patterns**. The analysis focuses on generating **business-relevant insights** using Python and exploratory data analysis (EDA).

---

## 🗂 Data Source
- **Dataset:** Online Retail Dataset (UCI Machine Learning Repository)
- **Period:** December 2010 – December 2011
- **Records:** ~541,000 transactions
- **Format:** Excel (.xlsx)

---

## ❓ Business Questions
This analysis aims to answer:
1. How does revenue change over time?
2. Are sales driven by a few top products or many mid-tier products?
3. Which countries contribute most to total revenue?
4. Are sales driven by many small transactions or a few large ones?

---

## 🧹 Data Preparation & Cleaning
The original dataset does not include a revenue column. Revenue was calculated as:

`Revenue = Quantity × UnitPrice`

Cleaning steps:
- Removed transactions with `Quantity ≤ 0` (returns or cancellations)
- Removed transactions with `UnitPrice ≤ 0` (invalid pricing)
- Kept rows with missing `CustomerID` since the analysis focuses on **sales performance**, not customer segmentation

After cleaning:
- ~530,000 valid transaction rows remained

---

## 📈 Key Insights

### 1️⃣ Revenue Trend
- Revenue shows **clear seasonality**
- Sales increase toward the **end of each quarter**
- **November** records the highest monthly revenue, indicating strong year-end demand

### 2️⃣ Product Performance
- Revenue is **not dominated by a single product**
- Many **mid-tier products** contribute meaningfully to total sales
- This suggests a **diversified product portfolio**

### 3️⃣ Country Analysis
- The **United Kingdom** accounts for the majority
