📌 Project Overview
This project analyzes transactional data from an online retail company to understand sales performance, product contribution, geographic distribution, and transaction patterns.
The analysis focuses on generating business-relevant insights using Python and exploratory data analysis (EDA).
The dataset contains real-world retail transactions, including multiple products, customers, and countries, making it suitable for practical sales analysis.
🗂 Data Source
Dataset: Online Retail Dataset (UCI Machine Learning Repository)
Period: December 2010 – December 2011
Records: ~541,000 transactions
Format: Excel (.xlsx)
❓ Business Questions
This analysis aims to answer the following questions:
How does revenue change over time?
Are sales driven by a few top products or many mid-tier products?
Which countries contribute most to total revenue?
Are sales driven by many small transactions or a few large ones?
🧹 Data Preparation & Cleaning
The original dataset does not include a revenue column.
Revenue was calculated as:
Revenue = Quantity × UnitPrice
The following cleaning steps were applied:
Removed transactions with Quantity ≤ 0 (returns or cancellations)
Removed transactions with UnitPrice ≤ 0 (invalid pricing)
Kept rows with missing CustomerID since the analysis focuses on sales performance, not customer segmentation
After cleaning:
~530,000 valid transaction rows remained
📈 Key Insights
1️⃣ Revenue Trend
Revenue shows clear seasonality
Sales peak toward the end of each quarter
November records the highest monthly revenue, indicating strong year-end demand
2️⃣ Product Performance
Revenue is not dominated by a single product
Many mid-tier products contribute meaningfully to total sales
This indicates a diversified and resilient product portfolio
3️⃣ Country Analysis
The United Kingdom accounts for the majority of total revenue
There is a large gap between the UK and the second-largest market
When excluding the UK:
Revenue is more evenly distributed
Netherlands leads among non-UK countries
No single non-UK country dominates sales
4️⃣ Invoice Size Analysis
Invoice revenue distribution is right-skewed
Most transactions have relatively low revenue
A small number of high-value invoices significantly increase the average revenue
This suggests:
Sales performance is mainly driven by transaction volume
Supported by occasional large orders
💡 Business Implications
Maintain strong operational capacity to handle high transaction volume
Ensure availability of mid-tier products, which form the revenue backbone
Reduce over-reliance on the UK by exploring international growth opportunities
Leverage high-value invoices through premium offerings or upselling strategies
🛠 Tools & Libraries
Python
pandas
matplotlib
seaborn
📌 Notes & Limitations
The dataset covers only one year of transactions
Customer-level analysis was not performed due to missing CustomerID values
Revenue analysis excludes returns and invalid pricing by design
🚀 Next Steps
Potential extensions of this analysis include:
Cohort or retention analysis
Customer segmentation (RFM) using complete customer data
Predictive sales forecasting
