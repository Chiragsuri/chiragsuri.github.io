---
layout: single
author_profile: false
classes: wide
---

<div class="hero-wrapper">
  <div class="hero-split">
    <div class="hero-left reveal">
      <div class="hero-eyebrow">Data &middot; Analytics &middot; Consulting</div>
      <h1 class="hero-title">Hi, I'm Chirag.<br><span class="highlight">Data Strategist.</span></h1>
      <p class="hero-bio">I build the pipeline, find what matters inside it, and hand leadership something they can act on. The goal has always been consulting - which is just the same work with a seat at the table.</p>
      <div class="hero-action">
        <a href="#work" class="btn btn-primary">Latest Works</a>
        <a href="https://drive.google.com/file/d/YOUR_GOOGLE_DRIVE_ID" target="_blank" class="btn btn-outline">Download CV</a>
      </div>
    </div>
    
    <div class="hero-right reveal-stagger visible">
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

<div class="tech-stack reveal">
  <div class="tech-item"><i class="fa-brands fa-python"></i> Python</div>
  <div class="tech-item"><i class="fa-solid fa-database"></i> SQL</div>
  <div class="tech-item"><i class="fa-solid fa-chart-pie"></i> Power BI</div>
  <div class="tech-item"><i class="fa-solid fa-brain"></i> Predictive AI</div>
  <div class="tech-item"><i class="fa-solid fa-network-wired"></i> ETL Pipelines</div>
  <div class="tech-item"><i class="fa-solid fa-chart-line"></i> Statistical Modeling</div>
</div>

<div class="section" id="work">
  <div class="section-header reveal">
    <h2 class="section-title">Featured Work.</h2>
  </div>
  <div class="project-grid reveal">
    <a href="/shm/" class="project-card">
      <img src="/docs/assets/SHM_Dashboard1.png" alt="Retail Anomaly Detection">
      <div class="card-overlay">
        <h4>Retail Sales & Anomaly Detection</h4>
        <p>Cut query execution by 20% through pipeline engineering.</p>
      </div>
    </a>
    
    <a href="/ipl/" class="project-card">
      <img src="/docs/assets/IPLP1.png" alt="Performance Forecasting">
      <div class="card-overlay">
        <h4>Performance Forecasting</h4>
        <p>Automated 10+ KPIs across 145 datasets for executive reporting.</p>
      </div>
    </a>

    <a href="/football/" class="project-card">
      <img src="/docs/assets/FootballStriker.png" alt="Striker Segmentation">
      <div class="card-overlay">
        <h4>Football Striker Segmentation</h4>
        <p>Classified 500 player profiles using predictive K-Means modeling.</p>
      </div>
    </a>

  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", () => {
  // 1. IntersectionObserver for Scroll Reveal
  const revealObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('active');
        revealObserver.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });

  document.querySelectorAll('.reveal').forEach(el => revealObserver.observe(el));

  // 2. IntersectionObserver for Metric Count-Up Animation
  const countObserver = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        const el = entry.target;
        const target = parseFloat(el.getAttribute('data-target'));
        const suffix = el.getAttribute('data-suffix') || '';
        const duration = 1500; // Adjust speed here (1.5 seconds)
        let startTimestamp = null;

        const step = (timestamp) => {
          if (!startTimestamp) startTimestamp = timestamp;
          const progress = Math.min((timestamp - startTimestamp) / duration, 1);
          // easeOutQuart curve for natural deceleration
          const easeProgress = 1 - Math.pow(1 - progress, 4);
          const current = easeProgress * target;
          
          const isFloat = target % 1 !== 0;
          el.innerText = (isFloat ? current.toFixed(1) : Math.floor(current)) + suffix;

          if (progress < 1) {
            window.requestAnimationFrame(step);
          } else {
            el.innerText = target + suffix; // Ensure it ends exactly on target
          }
        };
        
        window.requestAnimationFrame(step);
        countObserver.unobserve(el);
      }
    });
  }, { threshold: 0.5 });

  document.querySelectorAll('.m-val').forEach(el => countObserver.observe(el));
});
</script>
