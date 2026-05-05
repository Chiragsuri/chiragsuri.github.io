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
  <p class="cs-subtitle">A star schema across 800K+ records, an anomaly detection layer that cut false alerts by 85%, and a four-page executive dashboard built so leadership stops asking for one-off reports.</p>

  <!-- The New Professional Tech Grid -->
  <div class="cs-exec-summary">
    <div class="cs-exec-item">
      <span class="cs-exec-label">Database</span>
      <span class="cs-exec-value">MySQL (Star Schema)</span>
    </div>
    <div class="cs-exec-item">
      <span class="cs-exec-label">Logic Layer</span>
      <span class="cs-exec-value">Python (Pandas, NumPy)</span>
    </div>
    <div class="cs-exec-item">
      <span class="cs-exec-label">Visualization</span>
      <span class="cs-exec-value">Power BI</span>
    </div>
    <div class="cs-exec-item">
      <span class="cs-exec-label">Key Technique</span>
      <span class="cs-exec-value">DAX Time Intelligence</span>
    </div>
  </div>

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

  <div class="cs-approach-row" style="margin-top: 2rem; border-top: none;">
    <div class="cs-approach-phase">The Context</div>
    <p class="cs-approach-desc">Retail operations at this scale generate noise faster than humans can filter it. The business was processing millions of transactions with no reliable way to distinguish critical performance drops from standard seasonal variance. I was tasked with engineering an automated intelligence layer that didn't just visualize data, but actively identified where leadership needed to focus their attention.</p>
  </div>

  <div class="cs-approach-row">
    <div class="cs-approach-phase">Phase 01<br>Data Architecture</div>
    <p class="cs-approach-desc">Engineered a scalable MySQL Star Schema comprising one central fact table and three dimension tables. Layered 11 distinct analytical views on top to handle pre-aggregations, removing query bottlenecks for BI ingestion.</p>
  </div>
  
  <div class="cs-approach-row">
    <div class="cs-approach-phase">Phase 02<br>Anomaly Detection</div>
    <p class="cs-approach-desc">Replaced rigid static thresholds with a dynamic, percentile-based statistical model using advanced SQL. This allowed the system to adapt automatically to massive seasonal volume spikes (like Nov-Jan rushes) without triggering false failures.</p>
  </div>
  
  <div class="cs-approach-row">
    <div class="cs-approach-phase">Phase 03<br>Executive BI</div>
    <p class="cs-approach-desc">Developed four interactive Power BI reporting pages using dynamic DAX time-intelligence functions, mapping complex RFM customer segmentation into an intuitive visual format for regional managers.</p>
  </div>

  <div class="cs-section-label" style="margin-top: 3rem;">The Dashboards</div>

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

  <div class="cs-section-label">Key Findings</div>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">20% of customers drive 32% of total revenue.</h3>
    <p class="cs-finding-context">RFM segmentation revealed that a fraction of the customer base was disproportionately responsible for high-margin sales, allowing marketing to pivot retention strategies.</p>
  </div>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">Holiday peaks average 150% above the baseline.</h3>
    <p class="cs-finding-context">Temporal analysis identified a massive spike spanning Nov-Jan, validating the need for the dynamic anomaly thresholds implemented in Phase 2.</p>
  </div>

  <div class="cs-links">
    <a href="https://github.com/Chiragsuri/Sales_Health_Monitor" target="_blank" class="btn btn-primary">
      <i class="fa-brands fa-github"></i> View Repository
    </a>
  </div>

  <div class="projects-page-nav">
    <a href="/projects/">← Archive</a>
  </div>

</div>

<!-- Number Counters & Image Lightbox -->
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
