---
layout: default
title: About
permalink: /about/
---

<style>
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
  .papers { margin-top: 20px; }
  .paper { margin-bottom: 18px; padding-bottom: 14px; border-bottom: 1px solid #74a9d2ff; }
  .paper-title { font-weight: 600; font-size: 1.05rem; }
  .paper-authors { color: #555; margin-top: 2px; }
  .paper-meta { color: #777; font-size: 0.95rem; margin-top: 2px; }
  .contact a { color: #005fcc; text-decoration: none; }
  .contact a:hover { text-decoration: underline; }
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



## 📘 Selected Papers
<div class="papers">
{% for pub in site.data.publications %}
  <div class="paper">
    <div class="paper-title">{{ pub.title }}</div>
    <div class="paper-authors">{{ pub.authors }}</div>
    <div class="paper-meta">
      {% if pub.journal %}{{ pub.journal }}{% endif %}
      {% if pub.year %}, {{ pub.year }}{% endif %}
      {% if pub.DOI %} · <a href="https://doi.org/{{ pub.DOI }}" target="_blank">DOI</a>{% endif %}
    </div>
  </div>
{% endfor %}
</div>

---
## 🎤 Presentations
<ul>
{% for talk in site.data.presentations %}
  <li>
    <strong>{{ talk.type }}</strong>, {{ talk.event }}, {{ talk.location }} — {{ talk.date }}
  </li>
{% endfor %}
</ul>

---
## 💻 Programming
<h2>Skills</h2>
<p>
I use programming languages such as <strong>Mathematica</strong>, <strong>Python</strong>, and <strong>C++</strong>.
I also have experience with <strong>MATLAB</strong> and <strong>MAPLE</strong>.
</p>

<p><a href="/">← Back to Home</a></p>

---


