---
layout: single
author_profile: false
classes: wide
---

<div class="hero-wrapper">
  <div class="hero-split">
    <div class="hero-left reveal">
      <div class="hero-eyebrow">Data &middot; Analytics &middot; Consulting</div>
      <h1 class="hero-title">Hi, I'm Chirag<br><span class="highlight">Data Strategist</span></h1>
      <p class="hero-bio">I build data pipelines, find what actually matters, and give leadership clear answers. Consulting is just doing this with a seat at the table.</p>
      <div class="hero-action">
        <a href="/projects/" class="btn btn-primary">Latest Works</a>
        <a href="https://drive.google.com/file/d/YOUR_GOOGLE_DRIVE_ID" target="_blank" class="btn btn-outline">Download CV</a>
      </div>
    </div>
    
    <div class="hero-right">
      <div class="image-fade-left"></div>
      <div class="image-fade-bottom"></div>
      <img src="/docs/assets/Chirag_frontpage.png" alt="Chirag Suri Portrait">
    </div>
  </div>

  <div class="scroll-indicator">
    <span>Scroll to explore</span>
    <div class="scroll-line"></div>
  </div>
</div>

<div class="metrics-bar reveal">
  <div class="metric">
    <span class="m-val" data-target="40" data-suffix="%">0%</span>
    <span class="m-label">Faster Data Retrieval</span>
  </div>
  <div class="m-divider"></div>
  <div class="metric">
    <span class="m-val" data-target="85" data-suffix="%">0%</span>
    <span class="m-label">False Alert Reduction</span>
  </div>
  <div class="m-divider"></div>
  <div class="metric">
    <span class="m-val" data-target="96.06" data-suffix="%">0%</span>
    <span class="m-label">CAT 2024 (Top 4%)</span>
  </div>
</div>

<div class="section">
  <h2 class="section-title reveal" style="margin-bottom: 1rem;">Core Expertise</h2>
  <div class="expertise-section reveal">
    
    <div class="expertise-row">
      <div class="expertise-title">
        <span class="exp-num">01</span>
        <h3>Data Engineering</h3>
      </div>
      <div class="expertise-skills">
        <span class="expertise-pill">SQL & Optimization</span>
        <span class="expertise-pill">ETL Pipelines</span>
        <span class="expertise-pill">Star / Snowflake Schema</span>
        <span class="expertise-pill">Quality Frameworks</span>
      </div>
    </div>

    <div class="expertise-row">
      <div class="expertise-title">
        <span class="exp-num">02</span>
        <h3>Analytics & BI</h3>
      </div>
      <div class="expertise-skills">
        <span class="expertise-pill">Python (Pandas, NumPy)</span>
        <span class="expertise-pill">Power BI & DAX</span>
        <span class="expertise-pill">Tableau</span>
        <span class="expertise-pill">Advanced Excel</span>
      </div>
    </div>

    <div class="expertise-row">
      <div class="expertise-title">
        <span class="exp-num">03</span>
        <h3>Strategy & Modeling</h3>
      </div>
      <div class="expertise-skills">
        <span class="expertise-pill">Predictive AI (Scikit-learn)</span>
        <span class="expertise-pill">Hypothesis Testing</span>
        <span class="expertise-pill">KPI Development</span>
        <span class="expertise-pill">Cohort Analysis</span>
      </div>
    </div>

  </div>
</div>

<div class="section" id="work">
  <h2 class="section-title reveal">Case Studies</h2>
  
  <div class="project-showcase reveal">
    <a href="/projects/sales-health-monitor/" class="project-visual">
      <div class="card-slider">
        <img src="/docs/assets/SHM_Dashboard1.png" alt="Executive Overview">
        <img src="/docs/assets/SHM_Dashboard2.png" alt="Anomaly & Risk Monitor">
        <img src="/docs/assets/SHM_Dashboard3.png" alt="Customer Intelligence">
        <img src="/docs/assets/SHM_Dashboard4.png" alt="Geographic Performance">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Engineering &middot; BI</div>
      <h3 class="project-name">Retail Revenue & Anomaly Detection</h3>
      <p class="project-desc">Processed 800K+ records and cut false alerts by 85%. The dashboard shows exactly where revenue is coming from.</p>
      <a href="/projects/sales-health-monitor/" class="project-link">Read Case Study &rarr;</a>
    </div>
  </div>

  <div class="project-showcase reverse reveal">
    <a href="/projects/ipl-analysis/" class="project-visual">
      <div class="card-slider">
        <img src="/docs/assets/IPLP1.png" alt="IPL Overview">
        <img src="/docs/assets/IPLP2.png" alt="Team Performance">
        <img src="/docs/assets/IPLP3.png" alt="Players Performance">
        <img src="/docs/assets/IPLP4.png" alt="Match Flow">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Analytics &middot; SQL</div>
      <h3 class="project-name">Performance Forecasting Model</h3>
      <p class="project-desc">Tracked over 10 KPIs across 145 datasets to figure out what actually wins matches.</p>
      <a href="/projects/ipl-analysis/" class="project-link">Read Case Study &rarr;</a>
    </div>
  </div>

  <div class="project-showcase reveal">
    <a href="/projects/football-striker/" class="project-visual">
      <div class="card-slider">
        <img src="/docs/assets/FootballStriker.png" alt="Striker Dashboard">
      </div>
    </a>
    <div class="project-info">
      <div class="project-meta">Machine Learning &middot; Python</div>
      <h3 class="project-name">Football Striker Segmentation</h3>
      <p class="project-desc">Clustered 500 elite players using K-Means to find out what really drives goal-scoring.</p>
      <a href="/projects/football-striker/" class="project-link">Read Case Study &rarr;</a>
    </div>
  </div>
  
  <div class="archive-cta reveal">
    <p>Three projects. More in the archive.</p>
    <a href="/projects/" class="btn btn-outline archive-btn">Explore Full Archive</a>
  </div>
</div>

<div class="pre-footer-cta reveal">
  <h2>Let's talk.</h2>
  <p>I'm looking for full-time roles in analytics and consulting.</p>
  <a href="mailto:chiragsuri.in@gmail.com" class="btn btn-primary">Get in Touch &rarr;</a>
</div>

<script>
document.addEventListener("DOMContentLoaded", () => {
  // Reveal Animations
  const revealObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('active');
        revealObserver.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });
  document.querySelectorAll('.reveal').forEach(el => revealObserver.observe(el));

  // Number Counters
  const countObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        const el = entry.target;
        const target = parseFloat(el.getAttribute('data-target'));
        const suffix = el.getAttribute('data-suffix') || '';
        const duration = 1500;
        let startTimestamp = null;
        const step = (timestamp) => {
          if (!startTimestamp) startTimestamp = timestamp;
          const progress = Math.min((timestamp - startTimestamp) / duration, 1);
          const current = (1 - Math.pow(1 - progress, 4)) * target;
          const isFloat = target % 1 !== 0;
          el.innerText = (isFloat ? current.toFixed(2) : Math.floor(current)) + suffix;
          if (progress < 1) window.requestAnimationFrame(step);
          else el.innerText = target + suffix;
        };
        window.requestAnimationFrame(step);
        countObserver.unobserve(el);
      }
    });
  }, { threshold: 0.5 });
  document.querySelectorAll('.m-val').forEach(el => countObserver.observe(el));

  // Dynamic Image Fader
  document.querySelectorAll('.card-slider').forEach(slider => {
    const images = slider.querySelectorAll('img');
    if (images.length <= 1) return;
    
    images.forEach((img, i) => { img.style.opacity = i === 0 ? '1' : '0'; });
    let currentIndex = 0;
    
    setInterval(() => {
      images[currentIndex].style.opacity = '0'; 
      currentIndex = (currentIndex + 1) % images.length; 
      images[currentIndex].style.opacity = '1'; 
    }, 3500); 
  });
});
</script>
