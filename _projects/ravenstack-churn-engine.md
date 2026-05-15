---
title: "RavenStack Churn Decision Engine"
permalink: /projects/ravenstack-churn-engine/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/" class="side-nav-btn prev-btn-floating" title="Project Archive"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/sales-health-monitor/" class="side-nav-btn next-btn-floating" title="Next Project"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Machine Learning · Data Engineering</span>

  <h1 class="cs-title">Customer Churn &<br>Retention Engine</h1>
  <p class="cs-subtitle">RavenStack wrapped up its pilot phase with ~500 accounts and a massive churn problem. I built an end-to-end ML pipeline that flags at-risk accounts 30 days before renewal so Customer Success knows exactly who to call and why.</p>

  <div class="cs-metrics-strip">
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="64">0</span>%</span>
      <span class="cs-metric-label">Baseline Recall</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val">$<span class="counter" data-target="870">0</span>K</span>
      <span class="cs-metric-label">At-Risk MRR Flagged</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="146">0</span></span>
      <span class="cs-metric-label">Urgent Interventions</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="30">0</span></span>
      <span class="cs-metric-label">Day Warning Window</span>
    </div>
  </div>

  <div class="cs-brief-grid">
    <div class="cs-brief-context">
      <p>The goal wasn't just to model historical churn in a notebook. It was to build something a Customer Success Manager could open in the morning and act on. I built an end-to-end pipeline connecting Google BigQuery, an XGBoost classification model, and a live Power BI dashboard to make that happen without relying on static spreadsheets.</p>
    </div>
    <div class="cs-brief-meta">
      <h4>Tech Stack</h4>
      <div class="cs-tech-tags">
        <span class="cs-tech-tag">BigQuery</span>
        <span class="cs-tech-tag">XGBoost</span>
        <span class="cs-tech-tag">SHAP</span>
        <span class="cs-tech-tag">Python</span>
        <span class="cs-tech-tag">Power BI</span>
      </div>
    </div>
  </div>

  <h2 class="cs-section-label">The Methodology</h2>

  <div class="cs-approach-grid">
    <div class="cs-approach-card">
      <i class="fa-solid fa-database cs-approach-icon"></i>
      <h3>1. Data Warehousing</h3>
      <p>I engineered a SQL pipeline in BigQuery that ingests five normalized tables. I used window functions to calculate complex behavioral features like inactivity, support friction, and satisfaction trends anchored to the dataset timeline.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-brain cs-approach-icon"></i>
      <h3>2. Predictive Modeling</h3>
      <p>Missing a churner costs MRR, but sending a false alert just costs a 15-minute phone call. I applied scale_pos_weight to handle the severe class imbalance and aggressively optimized the XGBoost classifier for Recall.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-chart-pie cs-approach-icon"></i>
      <h3>3. Live Decision Engine</h3>
      <p>The model writes its predictions and SHAP explainability scores back to BigQuery. Power BI queries this live, mapping out a dynamic waterfall chart so a CSM can see exactly what behavioral metrics are pushing an account to cancel.</p>
    </div>
  </div>

  <h2 class="cs-section-label">The Deliverables</h2>

  <div class="cs-image-grid">
    <div class="cs-showcase-item">
      <img src="/docs/assets/RavenStack_Page1.png" alt="Executive Summary" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 1: Executive Summary tracking Net Revenue Churn and Gross Logo Churn.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/RavenStack_Page2.png" alt="CSM Action Board" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 2a: The CSM Action Board, highlighting accounts renewing in 30 days.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/RavenStack_Page3.png" alt="Action Board Filtered" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 2b: Selecting an account dynamically updates the SHAP waterfall, revealing exact churn drivers.</div>
    </div>
  </div>

  <h2 class="cs-section-label">Key Findings</h2>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">Inactivity dominates everything.</h3>
    <p class="cs-finding-context">Days since last usage consistently has the highest absolute SHAP values. An account that hasn't logged in for months is going to churn, period. CSAT surveys and support ticket resolution won't save them at that point.</p>
  </div>

  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">$503K at risk from "happy" customers.</h3>
    <p class="cs-finding-context">Accounts with high satisfaction scores (4–5) contributed over half a million dollars in at-risk MRR. Satisfaction scores are a lagging indicator; a high score just means a support interaction went well, not that the account is healthy.</p>
  </div>
  
  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Churn is behavioral, not plan-driven.</h3>
    <p class="cs-finding-context">Enterprise customers churned at nearly the exact same rate as Basic customers. Upgrading accounts to higher tiers does not meaningfully reduce churn risk if the core engagement isn't there.</p>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://github.com/Chiragsuri/saas-churn-retention-engine" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-brands fa-github"></i> View Full Repository
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Archive</a>
    <a href="/projects/sales-health-monitor/" class="nav-btn next-btn">Next: Retail Revenue <span class="nav-arrow">&rarr;</span></a>
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
