Retail Sales Exploratory Data Analysis (EDA)
🔍 Objective

(Data Set link- https://drive.google.com/drive/folders/15xRub7_ZH1jkJmO1jNp-4VJ-77ks2hyU?usp=drive_link )

This project performs a detailed Exploratory Data Analysis (EDA) on a real-world Online Retail dataset from Kaggle.
The goal is to uncover business insights about sales trends, customer behavior, and product performance using Python, Pandas, NumPy, and Matplotlib/Seaborn.

🧰 Tools & Technologies

Python 3.10+
NumPy, Pandas — Data cleaning & transformation
Matplotlib, Seaborn — Visualization
VS Code
Kaggle dataset: Online Retail Dataset (UCI Machine Learning Repository)

🧩 Dataset Description

The dataset contains all transactions between 01/12/2010 and 09/12/2011 for a UK-based online store.

Column	Description
InvoiceNo	Transaction number (unique per invoice)
StockCode	Product ID
Description	Product name
Quantity	Units purchased
InvoiceDate	Date & time of transaction
UnitPrice	Price per unit
CustomerID	Unique customer number
Country	Customer location
🪜 Project Workflow
🧹 Data Cleaning & Preparation

Goal: Remove noise, handle missing values, and prepare data for analysis.
Steps:

Removed missing CustomerID entries.
Dropped canceled transactions (negative quantities).
Created TotalPrice = Quantity × UnitPrice.
Verified data types and date ranges.

Time Series Analysis
Goal: Understand sales performance over time.

Daily Revenue Trend
<img width="955" height="561" alt="Image" src="https://github.com/user-attachments/assets/804b61b2-2212-4e29-9a46-fd8415102a80" />
📆 Monthly Revenue Trend
<img width="1014" height="484" alt="Image" src="https://github.com/user-attachments/assets/ae3205b5-10a8-4cc9-8b99-1d6f3713bc5d" />
Insights:

Clear seasonal pattern: Sales peak in November, indicating holiday-driven demand.
Revenue growth observed from mid-year to Q4.
Drop in December due to partial data coverage.

Customer Segmentation (RFM Analysis)
Goal: Identify customer behavior & value segments.

Metric	Meaning	Business Value
Recency (R)	Days since last purchase	Indicates engagement
Frequency (F)	Number of purchases	Indicates loyalty
Monetary (M)	Total spending	Indicates value


Visuals:

🔥 RFM Correlation Heatmap
<img width="486" height="372" alt="Image" src="https://github.com/user-attachments/assets/dca770d2-2e82-4f99-902d-2c43cfe60cbf" />
📊 RFM Distribution (Recency, Frequency, Monetary)
<img width="1584" height="490" alt="Image" src="https://github.com/user-attachments/assets/b571c331-05d1-4e3d-8ef2-8fe51d322a87" />
Key Business Insights

✅ Sales Trend:
Revenue peaks during holiday season (Nov–Dec).
Sales growth trend throughout.
✅ Customer Behavior:
Loyal customers are high spenders.
A small portion of customers contributes most revenue.
✅ Product Insights:
Top 10 products account for ~60% of total sales.
High cancellation rates for specific SKUs → potential operational improvements.
