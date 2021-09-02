---
layout: page
permalink: /publications/
title: publications
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
---

For a more up-to-date list, please also see my [google scholar](https://scholar.google.com/citations?user=2d-0ybAAAAAJ&hl=en) page.

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
