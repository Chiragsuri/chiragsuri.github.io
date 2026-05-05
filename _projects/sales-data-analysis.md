---
title: "Year-Over-Year Sales Analytics"
permalink: /projects/sales-data-analysis/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/football-striker/" class="side-nav-btn prev-btn-floating" title="Previous Project"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/house-sales-analysis/" class="side-nav-btn next-btn-floating" title="Next Project"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Analytics · BI</span>

  <h1 class="cs-title">Year-Over-Year Sales<br>Analytics</h1>
  <p class="cs-subtitle">An end-to-end dashboard comparing 2023 against 2024. Without access to proprietary corporate data, I engineered a Python script to generate a realistic synthetic ledger, mapping out year-over-year growth, customer habits, and regional trends.</p>

  <div class="cs-metrics-strip">
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="2">0</span></span>
      <span class="cs-metric-label">Years Simulated</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="3">0</span></span>
      <span class="cs-metric-label">Interactive Views</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="60">0</span>%</span>
      <span class="cs-metric-label">Top Customer Revenue</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="4">0</span></span>
      <span class="cs-metric-label">Core KPIs Tracked</span>
    </div>
  </div>

  <div class="cs-brief-grid">
    <div class="cs-brief-context">
      <p>Most YoY reports stop at top-line revenue. I wanted to see the underlying mechanics-how specific cities, product categories, and top customers shifted from one year to the next. Since I didn't have access to a real company's private sales database, I built a Python engine using Faker and NumPy to simulate millions of realistic transactions, complete with seasonal logic and product category mappings.</p>
    </div>
    <div class="cs-brief-meta">
      <h4>Tech Stack</h4>
      <div class="cs-tech-tags">
        <span class="cs-tech-tag">Python</span>
        <span class="cs-tech-tag">Pandas</span>
        <span class="cs-tech-tag">Faker</span>
        <span class="cs-tech-tag">NumPy</span>
        <span class="cs-tech-tag">Power BI</span>
      </div>
    </div>
  </div>

  <h2 class="cs-section-label">The Methodology</h2>

  <div class="cs-approach-grid">
    <div class="cs-approach-card">
      <i class="fa-solid fa-code cs-approach-icon"></i>
      <h3>1. Synthetic Data Engineering</h3>
      <p>Used Python libraries (Faker, NumPy) to simulate realistic customer and order behavior. I hardcoded specific logic blocks to ensure product categories mapped correctly to prices and seasonal buying habits.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-table cs-approach-icon"></i>
      <h3>2. Data Structuring</h3>
      <p>Formatted the raw simulation outputs into clean CSVs, ensuring all dates, primary keys, and data types were perfectly structured for relational modeling before they ever touched a BI tool.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-chart-pie cs-approach-icon"></i>
      <h3>3. Visual Analytics</h3>
      <p>Built a three-page Power BI dashboard featuring dynamic mapping, custom hover tooltips, and gauge charts to actively track actual performance against simulated 2024 targets.</p>
    </div>
  </div>

  <h2 class="cs-section-label">The Deliverables</h2>

  <div class="cs-image-grid">
    <div class="cs-showcase-item">
      <img src="/docs/assets/SalesDataKPI.png" alt="Sales Data KPI Dashboard" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 1: KPI Tracking, measuring actuals against yearly targets.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/SalesDataComparison.png" alt="Sales Data YoY Comparison" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 2: Comparison Analysis, mapping city revenues and category splits.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/SalesDataTooltip.png" alt="Sales Data Tooltip View" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 3: Custom Tooltip View, revealing quarterly breakdowns on hover.</div>
    </div>
  </div>

  <h2 class="cs-section-label">Key Findings</h2>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">The Pareto principle holds true.</h3>
    <p class="cs-finding-context">Even in a synthetic model designed with random variance, the top 100 customers accounted for over 60% of total revenue. This proves why identifying and isolating VIP cohorts is more important than tracking raw traffic.</p>
  </div>
  
  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Geography dictates volume.</h3>
    <p class="cs-finding-context">San Francisco, New York, and Houston heavily skewed the sales map. Drilling down into the Power BI map filters revealed that category dominance (like Electronics vs. Clothing) shifted drastically depending on the city.</p>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://github.com/Chiragsuri/Sales-Data-Analysis" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-brands fa-github"></i> View Full Repository
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/football-striker/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Prev: Striker Segments</a>
    <a href="/projects/house-sales-analysis/" class="nav-btn next-btn">Next: House Sales <span class="nav-arrow">&rarr;</span></a>
  </div>

</div>

<script>
window.addEventListener('load', () => {
  const counters = document.querySelectorAll(".counter");
  counters.forEach(counter => {
    const updateCount = () => {
      const target = +counter.getAttribute('data-target');
      const count = +counter.innerText;
      const inc = target / 150;
      if (count < target) {
        counter.innerText = Math.ceil(count + inc);
        setTimeout(updateCount, 15);
      } else {
        counter.innerText = target;
      }
    };
    updateCount();
  });

  const lightbox = document.createElement('div');
  lightbox.id = 'cs-lightbox';
  lightbox.className = 'cs-lightbox';
  document.body.appendChild(lightbox);

  document.querySelectorAll('.cs-showcase-img').forEach(image => {
    image.addEventListener('click', () => {
      lightbox.classList.add('active');
      while (lightbox.firstChild) lightbox.removeChild(lightbox.firstChild);
      const img = document.createElement('img');
      img.src = image.src;
      lightbox.appendChild(img);
    });
  });

  lightbox.addEventListener('click', () => lightbox.classList.remove('active'));
});
</script>
