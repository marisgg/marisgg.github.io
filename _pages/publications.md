---
layout: page
permalink: /publications/
title: Publications
description: This list contains my articles in proceedings, workshop/arXiv papers, as well as my master's thesis.
years: [2025, 2024, 2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
