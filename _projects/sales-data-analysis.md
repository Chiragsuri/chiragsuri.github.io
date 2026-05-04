---
permalink: /projects/
layout: single
title: ""
author_profile: false
classes: wide
header: false
---

<div class="archive-container">

  <div class="projects-header reveal active">
    <span class="header-eyebrow">Selected Work</span>
    <h1>Case Studies</h1>
    <p>Five strategic projects across data engineering, analytics, and machine learning designed to give leadership actionable visibility into performance.</p>
  </div>

  <div class="filter-bar reveal active">
    <button class="filter-tab active" data-filter="all">All</button>
    <button class="filter-tab" data-filter="engineering">Engineering & BI</button>
    <button class="filter-tab" data-filter="analytics">Analytics</button>
    <button class="filter-tab" data-filter="ml">Machine Learning</button>
  </div>

  <!-- 1. Retail Revenue & Anomaly Detection -->
  <div class="project-showcase reveal" data-category="engineering">
    <a href="/projects/sales-health-monitor/" class="project-visual">
      <div class="slider-track track-1">
        <img src="/docs/assets/SHM_Dashboard1.png" alt="Retail Revenue & Anomaly Detection">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Engineering · BI</div>
      <h2 class="project-name">Retail Revenue & Anomaly Detection</h2>
      <p class="project-desc">Processing 800,000 transaction records required a custom star schema. I built this architecture across eight tables and deployed an anomaly detection layer that cut false-positive alerts by 85%. The result is a clean Power BI dashboard that lets executives track actual revenue health instead of chasing ghost data.</p>
      <div class="project-tech">
        <span class="has-tooltip" data-tooltip="Star schema with 8 tables & 11 views">MySQL</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Multi-page dashboards">Power BI</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Data validation & automation">Python</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Time intelligence">DAX</span>
      </div>
      <div class="project-actions">
        <a href="/projects/sales-health-monitor/" class="project-link">Read Case Study →</a>
        <a href="https://github.com/Chiragsuri/Sales_Health_Monitor" target="_blank" class="project-link-secondary">GitHub ↗</a>
      </div>
    </div>
  </div>

  <!-- 2. Performance Forecasting Model (IPL) -->
  <div class="project-showcase reverse reveal" data-category="analytics">
    <a href="/projects/ipl-analysis/" class="project-visual">
      <div class="slider-track track-1">
        <img src="/docs/assets/IPLP1.png" alt="Performance Forecasting Model">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · SQL</div>
      <h2 class="project-name">Performance Forecasting Model</h2>
      <p class="project-desc">Franchise sports run on razor-thin margins. I built this forecasting model to track player and team performance across 145 distinct IPL datasets. By isolating batting trends and boundary patterns into an interactive tool, coaching staff can project match momentum and build data-backed strategies.</p>
      <div class="project-tech">
        <span class="has-tooltip" data-tooltip="Complex query filtering">SQL</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Pandas, Matplotlib">Python</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Interactive reporting">Power BI</span>
      </div>
      <div class="project-actions">
        <a href="/projects/ipl-analysis/" class="project-link">Read Case Study →</a>
        <a href="https://github.com/Chiragsuri/IPL_Analysis" target="_blank" class="project-link-secondary">GitHub ↗</a>
      </div>
    </div>
  </div>

  <!-- 3. Football Striker Segmentation -->
  <div class="project-showcase reveal" data-category="ml">
    <a href="/projects/football-striker/" class="project-visual">
      <div class="slider-track track-1">
        <img src="/docs/assets/FootballStriker.png" alt="Football Striker Segmentation">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Machine Learning · Python</div>
      <h2 class="project-name">Football Striker Segmentation</h2>
      <p class="project-desc">Finding undervalued talent requires looking past basic stats. I applied K-Means clustering across 500 elite players to isolate the true drivers of goal-scoring. By engineering custom contribution scores from raw match logs, I developed a classification model that correlates strongly with future on-pitch performance.</p>
      <div class="project-tech">
        <span class="has-tooltip" data-tooltip="Statistical clustering">Scikit-learn</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Data processing">Python</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Visual plotting">Seaborn</span>
      </div>
      <div class="project-actions">
        <a href="/projects/football-striker/" class="project-link">Read Case Study →</a>
        <a href="https://github.com/Chiragsuri/Football-Striker-Performance" target="_blank" class="project-link-secondary">GitHub ↗</a>
      </div>
    </div>
  </div>

  <!-- 4. Year-Over-Year Sales Analytics -->
  <div class="project-showcase reverse reveal" data-category="analytics">
    <a href="/projects/sales-data-analysis/" class="project-visual">
      <div class="slider-track track-1">
        <img src="/docs/assets/SalesDataKPI.png" alt="Year-Over-Year Sales Analytics">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · BI</div>
      <h2 class="project-name">Year-Over-Year Sales Analytics</h2>
      <p class="project-desc">I built this end-to-end sales analytics dashboard to compare business performance between 2023 and 2024. Using Python libraries like pandas, NumPy, and Faker, I generated and cleaned realistic synthetic datasets, routing them into Power BI to visualize YoY growth, customer behavior, and city-level trends.</p>
      <div class="project-tech">
        <span class="has-tooltip" data-tooltip="Data manipulation">Pandas</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Synthetic data generation">Faker</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Interactive slicing">Power BI</span>
      </div>
      <div class="project-actions">
        <a href="/projects/sales-data-analysis/" class="project-link">Read Case Study →</a>
        <a href="https://github.com/Chiragsuri/Sales-Data-Analysis" target="_blank" class="project-link-secondary">GitHub ↗</a>
      </div>
    </div>
  </div>

  <!-- 5. Geospatial Real Estate Valuation -->
  <div class="project-showcase reveal" data-category="analytics">
    <a href="https://public.tableau.com/app/profile/chirag.suri/viz/KingCountyHouseSales_16953115471270/KingCountyHouseSales" target="_blank" class="project-visual">
      <div class="slider-track track-1">
        <img src="/docs/assets/HouseSales.png" alt="Geospatial Real Estate Valuation">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · Tableau</div>
      <h2 class="project-name">Geospatial Real Estate Valuation</h2>
      <p class="project-desc">Raw property records are notoriously disorganized. I stripped and normalized the King County housing database to build a dynamic geographic mapping tool. The dashboard filters property valuations by physical condition and build year, illustrating exactly how hyper-local geography dictates market price ceilings.</p>
      <div class="project-tech">
        <span class="has-tooltip" data-tooltip="Data cleansing">Excel</span> <span class="dot">•</span>
        <span class="has-tooltip" data-tooltip="Geospatial visualization">Tableau</span>
      </div>
      <div class="project-actions">
        <a href="https://public.tableau.com/app/profile/chirag.suri/viz/KingCountyHouseSales_16953115471270/KingCountyHouseSales" target="_blank" class="project-link">View Dashboard ↗</a>
      </div>
    </div>
  </div>

  <div class="projects-page-nav">
    <a href="/">← Back to Home</a>
    <a href="/certifications/">Certifications →</a>
  </div>

</div>

<!-- Filter Javascript -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const tabs = document.querySelectorAll(".filter-tab");
    const projects = document.querySelectorAll(".project-showcase");

    tabs.forEach(tab => {
      tab.addEventListener("click", () => {
        tabs.forEach(t => t.classList.remove("active"));
        tab.classList.add("active");
        
        const filter = tab.getAttribute("data-filter");
        
        projects.forEach(project => {
          if (filter === "all" || project.getAttribute("data-category") === filter) {
            project.style.display = "flex";
            setTimeout(() => { project.classList.add("active"); }, 50);
          } else {
            project.style.display = "none";
            project.classList.remove("active");
          }
        });
      });
    });
    
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('active');
        }
      });
    }, { threshold: 0.1 });

    projects.forEach(project => observer.observe(project));
  });
</script>
