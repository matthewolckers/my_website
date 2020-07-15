---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order.
order: 1
years: [2020]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
