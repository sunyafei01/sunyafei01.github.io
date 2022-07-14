---
layout: page
permalink: /publications/
title: publications
description: 虽然现在还没有，但是以后一定会有的！
years: []
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
