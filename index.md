---
layout: default
title: Tianyu Cheng
permalink: /
---

<style>
  body {
    background-image: url('/assets/images/background.jpg');
    background-size: cover;
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-position: center;
  }

  body::before {
    content: "";
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(255, 255, 255, 0.65);
    z-index: -1;
  }

  .header {
    text-align: center;
    margin-top: 40px;
    margin-bottom: 30px;
  }

  .header h1 {
    font-size: 2.4rem;
    margin-bottom: 5px;
  }

  .subtitle {
    font-size: 1.15rem;
    color: #666;
    font-weight: 300;
  }

  .content {
    max-width: 760px;
    margin: auto;
    line-height: 1.75;
    font-size: 1.06rem;
    color: #333;
  }

  section {
    margin-bottom: 42px;
  }

  .navigation ul {
    list-style: none;
    padding-left: 0;
  }

  .navigation li {
    margin-bottom: 12px;
    font-size: 1.12rem;
  }

  .navigation a:hover {
    color: #005fcc;
  }

  .contact a {
    color: #005fcc;
    text-decoration: none;
  }

  .contact a:hover {
    text-decoration: underline;
  }
</style>

<div class="header">
  <h1>Tianyu Cheng</h1>
  <p class="subtitle">Postdoctoral Researcher · York University</p>
</div>

<div class="content">

  <!-- Contact Section -->
  <section class="contact">
    <h2>Contact</h2>
    <p>
      ✉️ <strong>Primary:</strong> 
      <a href="mailto:{{ site.email }}">{{ site.email }}</a>
    </p>
    <p>
      📮 <strong>Secondary:</strong> 
      <a href="mailto:your.second.email@example.com">your.second.email@example.com</a>
    </p>
  </section>

</div>
