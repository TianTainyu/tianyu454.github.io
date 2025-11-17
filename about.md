---
layout: default
title: About
permalink: /about/
---


<div class="intro">
  <div class="intro-text">
    I am a postdoctoral researcher under the supervision of Jianhong Wu at York University, Canada.
    Before that, I completed my PhD under the supervision of Xingfu Zou at the University of Western Ontario.
    Previously, I obtained my Bachelor’s and Master’s degrees at Beijing Normal University under the supervision of Xu'an Zhao.
  </div>

  <div class="intro-image">
    ![Profile Photo](/assets/images/profile.jpg)
  </div>
</div>

## Research Interests

- Mathematical biology  
- Infectious disease modelling  
- Dynamical systems  
- Applied mathematics  

## Papers

<div class="papers">
{% for pub in site.data.publications %}
  <div class="paper">
    <div class="paper-title">{{ pub.title }}</div>
    <div class="paper-authors">{{ pub.authors }}</div>
    <div class="paper-meta">{{ pub.journal }}, {{ pub.year }}</div>
    {% if pub.link %}
    <a href="{{ pub.link }}" class="paper-link">[PDF]</a>
    {% endif %}
  </div>
{% endfor %}
</div>

## Contact

<div class="contact">
  Email:
  <a href="mailto:tianyu45@yorku.ca">tianyu45@yorku.ca</a>,
  <a href="mailto:tchen454@uwo.ca">tchen454@uwo.ca</a>
</div>
