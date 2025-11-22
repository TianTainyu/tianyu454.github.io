---
layout: default
title: About
permalink: /about/
---

<style>
  .papers { margin-top: 20px; }
  .paper { margin-bottom: 18px; padding-bottom: 14px; border-bottom: 1px solid #010305ff; }
  .paper-title { font-weight: 600; font-size: 1.05rem; }
  .paper-authors { color: #020408ff; margin-top: 2px; }
  .paper-meta { color: #01060aff; font-size: 0.95rem; margin-top: 2px; }

  ul { line-height: 1.7; }

  .contact a { color: #010409ff; text-decoration: none; }
  .contact a:hover { text-decoration: underline; }
</style>

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
      {% if pub.DOI %} · <a href="https://doi.org/{{ pub.DOI }}" target="_blank">Available here</a>{% endif %}
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

## 💻 Skills

<p>
I use programming languages such as <strong>Mathematica</strong>, <strong>Python</strong>, and <strong>C++</strong>.
I also have experience with <strong>MATLAB</strong> and <strong>MAPLE</strong>.
</p>

---

<p><a href="/">← Back to Home</a></p>