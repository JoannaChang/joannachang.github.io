---
layout: publications
permalink: /publications/
title: publications
description: (*) denotes equal contribution, (**) denotes joint supervision
years: [2023,2021,2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
