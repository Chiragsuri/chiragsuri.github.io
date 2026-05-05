---
title: "Performance Forecasting Model"
permalink: /projects/ipl-analysis/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/sales-health-monitor/" class="side-nav-btn prev-btn-floating" title="Previous Project"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/football-striker/" class="side-nav-btn next-btn-floating" title="Next Project"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active">

<span class="cs-eyebrow">Analytics · Strategy</span>

  <h1 class="cs-title">Performance Forecasting<br>Model</h1>
  <p class="cs-subtitle">I built an end-to-end sports analytics engine to see if data could explain match outcomes better than basic cricket intuition. By chewing through two seasons of ball-by-ball logs, this dashboard strips away the noise to highlight the tactical decisions that actually win games.</p>

  <div class="cs-metrics-strip">
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="145">0</span></span>
      <span class="cs-metric-label">Datasets Processed</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="10">0</span>+</span>
      <span class="cs-metric-label">KPIs Tracked</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="2">0</span></span>
      <span class="cs-metric-label">Seasons Analyzed</span>
    </div>
    <div class="cs-metric">
      <span class="cs-metric-val"><span class="counter" data-target="4">0</span></span>
      <span class="cs-metric-label">Dashboard Pages</span>
    </div>
  </div>

  <div class="cs-brief-grid">
    <div class="cs-brief-context">
      <p>Most cricket analysis stops at batting averages and win rates. That's boring. I wanted to know if winning the toss actually matters, or what specific target score forces a batting collapse. To get there, I had to wrangle massive event logs into something a strategist could actually read at a glance without getting lost in the numbers.</p>
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
      <h3>1. Data Engineering</h3>
      <p>I pulled the raw ball-by-ball data and filtered it down to the 2024 and 2025 seasons using MySQL. I stripped out cancelled matches and playoff anomalies to build three clean reporting tables.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-microchip cs-approach-icon"></i>
      <h3>2. Exploratory Analysis</h3>
      <p>Before building anything visual, I used Python to map the terrain. This is where the real story emerged-like seeing the exact dot-ball volume required to choke a run chase.</p>
    </div>
    <div class="cs-approach-card">
      <i class="fa-solid fa-chart-line cs-approach-icon"></i>
      <h3>3. Executive BI</h3>
      <p>I built a four-page Power BI dashboard. Instead of relying on static charts, I used dynamic DAX functions so a user can slice the data by team or venue without breaking the views.</p>
    </div>
  </div>

  <h2 class="cs-section-label">The Deliverables</h2>

  <div class="cs-image-grid">
    <div class="cs-showcase-item">
      <img src="/docs/assets/IPLP1.png" alt="Tournament Overview" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 1: Tournament Overview, mapping team venues and toss-winner impact.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/IPLP2.png" alt="Team Performance" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 2: Team Performance, tracking boundary hits, dot ball flow, and fielding stats.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/IPLP3.png" alt="Player Intelligence" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 3: Player Intelligence, highlighting top run scorers and wicket takers.</div>
    </div>
    <div class="cs-showcase-item">
      <img src="/docs/assets/IPLP4.png" alt="Match Behaviour" class="cs-showcase-img">
      <div class="cs-showcase-caption">Dashboard 4: Match Behaviour, analyzing DRS review success and target score distributions.</div>
    </div>
  </div>

  <h2 class="cs-section-label">Key Findings</h2>

  <div class="cs-finding">
    <h3 class="cs-finding-stat">Toss wins don't equal match wins.</h3>
    <p class="cs-finding-context">Everyone assumes the toss dictates the game. The data proves it doesn't. Execution, specifically maintaining a high dot-ball percentage, correlates much stronger with a victory than winning the coin flip.</p>
  </div>
  
  <div class="cs-finding">
    <h3 class="cs-finding-stat">200 is the new normal.</h3>
    <p class="cs-finding-context">The run environment has shifted heavily. Teams routinely chased targets over 200, which entirely changes how middle-order batters have to pace their innings.</p>
  </div>

  <div class="cs-finding" style="margin-top: 2rem;">
    <h3 class="cs-finding-stat">Next Steps: Predictive modeling.</h3>
    <p class="cs-finding-context">Right now, this dashboard looks backward. My next move is wiring up Scikit-learn to predict match outcomes live based on real-time stadium metrics.</p>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://github.com/Chiragsuri/IPL_Analysis" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-brands fa-github"></i> View Full Repository
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/sales-health-monitor/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Prev: Retail Revenue</a>
    <a href="/projects/football-striker/" class="nav-btn next-btn">Next: Striker Segments <span class="nav-arrow">&rarr;</span></a>
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
