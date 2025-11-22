---
layout: default
title: About
permalink: /about/
---

<style>
  /* Layout container */
  .intro {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 30px;
    margin-top: 20px;
    margin-bottom: 40px;
  }

  .intro-text {
    flex: 1 1 380px;
    font-size: 1.05rem;
    line-height: 1.7;
  }

  .intro-image img {
    width: 200px;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 4px 14px rgba(0,0,0,0.12);
  }

  /* Papers section styling */
  .papers {
    margin-top: 20px;
  }

  .paper {
    margin-bottom: 18px;
    padding-bottom: 14px;
    border-bottom: 1px solid #eee;
  }

  .paper-title {
    font-weight: 600;
    font-size: 1.05rem;
  }

  .paper-authors {
    color: #555;
    margin-top: 2px;
  }

  .paper-meta {
    color: #777;
    font-size: 0.95rem;
    margin-top: 2px;
  }

  .paper-link {
    font-size: 0.92rem;
    color: #005fcc;
    text-decoration: none;
  }
  .paper-link:hover {
    text-decoration: underline;
  }

  /* Contact section */
  .contact a {
    color: #005fcc;
    text-decoration: none;
  }
  .contact a:hover {
    text-decoration: underline;
  }
</style>

<div class="intro">

  <div class="intro-text">
    I am a postdoctoral researcher under the supervision of 
    <strong>Prof. Jianhong Wu</strong> at York University, Canada.
    Before that, I completed my PhD under the supervision of 
    <strong>Prof. Xingfu Zou</strong> at the University of Western Ontario.
  </div>

  <div class="intro-image">
    <img src="/assets/images/profile.jpg" alt="Profile Photo">
  </div>

</div>

---

## 🎓 Research Interests

- Mathematical biology  
- Infectious disease modelling  
- Dynamical systems  
- Applied mathematics  

---

## 🎤 Presentations
<ul>
  <li><strong>Minisymposia Talk (Invited)</strong>, The Third Joint SIAM/CAIMS Annual Meetings (AN25), Montréal, Québec — July 28–August 1, 2025</li>
  <li><strong>Poster</strong>, Workshop on Mathematical Ecology 2025 — Phylodynamics, Queen’s University, Kingston — July 24–25, 2025</li>
  <li><strong>Minisymposia Talk</strong>, Society for Mathematical Biology Annual Meeting 2025, Edmonton, Canada — July 13–18, 2025</li>
  <li><strong>Poster Session</strong>, Modelling and Theory in Population Biology (NITMB) — Travel Award Recipient, Chicago, USA — June 2–6, 2025</li>
  <li><strong>Invited Talk</strong>, Workshop on Differential Equations and Mathematical Biology, University of Miami, Coral Gables — Nov 23–26, 2024</li>
  <li><strong>Talk</strong>, MfPH International Collaborative Summer Program in Nonlinear Differential Equations with Application, York University, Toronto — Aug 21, 2024</li>
  <li><strong>Minisymposia Talk</strong>, CAIMS Annual Meeting 2024, Queen’s University — June 24–27, 2024</li>
  <li><strong>Invited Talk</strong>, MathBio Seminar, University of Nebraska-Lincoln (Online) — Nov 2, 2023</li>
  <li><strong>Minisymposia Talk</strong>, Society for Mathematical Biology Annual Meeting 2023, Ohio State University — July 16–21, 2023</li>
  <li><strong>Poster Session</strong>, Advances in Mathematical Ecology 2023, University of Pittsburgh — June 1–3, 2023</li>
  <li><strong>Talk</strong>, CMS Scientific Session — Topics in Mathematical Biology, Toronto, Canada — Dec 2–5, 2022</li>
  <li><strong>Poster Session</strong>, Fields Workshop on Mathematical Ecology: Modeling Epidemics, Queen’s University, Canada — Aug 10–13, 2022</li>
  <li><strong>Group Presentation</strong>, Fields CQAM Thematic Program on Integrative Modeling of Emerging Infectious Disease Outbreaks, Canada — May–June 2021</li>
  <li><strong>Seminar Presentation</strong>, Dynamical Systems Seminar, Western University — Every academic term, Sept 2019–2024</li>
</ul>

---

## 📘 Selected Papers

<div class="papers">
{% for pub in site.data.publications %}
  <div class="paper">
    <div class="paper-title">{{ pub.title }}</div>
    <div class="paper-authors">{{ pub.authors }}</div>
    <div class="paper-meta">
      {% if pub.journal %}{{ pub.journal }}{% endif %}
      {% if pub.year %}, {{ pub.year }}{% endif %}
      {% if pub.DOI %}
        · <a href="https://doi.org/{{ pub.DOI }}" target="_blank">DOI</a>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

---

## 💻 Programming

<h2>Programming Projects</h2>
<p>
I use programming languages such as <strong>Mathematica</strong>, <strong>Python</strong>, and <strong>C++</strong>.
I have experience with <strong>MATLAB</strong> and <strong>MAPLE</strong>.
</p>

<p><a href="/">← Back to Home</a></p>
    <div class="paper-authors">{{ pub.authors }}</div>
    <div class="paper-meta">
      {% if pub.journal %}{{ pub.journal }}{% endif %}
      {% if pub.year %}, {{ pub.year }}{% endif %}
      {% if pub.DOI %}
        · <a href="https://doi.org/{{ pub.DOI }}" target="_blank">DOI</a>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

---

## 📬 Contact

<div class="contact">
  ✉️ <strong>Email:</strong><br>
  <a href="mailto:tianyu45@yorku.ca">tianyu45@yorku.ca</a><br>
  <a href="mailto:tchen454@uwo.ca">tchen454@uwo.ca</a>
</div>
