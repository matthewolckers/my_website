---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order.
order: 1
years_journals: [2020]
years_conferences: [2021]
nav: true
---

## Journals

<div class="publications">

{% for y in page.years_journals %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

---

<br>

## Conference Proceedings

<div class="publications">

{% for y in page.years_conferences %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>
