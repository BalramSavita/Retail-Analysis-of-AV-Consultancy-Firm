🛍️ Retail Analysis of AV Firm

End-to-end data analytics project analyzing retail operations, sales trends, inventory, and resource scheduling of an Audio-Visual (AV) Consultancy Firm using Python, SQL, and Power BI.

📑 Table of Contents

📊 Project Overview

📂 Data Source

🗃️ Data Model

⚙️ Tools & Tech

📈 Dashboard Insights

💰 Sales & Retail Overview

📦 Inventory Overview

🚀 How to Reproduce

🔗 Resources

📊 Project Overview

This project focuses on the retail and service operations of an AV consultancy firm. The goal is to analyze sales, equipment inventory, and operational costs, while identifying areas of improvement in client delivery and resource allocation.

Through this project, we:

✅ Analyze sales & revenue performance across projects and equipment categories

✅ Track equipment inventory, valuation, and turnover

✅ Identify top-performing categories contributing to revenue

✅ Highlight downtime & repair costs impacting profitability

✅ Deliver a Power BI dashboard for interactive retail insights

📂 Data Source

The dataset (modeled on ERP-style retail data) contains:

🛒 Sales Orders – client purchases of AV services/equipment

🎥 Equipment Details – cameras, speakers, lighting, projectors

📦 Inventory Data – stock levels, valuation, and turnover

🛠 Maintenance Records – repair, downtime, and idle equipment costs

📅 Scheduling – deployment of assets for projects

🗃️ Data Model

We use a Star Schema for faster queries and dashboard refresh.

📌 Click to expand Data Model
⚙️ Tools & Tech
Python

SQL Server

Power BI

DAX

📈 Dashboard Insights

💰 Sales & Retail Overview

📅 Fiscal Year Calendar (Apr–Mar) built with DAX

📊 Cumulative Line Chart – Revenue trends over time

🍩 Donut Chart – Sales distribution across equipment categories

📉 Downtime Cost Trend – Yearly costs due to idle or repaired assets

👉 Category Drilldown

Pareto Charts → Top categories driving 80% of revenue

Matrix → Reasons for equipment downtime & financial impact

On-Time Deployment → Client projects delivered on or before schedule

📦 Inventory Overview

📌 KPIs: Inventory Quantity, Inventory Value, Turnover Rate

📈 Area Charts – Quantity vs. Valuation by equipment category

🔄 Turnover Multi-Line Chart – Compare yearly refresh/usage cycles

🚀 How to Reproduce

Data Prep (Python + SQL)

import pandas as pd sales = pd.read_csv("sales_orders.csv") print(sales.head())

SELECT Category, SUM(SalesAmount) AS Total_Revenue FROM FactSales GROUP BY Category ORDER BY Total_Revenue DESC;

Model Setup → Create star schema in SQL Server

Dashboard Build → Import tables into Power BI, create relationships, add measures

Total Revenue = SUM(FactSales[SalesAmount]) Inventory Value = SUM(FactInventory[Value])

Publish → Share the .pbix file or publish to Power BI Service

🔗 Resources

📘 SQL Queries → /SQL

🐍 Python Scripts → /Python

📊 Power BI Dashboard → /PowerBI/Retail_AV_Dashboard.pbix

🗂 Documentation → /Docs

✨ Final Insight: With this analysis, the AV consultancy firm can track revenue, sales trends, inventory health, and downtime costs. The Power BI dashboard enables management to make data-driven retail decisions for profitability and growth.
