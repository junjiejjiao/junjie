---
layout: page
permalink: /publications/
title: Publications
description: publications in reversed chronological order.  
years: [2023, 2022, 2021, 2020, 2018]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">
{%- for y in page.years %}
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
