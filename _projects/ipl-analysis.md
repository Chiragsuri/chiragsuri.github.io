---
title: "🏏 IPL Data Analysis (Season 2024 and 2025)"
permalink: /projects/ipl-analysis/
layout: single
author_profile: true
classes: wide
pagination: false
---

<div class="back-btn-top">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>

A data-driven project exploring player and team performances across the 2024 and 2025 IPL seasons — combining SQL, Python, Power BI, and Generative AI to break down everything from boundaries and catches to toss impact and review success.

## 🛠️ Tools & Technologies Used

- **SQL (MySQL)** – Used for slicing the main IPL dataset into filtered views for the 2024 and 2025 seasons.
- **Python (pandas, matplotlib, seaborn)** – Exploratory Data Analysis, player performance trends, season-wise insights.
- **Power BI** – Built a multi-page interactive dashboard with KPIs, slicers, trendlines, and maps.
- **Generative AI (ChatGPT)** – Assisted in ideation, error handling, SQL optimisation, notebook documentation, visual design, and storytelling.

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

## 📁 Dataset

The project started with a large **IPL Dataset** covering all IPL seasons. Using SQL, I derived three filtered datasets specifically for the 2024 and 2025 seasons:

- [`ipl_filtered_24_25.csv`](https://github.com/Chiragsuri/IPL_Analysis/blob/main/Dataset/ipl_filtered_24_25.csv) – Ball-by-ball data for the 2024–25 seasons only
- [`ipl_player_stats_24_25.csv`](https://github.com/Chiragsuri/IPL_Analysis/blob/main/Dataset/ipl_player_stats_24_25.csv) – Simplified version to track batter/bowler/wicket actions
- [`ipl_summary_24_25.csv`](https://github.com/Chiragsuri/IPL_Analysis/blob/main/Dataset/ipl_summary_24_25.csv) – Match-level summary (toss winner, result, player of match)

📎 **Original Source**:

<div class="links-grid">
<a href="https://www.kaggle.com/datasets/chaitu20/ipl-dataset2008-2025" class="link-card" target="_blank">
<i class="fa-solid fa-database"></i> Kaggle</a>
</div>

## 🎯 Problem Statements / Goals

This project wasn’t just about which team won more matches — it was about **uncovering patterns that aren’t obvious casually**, such as:

- **How important is the toss** — does **winning it** actually increase **win%**?
- Does **batting position** matter in **scoring runs**?
- Which players are **consistent** but **overlooked**?
- How **successful** are **DRS reviews** per team?
- What’s the typical **target score range** teams face in **chases**?
- Which teams are **tactically better** at **bowling dot balls**?
- Do some teams **dominate in catches** or commit **fewer fielding errors**?
- And lastly, in which **stadium** were **most IPL matches played** in those seasons?

## 🧪 Project Workflow

### <i class="fas fa-database"></i> SQL Phase

- Used Filtering methods to create 3 tables from the master IPL dataset.
- Removed cancelled matches and playoff outliers where needed.
- Wrote queries to calculate:
  <ul class="query-output-list">
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/most_runs_match.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Most Runs scored in a Single Match</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/orange_cap_25.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Orange Cap Leaderboard</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/purple_cap_25.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Purple Cap Leaderboard</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/most_catches_25.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Most Catches by Players</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/strike_rate_25.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Strike Rate of Top Batters</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/economy_rate_25.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Economy Rates of Top Bowlers</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/toss_win_impact.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Toss-Win Impact Summary</a></li>
  <li><a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/Exported%20Query%20Datasets/player_of_match.csv" target="_blank"><i class="fa-solid fa-file-lines"></i> Player of the Match Award Tally</a></li>
  </ul>

<div class="links-grid" style="margin-top: 1rem;">
<a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/MYSQL/IPLsql.sql" class="link-card" target="_blank">
<i class="fa-solid fa-code"></i> View SQL Script
</a>
</div>

---

### <i class="fab fa-python"></i> Python + Jupyter Notebook Phase

- Loaded the 3 pre-filtered datasets exported from MySQL Workbench into pandas.
- Validated datatypes, fixed inconsistencies (e.g., nulls in "runs_target", unknown fields).
- Season-separated stats and grouped analysis (2024 vs 2025).
- Built tables and visualisations for:
  - Team win% (excluding cancelled matches).
  - Catches per team (bar charts).
  - Dot Balls bowled by Each Team (bar charts).
  - Total Boundaries differentiated by number of 4s & 6s. (side-by-side bar charts).
  - Toss-Winner Impact on Match Result (Pie-Charts).
- Comments and markdowns added to enhance storytelling.

<div class="links-grid" style="margin-top: 1rem;">
  <a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/Python/IPL_Analysis.ipynb" class="link-card" target="_blank">
    <i class="fa-brands fa-python"></i> View Notebook
  </a>
</div>

---

### <i class="fas fa-chart-bar"></i> Power BI Dashboard

Built a 4-page dashboard with interactivity and visual elements:

#### 📄 Page 1: IPL Overview

- Total boundaries, matches, runs, deliveries (KPI cards).
- Team-wise venue map.
- Toss Winner v/s Match Winner Donut Chart.
- Slicers for seasons and teams.

![Overview](/docs/assets/IPLP1.png)

#### 📄 Page 2: Boundary & Dot Ball Insights

- Total Runs scored by Teams.
- Total 4s and 6s by team.
- Dot balls bowled per team (per season)
- Total Catches taken by each team.
- Slicers for seasons.

![Team Performance](/docs/assets/IPLP2.png)

#### 📄 Page 3: Batting Performance

- Trendline: Batting position vs runs scored.
- Donut: Top 10 boundary hitters
- Bar Charts: Top run scorers, wicket takers, i.e. Orange and Purple Cap Leaderboard.

![Player Performance](/docs/assets/IPLP3.png)

#### 📄 Page 4: Match Behaviour

- Review system summary
- Target range distribution while chasing

![Match Flow](/docs/assets/IPLP4.png)

✔️ Page navigation via buttons (no bookmarks/DAX required)

<div class="links-grid" style="margin-top: 1rem;">
  <a href="https://github.com/Chiragsuri/IPL_Analysis/blob/main/PowerBi_Dashboard/IPL_Analysis_Dashboard.pbix" class="link-card" target="_blank">
    <i class="fa-solid fa-chart-column"></i> Power BI Dashboard
  </a>
</div>

<!-- 🖼️ Published version: [*Add Power BI service link here*] -->

## 📊 Key Insights

- 🏏 **Punjab Kings** led in total catches in 2025.
- 🎯 Most teams had to chase targets of more than 200 runs.
- 🥇 **V. Kohli**, **B. Sai Sudharsan** had dominant batting performances.
- ⚖️ Toss winner didn't always secure match wins — strategy mattered more.
- 🔄 Several matches had successful DRS overturns — DRS efficiency varies by team.
- 🎯 Dot ball count helped teams control run flow, especially in 2024.

## 💡 Things I Learned

This project taught me a lot — not just about cricket data, but about organising a full-stack data project from scratch:

- How to set up and clean real-world data in SQL.
- Structuring exploratory analysis in Python before designing visuals.
- Creating clean, slicer-friendly dashboards in Power BI.
- Avoiding visual clutter and focusing on **what insights actually matter**.
- Balancing aesthetics with interactivity (tooltips, maps, dynamic filtering).
- Using AI tools for efficiency and handling complex tasks easily.

## 📦 How to Explore

If you're checking this project out:

1. You can review the `.sql` file to recreate the database
2. Use the Jupyter Notebook to experiment or modify visualisations
3. View the Power BI `.pbix` file directly, or try the online published version

## 🙏 THANK YOU

<div class="back-btn-bottom">
  <a href="/projects/"><i class="fa-solid fa-arrow-left"></i> Back to Projects</a>
</div>
