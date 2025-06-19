---
title: "🛍️ Sales Data Dashboard (2023 vs 2024)"
permalink: /projects/sales-data-analysis/
layout: single
author_profile: true
classes: wide
pagination: false
---

<div class="back-btn-top">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>

A complete end-to-end data generation, cleaning, and visualization project comparing two business years (2023 vs 2024) through custom synthetic data. Built entirely in Python (Jupyter Notebook) and visualized using Power BI — combining storytelling with interactivity using dynamic slicers, maps, and custom tooltips.

## 🛠️ Tools & Technologies Used

- **Python (pandas, Faker, NumPy)** – Generated and cleaned 2023 & 2024 datasets using random logic and libraries.
- **Power BI** – Designed interactive dashboards with city/state maps, slicers, donut charts, KPI cards, tooltips, and bar graphs.
- **Generative AI (ChatGPT)** – Used as a co-pilot to debug scripts, organize logic, rewrite markdown, and brainstorm layout/design enhancements.

## 🔗 Links

<div class="links-grid">
  <a href="https://github.com/Chiragsuri" target="_blank" class="link-card">
    <i class="fa-brands fa-github"></i>
    GitHub
  </a>
  <a href="https://www.linkedin.com/in/chirag-suri/" target="_blank" class="link-card">
    <i class="fa-brands fa-linkedin"></i>
    LinkedIn
  </a>
  <a href="https://chiragsuri.github.io" target="_blank" class="link-card">
    <i class="fa-solid fa-globe"></i>
    Portfolio
  </a>
</div>

## 📁 Dataset Description

This project doesn’t use real-world business sales data. Instead:

🔹 I first **generated synthetic sales data** for 2023 and 2024 using Python’s Faker and NumPy libraries.  
🔹 Then saved them into two datasets:

- [`Sales_data_2023.csv`](https://github.com/Chiragsuri/Sales-Data-Analysis/blob/main/Datasets/sales_data_2023.csv)
- [`Sales_data_2024.csv`](https://github.com/Chiragsuri/Sales-Data-Analysis/blob/main/Datasets/sales_data_2024.csv)

## 🎯 Problem Statements / Goals

This project wasn’t just about revenue per year — it was about answering questions like:

- 🛒 Are certain **product categories** more dominant by **sales** or by **total orders**?
- 🏙️ Which **cities** contributed the most to overall **revenue**?
- 📈 How do **trends** change **month-by-month** across KPIs like **Sales**, **Orders**, **Quantity Sold**?
- 👤 Who are the **top customers** and how much are they contributing to our **growth**?
- 🧭 What is the **business growth direction** comparing **2023** and **2024**?

## 🔄 Project Workflow

### <i class="fab fa-python"></i> Python (Jupyter Notebook)

- Used `Faker`, `random`, and `NumPy` to simulate customer/product/order behaviour.
- Created logic blocks for 2023 and 2024 (product-category mappings, ID formats, etc.)
- Saved final outputs as `.csv` files for Power BI import.

<div class="links-grid" style="margin-top: 1rem;">
  <a href="https://github.com/Chiragsuri/Sales-Data-Analysis/blob/main/Python/SalesDataset.ipynb" class="link-card" target="_blank">
    <i class="fa-brands fa-python"></i> View Notebook
  </a>
</div>

---

### <i class="fas fa-chart-bar"></i> Power BI Dashboard

Built an interactive dashboard with 3 report pages covering:

#### 📄 Page 1: KPI Dashboard

- 📌 KPI cards: Sales, quantity sold, orders, customers
- 📈 Line charts: Month-wise trends
- 🎯 Gauges: Year-end vs target KPIs

![KPI Dashboard](/docs/assets/SalesDataKPI.png)

#### 📄 Page 2: Comparison Analysis

- 📊 Sales by product category (bar)
- 🧮 Orders by product category (donut)
- 🗺️ City-wise sales (map)
- 🧑 Top 100 customers by sales and quantity

![Comparison Analysis](/docs/assets/SalesDataComparison.png)

#### 📄 Page 3: Custom Tooltip View

- Tooltip with **Qtr-wise** breakdown
- Appears on visual hover in dashboards

![Tooltip Summary](/docs/assets/SalesDataTooltip.png)

<div class="links-grid" style="margin-top: 1rem;">
  <a href="https://github.com/Chiragsuri/Sales-Data-Analysis/blob/main/Dashboard/Sales_Data_Dashboard.pbix" class="link-card" target="_blank">
    <i class="fa-solid fa-chart-column"></i> Power BI Dashboard
  </a>
</div>

<!-- 🖼️ Published version: [*Add Power BI service link here*] -->

## 💡 Key Insights

- 📈 **2024** saw a spike in both **total customers** and **sales**.
- 🧢 **Clothing** & **Electronics** dominated in **sales** and **orders**.
- 🗺️ **San Francisco**, **New York**, **Houston** led **city-wise performance**.
- 💎 **Top 100 customers** made up over **60% of revenue**.
- 🎯 Most **KPIs** surpassed their original **2024 targets**.

## 🚀 Things I Learned

- How to create **realistic synthetic datasets** with Python.
- Balancing logic complexity with data readability.
- How to format and clean data to be dashboard-ready.
- Designing **Power BI dashboards that tell stories visually**.
- Using AI as a fast-thinking assistant in exploratory and design stages.

## 📦 How to Explore This Project

1. 📥 Download the datasets from the repo.
2. 🐍 Explore the logic in the Jupyter Notebook.
3. 📊 Open and analyze the Power BI `.pbix` file.
4. 🧭 Use filters/slicers in Power BI to explore dynamic trends.

## 🙏 THANK YOU

<div class="back-btn-bottom">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>
