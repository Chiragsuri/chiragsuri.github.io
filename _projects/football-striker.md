---
title: "⚽ Football Striker Performance Analysis"
permalink: /projects/football-striker/
layout: single
author_profile: true
classes: wide
pagination: false
---

<div class="back-btn-top">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>

In this project, I dove deep into understanding what separates an ordinary striker from a great one. Using Python, I explored a dataset of 500 strikers containing personal attributes and on-field performance stats — all with the goal of answering one simple question:

👉 _What makes a football striker exceptional?_

## 🛠️ Tools & Technologies Used

- **Python (pandas, seaborn, matplotlib, scipy, sklearn, statsmodels)** – For EDA, visualization, statistical testing, clustering, and machine learning.
- **Jupyter Notebook** – For code execution and documentation.
- **Generative AI (ChatGPT)** – Helped refine analysis steps, validate statistical logic, helped with ideation and structure the project cleanly.

## 🔗 Links

<div class="links-grid">
  <a href="https://github.com/Chiragsuri" target="_blank" class="link-card">
    <i class="fa-brands fa-github"></i> GitHub
  </a>
  <a href="https://www.linkedin.com/in/chirag-suri/" target="_blank" class="link-card">
    <i class="fa-brands fa-linkedin"></i> LinkedIn
  </a>
  <a href="https://chiragsuri.github.io" target="_blank" class="link-card">
    <i class="fa-solid fa-globe"></i> Portfolio
  </a>
</div>

## 📁 Dataset

I worked with a dataset of **500 football strikers**, covering both demographic and performance-based variables.

- [`Strikers_Performance.xlsx`](https://github.com/Chiragsuri/Football-Striker-Performance/blob/main/Dataset/Strikers_Performance.xlsx)

📌 **Note**: I couldn’t locate the original source, so it’s being treated as synthetic/simulated data for educational purposes.

## 🎯 Project Objectives

This project was focused on segmenting and classifying strikers based on their:

- ⚽ **On-field performance** (Goals, Assists, Dribbling, etc.)
- 🧠 **Attributes** (Footedness, Consistency, Game IQ, Conduct)
- 📊 **Team Impact & Match Influence**

The broader goal was to develop a **data-backed system** for:

- Identifying top-tier vs average strikers.
- Helping scouts/coaches with player selection.
- Answering questions even analysts may overlook.

## 🧠 Key Questions Solved

- What’s the **maximum number of goals** scored by a striker?
- What **percentage of strikers are right-footed**?
- Which **nationality scores the most goals on average**?
- What’s the **average conversion rate** of left-footed players?
- Do **hold-up play skills** correlate with consistency?
- Are **consistency scores normally distributed**?
- Is there a **statistical difference** in performance between nationalities?
- Can we **predict striker types** using logistic regression?

## 🔄 Project Workflow

### 🧼 1. Data Cleaning & Preparation

- Handled null values using **SimpleImputer**:
  - Median for numeric
  - Most frequent for categorical
- Typecasting of key performance metrics (e.g., Goals, Assists).
- Used `LabelEncoder` for footedness and marital status.
- Created dummy variables for nationality.

### 📊 2. Exploratory Data Analysis

- Descriptive stats for all key metrics.
- Pie chart for footedness distribution.
- Countplot of footedness by nationality.

### 📈 3. Statistical Analysis

- Used **groupby + mean** to analyze national scoring rates.
- Performed **Shapiro-Wilk** for normality check.
- **Levene’s Test** to validate homogeneity before ANOVA.
- **Correlation (Pearson)** and **regression** to understand how "Hold-up Play" influences consistency.

### 🧪 4. Feature Engineering

- Created a **Total Contribution Score** from key fields:
  - Goals, Assists, Shots on Target, Dribbles, etc.
- Used this score for clustering and ML input.

### 🧠 5. K-Means Clustering

- Identified **2 clusters** using elbow method.
- Tagged strikers as:
  - **Best Strikers**
  - **Regular Strikers**

### 🤖 6. Machine Learning (Logistic Regression)

- Trained model to classify striker type.
- Used StandardScaler for normalization.
- Achieved solid accuracy and visualized predictions via confusion matrix.

<div class="links-grid" style="margin-top: 1rem;">
  <a href="https://github.com/Chiragsuri/Football-Striker-Performance/blob/main/Football-Striker.ipynb" class="link-card" target="_blank">
    <i class="fa-brands fa-python"></i> View Notebook
  </a>
</div>

## 💡 Key Insights

- 🥇 The highest individual goal tally: **36 goals**
- 🦵 Right-footed strikers dominate the dataset (about 73%)
- 🌍 **Brazilian** strikers had the highest average goal count
- 🧠 Hold-up Play shows positive correlation (0.55) with consistency
- 📊 Consistency scores were **not normally distributed**, but **heteroscedasticity was not an issue**
- 🧪 Regression model showed **hold-up play** significantly predicts **consistency**
- 🧮 Best strikers had an average contribution score of **~212**
- ✅ Logistic Regression model achieved **X% accuracy**

## 📚 Things I Learned

- ✅ **End-to-end structuring** of ML-based projects
- 📊 **Choosing the right statistical test** depending on data assumptions
- 🧹 Proper **preprocessing**: imputation, encoding, scaling
- 💬 **Explaining results** with storytelling, not just numbers
- 🤝 Using **generative AI** to validate and speed up analysis

## 🚀 How to Explore

If you're looking to test the code:

1. 📥 Clone or download the repo
2. 🐍 Open `Football-Striker.ipynb` in Jupyter
3. 🧠 Run through sections, tweak assumptions, explore clusters and model results

## ✅ What's Next?

- Building a **Power BI Dashboard** to turn this analysis into a visual scouting tool

## 🙏 THANK YOU! 🙌

<div class="back-btn-bottom">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>
