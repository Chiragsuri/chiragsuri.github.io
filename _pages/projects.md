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
    <span class="header-eyebrow">The Archive</span>
    <h1>Case Studies</h1>
    <p>I build pipelines that scale and dashboards that actually get used. Here are five times I turned messy, disconnected data into strategic leverage for decision-makers.</p>
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
      <div class="card-slider">
        <div class="slider-track track-4">
          <img src="/docs/assets/SHM_Dashboard1.png" alt="Executive Overview">
          <img src="/docs/assets/SHM_Dashboard2.png" alt="Anomaly & Risk Monitor">
          <img src="/docs/assets/SHM_Dashboard3.png" alt="Customer Intelligence">
          <img src="/docs/assets/SHM_Dashboard4.png" alt="Geographic Performance">
        </div>
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Engineering · BI</div>
      <h2 class="project-name">Retail Revenue & Anomaly Detection</h2>
      <p class="project-desc">Processed 800,000+ records via a custom star schema. Deployed an anomaly detection layer that cut false alerts by 85%, delivering a clean Power BI dashboard for exact revenue tracking.</p>
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
  <div class="project-showcase reveal" data-category="analytics">
    <a href="/projects/ipl-analysis/" class="project-visual">
      <div class="card-slider">
        <div class="slider-track track-4 alt-timing">
          <img src="/docs/assets/IPLP1.png" alt="IPL Overview">
          <img src="/docs/assets/IPLP2.png" alt="Team Performance">
          <img src="/docs/assets/IPLP3.png" alt="Players Performance">
          <img src="/docs/assets/IPLP4.png" alt="Match Flow">
        </div>
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · SQL</div>
      <h2 class="project-name">Performance Forecasting Model</h2>
      <p class="project-desc">Analyzed 145 distinct datasets to forecast player and team KPIs. This interactive tool tracks batting trends and boundary patterns, enabling coaching staff to build data-backed match strategies.</p>
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
      <div class="card-slider">
        <div class="slider-track track-1">
          <img src="/docs/assets/FootballStriker.png" alt="Football Striker Segmentation">
        </div>
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Machine Learning · Python</div>
      <h2 class="project-name">Football Striker Segmentation</h2>
      <p class="project-desc">Applied K-Means clustering across 500 elite players to isolate goal-scoring drivers. Engineered custom contribution scores to build a classification model predicting future on-pitch performance.</p>
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
  <div class="project-showcase reveal" data-category="analytics">
    <a href="/projects/sales-data-analysis/" class="project-visual">
      <div class="card-slider">
        <div class="slider-track track-3">
          <img src="/docs/assets/SalesDataKPI.png" alt="Sales Data KPI Dashboard">
          <img src="/docs/assets/SalesDataComparison.png" alt="Sales Data YoY Comparison">
          <img src="/docs/assets/SalesDataToolTip.png" alt="Sales Data Tooltip View">
        </div>
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · BI</div>
      <h2 class="project-name">Year-Over-Year Sales Analytics</h2>
      <p class="project-desc">End-to-end dashboard comparing 2023 vs. 2024 performance. Generated synthetic datasets using Python to visualize YoY growth, customer behavior, and city-level trends in Power BI.</p>
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
      <div class="card-slider">
        <div class="slider-track track-1">
          <img src="/docs/assets/HouseSales.png" alt="Geospatial Real Estate Valuation">
        </div>
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics · Tableau</div>
      <h2 class="project-name">Geospatial Real Estate Valuation</h2>
      <p class="project-desc">Normalized King County housing records into a dynamic geographic mapping tool. Filters property valuations by condition and build year to illustrate how local geography dictates market ceilings.</p>
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
    <a href="/" class="nav-btn prev-btn">
      <span class="nav-arrow">&larr;</span>
      <span>Back to Home</span>
    </a>
    <a href="/certifications/" class="nav-btn next-btn">
      <span>Certifications</span>
      <span class="nav-arrow">&rarr;</span>
    </a>
  </div>

</div>

<!-- Filter & Dynamic Layout Javascript -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    const tabs = document.querySelectorAll(".filter-tab");
    const projects = document.querySelectorAll(".project-showcase");

    // This function runs every time you click a filter. 
    // It guarantees that only visible projects get the alternating left/right layout.
    function applyAlternatingLayout(filterStr) {
      let visibleCount = 0;
      
      projects.forEach(project => {
        if (filterStr === "all" || project.getAttribute("data-category") === filterStr) {
          project.style.display = "flex";
          
          // Dynamically apply zig-zag based on visibility index
          if (visibleCount % 2 !== 0) {
            project.classList.add("reverse");
          } else {
            project.classList.remove("reverse");
          }
          
          visibleCount++;
          setTimeout(() => { project.classList.add("active"); }, 50);
        } else {
          project.style.display = "none";
          project.classList.remove("active");
        }
      });
    }

    // Run once on page load to set up the initial "All" view
    applyAlternatingLayout("all");

    tabs.forEach(tab => {
      tab.addEventListener("click", () => {
        // Handle tab active state
        tabs.forEach(t => t.classList.remove("active"));
        tab.classList.add("active");
        
        // Grab the data attribute and run the layout function
        const filter = tab.getAttribute("data-filter");
        applyAlternatingLayout(filter);
      });
    });
    
    // Intersection Observer for scroll animations
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
