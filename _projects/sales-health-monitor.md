---
title: "Retail Revenue & Anomaly Detection"
permalink: /projects/sales-health-monitor/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/" class="side-nav-btn prev-btn-floating" title="Project Archive"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/ipl-analysis/" class="side-nav-btn next-btn-floating" title="Next Project"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Engineering · BI</span>

  <h1 class="cs-title">Retail Revenue &<br>Anomaly Detection</h1>
  <p class="cs-subtitle">An analytics pipeline that turns raw transaction logs into plain answers. I built an anomaly detection model that cut false alerts by 85% and gave leadership a dashboard they can actually use themselves.</p>

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
      <p>Retail generates noise faster than humans can filter it. The business was processing millions of transactions but couldn't separate a real performance drop from a normal seasonal dip. They needed an automated layer that didn't just draw charts, but told them exactly where to look.</p>
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
      <p>Simulated a retail dataset with 50,000 customers and 500 products. I cleaned the intentionally messy data in Python, then built a MySQL Star Schema with 11 views so the BI tools wouldn't bottleneck.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-microchip cs-approach-icon"></i>
      <h3>2. Adaptive Anomaly Detection</h3>
      <p>I replaced their rigid alerts with a dynamic, percentile-based model built entirely in SQL. It adapted automatically to the holiday volume spikes, bringing false alarms down from over 10,000 to just 1,524.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-chart-line cs-approach-icon"></i>
      <h3>3. Executive BI</h3>
      <p>Built four Power BI pages using custom DAX time-intelligence functions. It mapped out complex RFM customer segmentation into something regional managers could understand at a glance.</p>
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
    <p class="cs-finding-context">RFM segmentation showed that a tiny fraction of the customer base drove almost all the high-margin sales. This let the marketing team completely change how they handled retention.</p>
  </div>

  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Next Steps: AI & Automation.</h3>
    <p class="cs-finding-context">Right now, the pipeline relies on SQL statistical anomalies. Next, I'm integrating Scikit-learn to do predictive anomaly detection, plus an alerting system that emails regional directors the second a KPI drops.</p>
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
