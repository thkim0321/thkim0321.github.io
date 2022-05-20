---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2023]
nav: true
nav_order: 1
---

Currently, this page is under construction. For now, you can find a complete publication list in my <a href = '/al-folio/assets/pdf/cv.pdf'>cv</a>. 

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
