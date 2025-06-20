---
permalink: /about/
layout: single
classes: wide
author_profile: true
---

<div class="page-header">
  <i class="fa-solid fa-address-card" style="color:rgb(156, 118, 12);"></i>
  <h1>About</h1>
</div>

<div class="links-grid">

  <a href="https://github.com/Chiragsuri" target="_blank" class="link-card">
    <i class="fa-brands fa-github"></i>
    GitHub
  </a>
  <a href="https://www.linkedin.com/in/chirag-suri/" target="_blank" class="link-card">
    <i class="fa-brands fa-linkedin"></i>
    LinkedIn
  </a>
  <a href="https://chiragsuri.github.io" target="_blank" class="link-card">
    <i class="fa-solid fa-globe"></i>
    Portfolio
  </a>
</div>

<div class="contact-section">
  <h2>📬 Contact Me</h2>
  <div class="contact-flex-box">
    <form id="contact-form" class="contact-form">
      <div class="form-group mb-3">
        <label for="name">👤 Your Name</label>
        <input type="text" name="from_name" id="name" class="form-control" required>
      </div>

      <div class="form-group mb-3">
        <label for="email">📧 Your Email</label>
        <input type="email" name="reply_to" id="email" class="form-control" required>
      </div>

      <div class="form-group mb-3">
        <label for="message">📝 Your Message</label>
        <textarea name="message" id="message" rows="4" class="form-control" required></textarea>
      </div>

      <button type="submit" class="send-btn">Send Message</button>
    </form>

  </div>

  <div id="form-toast" class="form-toast"></div>
</div>
