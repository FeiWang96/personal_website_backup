---
layout: page
permalink: /publications/
title: publications
description: * denotes equal contribution and joint lead authorship.
years: [2021, 2020, 2019]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
