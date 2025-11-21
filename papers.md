---
layout: default
title: Papers
---

<h2>Papers</h2>

<!-- Publications Section -->
{% assign pubs = site.data.publications | where_exp: "p", "p.journal" %}
{% if pubs.size > 0 %}
<section class="publications">
  <h3>Publications</h3>
  <ol class="paper-list">
    {% for paper in pubs %}
    <li class="paper">
      <span class="paper-authors">{{ paper.authors }}.</span>
      <span class="paper-title"><strong>{{ paper.title }}</strong>.</span>

      {% if paper.journal %}
      <span class="paper-journal"><em>{{ paper.journal }}</em>.</span>
      {% endif %}

      <span class="paper-year">{{ paper.year }}.</span>

      {% if paper.doi %}
      <a href="https://doi.org/{{ paper.doi }}">DOI</a>.
      {% endif %}

      {% if paper.pdf %}
      <a href="{{ paper.pdf }}">[PDF]</a>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>
{% endif %}

<!-- Preprints Section -->
{% assign preprints = site.data.publications | where_exp: "p", "p.preprint" %}
{% if preprints.size > 0 %}
<h3>Preprints</h3>
<ol class="paper-list">
  {% for p in preprints %}
  <li class="paper">
    <span class="paper-title"><strong>{{ p.title }}</strong>.</span>
    <span class="paper-authors">{{ p.authors }}.</span>
    <span class="paper-year">{{ p.year }}.</span>

    {% if p.preprint %}
    <a href="https://arxiv.org/abs/{{ p.preprint }}" target="_blank">arXiv:{{ p.preprint }}</a>
    {% endif %}
  </li>
  {% endfor %}
</ol>
{% endif %}

<!-- Notes Section -->
{% assign notes = site.data.publications | where: "note", true %}
{% if notes.size > 0 %}
<h3>Notes</h3>
<ol class="paper-list">
  {% for n in notes %}
  <li class="paper">
    <span class="paper-title"><strong>{{ n.title }}</strong>.</span>
    <span class="paper-authors">{{ n.authors }}.</span>
    <span class="paper-year">{{ n.year }}.</span>
    {% if n.file_link %}
      <a href="{{ n.file_link }}" target="_blank">[PDF]</a>
    {% endif %}
  </li>
  {% endfor %}
</ol>
{% endif %}

<!-- Theses Section -->
{% assign theses = site.data.publications | where: "type", "thesis" %}
{% if theses.size > 0 %}
<h3>Theses</h3>
<ol class="paper-list">
  {% for t in theses %}
  <li class="paper">
    <span class="paper-title"><strong>{{ t.title }}</strong>.</span>
    <span class="paper-authors">{{ t.degree }} — {{ t.authors }}.</span>
    <span class="paper-year">{{ t.year }}.</span>
  </li>
  {% endfor %}
</ol>
{% endif %}

<p><a href="/">← Back to Home</a></p>
