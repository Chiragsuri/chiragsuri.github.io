---
title: "Football Striker Segmentation"
permalink: /projects/football-striker/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/ipl-analysis/" class="side-nav-btn prev-btn-floating" title="Previous Project"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/sales-data-analysis/" class="side-nav-btn next-btn-floating" title="Next Project"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Machine Learning · Python</span>

  <h1 class="cs-title">Football Striker<br>Segmentation</h1>
  <p class="cs-subtitle">A machine learning model built to isolate exactly what makes a striker elite. I used K-Means clustering and logistic regression to turn 500 players' raw stats into a predictive classification system.</p>

  <div class="cs-metrics-strip">
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="500">0</span></span>
      <span class="cs-metric-label">Players Analyzed</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="2">0</span></span>
      <span class="cs-metric-label">Performance Tiers</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="212">0</span></span>
      <span class="cs-metric-label">Elite Base Score</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="73">0</span>%</span>
      <span class="cs-metric-label">Right-Footed Bias</span>
    </div>
  </div>

  <div class="cs-brief-grid">
    <div class="cs-brief-context">
      <p>Scouting a striker usually stops at looking at how many goals they scored last season. That's a flawed metric. I wanted to see if statistical modeling could strip away the bias. By clustering 500 players based on secondary metrics like hold-up play and passing consistency, I built a classification system that predicts future performance instead of just rewarding past luck.</p>
    </div>
    <div class="cs-brief-meta">
      <h4>Tech Stack</h4>
      <div class="cs-tech-tags">
        <span class="cs-tech-tag">Python</span>
        <span class="cs-tech-tag">Scikit-Learn</span>
        <span class="cs-tech-tag">Pandas</span>
        <span class="cs-tech-tag">SciPy</span>
        <span class="cs-tech-tag">Seaborn</span>
      </div>
    </div>
  </div>

  <h2 class="cs-section-label">The Methodology</h2>

  <div class="cs-approach-grid">
    <div class="cs-approach-card">
      <i class="fa-solid fa-flask cs-approach-icon"></i>
      <h3>1. Statistical Validation</h3>
      <p>You can't just throw data at an algorithm and hope for the best. I ran Shapiro-Wilk and Levene's tests first to validate the distributions. I proved mathematically that a trait like "hold-up play" heavily correlates with long-term consistency.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-code-branch cs-approach-icon"></i>
      <h3>2. Feature Engineering</h3>
      <p>Raw stats are too noisy. I engineered a custom "Total Contribution Score" that weighted goals, assists, and dribbles into a single, clean metric. This gave the clustering algorithm a much sharper signal to process.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-brain cs-approach-icon"></i>
      <h3>3. Clustering & Classification</h3>
      <p>I deployed K-Means to naturally divide the 500 strikers into two distinct tiers: Elite and Regular. From there, I trained a Logistic Regression model to accurately classify any new player into these buckets based on their stats.</p>
    </div>
  </div>

  <h2 class="cs-section-label">The Deliverables</h2>

  <div class="cs-image-grid" style="grid-template-columns: 1fr;">
    <div class="cs-showcase-item">
      <img src="/docs/assets/FootballStriker.png" alt="Football Striker Segmentation Visuals" class="cs-showcase-img">
      <div class="cs-showcase-caption">Statistical distributions, clustering results, and performance mappings isolating the elite tier.</div>
    </div>
  </div>

  <h2 class="cs-section-label">Key Findings</h2>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">Hold-up play is the hidden engine.</h3>
    <p class="cs-finding-context">The regression model proved that a striker's hold-up play is a massive predictor of their overall consistency (a 0.55 correlation). It isn't just about shooting; it's about keeping the possession alive in the final third.</p>
  </div>
  
  <div class="cs-finding">
    <h3 class="cs-finding-stat">The math defines the elite.</h3>
    <p class="cs-finding-context">The K-Means algorithm naturally found the breakpoint without human bias. The "Elite" strikers clustered tightly around an average contribution score of 212. The logistic regression model easily learned this threshold and classified players with high accuracy.</p>
  </div>

  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Next Steps: A scouting dashboard.</h3>
    <p class="cs-finding-context">Jupyter notebooks are great for data scientists, but terrible for football coaches. My next step is wiring this Python model into an interactive Power BI dashboard so scouts can drag sliders and interact with the predictions visually.</p>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://github.com/Chiragsuri/Football-Striker-Performance" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-brands fa-github"></i> View Full Repository
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/ipl-analysis/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Prev: Forecasting Model</a>
    <a href="/projects/sales-data-analysis/" class="nav-btn next-btn">Next: YoY Sales Analytics <span class="nav-arrow">&rarr;</span></a>
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
