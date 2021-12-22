---
layout: page
permalink: /publications/
title: Publications
description: You may also checkout <a href="https://www.andrew.cmu.edu/user/kunz1/Publications.html"><u>full list of publications</u></a> and <a href="https://www.andrew.cmu.edu/user/kunz1/Research.html"><u>research overview</u></a>.
years: [2021, 2020, 2019]
nav: true
---

<div class="publications">


<h1 id="publications">publications</h1>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


</div>




