---
layout: page
permalink: /publications/
title: Publications
description: You can also browse my <a href="https://scholar.google.it/citations?hl=en&user=JBnyLicAAAAJ&view_op=list_works&sortby=pubdate" target="_blank"><b>Google Scholar</b></a> profile.
years: [2021, 2020, 2019, 2018, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
