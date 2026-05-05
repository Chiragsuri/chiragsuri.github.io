---
title: "Geospatial Real Estate Valuation"
permalink: /projects/house-sales-analysis/
layout: single
author_profile: false
classes: wide
header: false
share: false
---

<a href="/projects/sales-data-analysis/" class="side-nav-btn prev-btn-floating" title="Previous Project"><i class="fa-solid fa-chevron-left"></i></a>
<a href="/projects/" class="side-nav-btn next-btn-floating" title="Project Archive"><i class="fa-solid fa-chevron-right"></i></a>

<div class="case-study-container reveal active" style="padding-bottom: 4rem;">

<span class="cs-eyebrow">Analytics · Tableau</span>

  <h1 class="cs-title">Geospatial Real Estate<br>Valuation</h1>
  <p class="cs-subtitle">A dynamic geographic mapping tool for King County housing records. This dashboard filters property valuations by condition and build year to show exactly how much location changes market prices.</p>

  <div class="cs-brief-grid" style="margin-bottom: 2rem;">
    <div class="cs-brief-context">
      <p>Real estate pricing is notoriously difficult to visualize in a spreadsheet. I took raw housing records from King County, Washington, cleaned them in Excel, and normalized them into a dynamic Tableau map. This allows users to visually filter properties by condition, square footage, and build year to instantly see neighborhood pricing ceilings and spatial market trends.</p>
    </div>
    <div class="cs-brief-meta">
      <h4>Tech Stack</h4>
      <div class="cs-tech-tags">
        <span class="cs-tech-tag">Tableau</span>
        <span class="cs-tech-tag">Excel</span>
        <span class="cs-tech-tag">Geospatial Mapping</span>
      </div>
    </div>
  </div>

  <div class="cs-image-grid" style="grid-template-columns: 1fr; margin-top: 4rem;">
    <div class="cs-showcase-item">
      <img src="/docs/assets/HouseSales.png" alt="Geospatial Real Estate Valuation Dashboard" class="cs-showcase-img">
      <div class="cs-showcase-caption">Interactive Tableau Map: Filtering King County property valuations by location and condition.</div>
    </div>
  </div>

  <div style="display: flex; justify-content: center; margin: 4rem 0;">
    <a href="https://public.tableau.com/app/profile/chirag.suri/viz/KingCountyHouseSales_16953115471270/KingCountyHouseSales" target="_blank" class="btn btn-primary" style="padding: 16px 36px;">
      <i class="fa-solid fa-chart-line"></i> View Live Dashboard
    </a>
  </div>

  <div class="projects-page-nav" markdown="0">
    <a href="/projects/sales-data-analysis/" class="nav-btn prev-btn"><span class="nav-arrow">&larr;</span> Prev: YoY Sales</a>
    <a href="/projects/" class="nav-btn next-btn">Project's Archive <span class="nav-arrow">&rarr;</span></a>
  </div>

</div>

<script>
window.addEventListener('load', () => {
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
