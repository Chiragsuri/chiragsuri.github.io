---
title: "Retail Revenue & Anomaly Detection"
permalink: /projects/sales-health-monitor/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Engineering · BI</span>

  <h1 class="cs-title">Retail Revenue &<br>Anomaly Detection</h1>
  <p class="cs-subtitle">An end-to-end analytics pipeline that transforms raw transaction logs into strategic insights. I engineered a custom anomaly detection model that reduced false alerts by 85%, and delivered a comprehensive executive dashboard that empowers leadership with immediate, self-serve reporting.</p>

  <div class="cs-metrics-strip">
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="800">0</span>K+</span>
      <span class="cs-metric-label">Records Processed</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="85">0</span>%</span>
      <span class="cs-metric-label">False Alert Reduction</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="100">0</span>%</span>
      <span class="cs-metric-label">Automated Pipeline</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="4">0</span></span>
      <span class="cs-metric-label">Dashboard Pages</span>
    </div>
  </div>

  <div class="cs-brief-grid">
    <div class="cs-brief-context">
      <p>Retail operations generate noise faster than humans can filter it. The business was processing millions of transactions without a reliable way to separate critical performance drops from standard seasonal variance. I needed an automated intelligence layer that didn't just visualize data, but actively told leadership exactly where to focus their attention.</p>
    </div>
    <div class="cs-brief-meta">
      <h4>Tech Stack</h4>
      <div class="cs-tech-tags">
        <span class="cs-tech-tag">MySQL</span>
        <span class="cs-tech-tag">Python</span>
        <span class="cs-tech-tag">Pandas</span>
        <span class="cs-tech-tag">Power BI</span>
        <span class="cs-tech-tag">DAX</span>
      </div>
    </div>
  </div>

  <h2 class="cs-section-label">The Methodology</h2>

  <div class="cs-approach-grid">
    <div class="cs-approach-card">
      <i class="fa-solid fa-server cs-approach-icon"></i>
      <h3>1. Data Generation & Architecture</h3>
      <p>Simulated a realistic retail dataset (50,000 customers, 500 products). Cleaned the intentionally messy data via Python, then engineered a robust MySQL Star Schema with 11 distinct analytical views to eliminate BI bottlenecks.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-microchip cs-approach-icon"></i>
      <h3>2. Adaptive Anomaly Detection</h3>
      <p>Replaced rigid monitoring with a dynamic, percentile-based statistical model built entirely in SQL. This engine adapted automatically to Nov-Jan volume spikes, dropping false failure alerts from over 10,000 down to 1,524.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-chart-line cs-approach-icon"></i>
      <h3>3. Executive BI</h3>
      <p>Developed four interactive Power BI reporting pages powered by custom DAX time-intelligence functions. The views successfully mapped complex RFM customer segmentation into an intuitive visual format for regional managers.</p>
    </div>
  </div>

  <h2 class="cs-section-label">The Deliverables</h2>

  <div class="cs-image-grid">
    <div class="cs-showcase-item">
      <img src="/docs/assets/SHM_Dashboard1.png" alt="Executive Dashboard" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 1: Revenue trends, YoY comparisons, and top-performer rankings.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/SHM_Dashboard2.png" alt="Anomaly Monitor" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 2: The Anomaly & Risk Monitor, tracking abnormal product behavior.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/SHM_Dashboard3.png" alt="Customer Intelligence" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 3: Customer Intelligence, RFM segmentation, and lifetime value tracking.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/SHM_Dashboard4.png" alt="Geographic Performance" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 4: Geographic Performance, mapping regional growth and product matrices.</div>
    </div>
  </div>

  <h2 class="cs-section-label">Key Findings & Future Scope</h2>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">20% of customers drive 32% of total revenue.</h3>
    <p class="cs-finding-context">RFM segmentation revealed that a fraction of the customer base was disproportionately responsible for high-margin sales, allowing marketing to pivot retention strategies effectively.</p>
  </div>

  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Next Steps: AI & Automation.</h3>
    <p class="cs-finding-context">The pipeline currently relies on SQL-based statistical anomalies. The next iteration of this project will integrate Scikit-learn for ML-based predictive anomaly detection, alongside an automated alerting system that triggers emails directly to regional directors when a KPI drops.</p>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://github.com/Chiragsuri/Sales_Health_Monitor" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-brands fa-github"></i> View Full Repository
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Archive</a>
    <a href="/projects/ipl-analysis/" class="nav-btn next-btn">Next: Forecasting Model <span class="nav-arrow">&rarr;</span></a>
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
