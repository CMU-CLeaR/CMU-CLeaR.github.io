---
layout: page
permalink: /publications/
title: publications
description: Please see <a href="https://www.andrew.cmu.edu/user/kunz1/Publications.html"><u>here</u></a> for 
full list of publications and <a href="https://www.andrew.cmu.edu/user/kunz1/Research.html"><u>research 
overview</u></a>.
years: [2021, 2020, 2019]
nav: true
---

<b>CLeaR Members:</b> If you want to add your publications to this page, please refer to the <a 
href="https://github.com/cmu-clear/cmu-clear.github.io/blob/main/docs/publications.md">instruction</a>.

<div class="publications">
<h2>Jump to: <a href="#preprints">preprints</a>, <a href="#publications">publications</a>, <a href="#dissertations">dissertations</a>.</h2>

<h1 class="year" id="preprints">preprints</h1>
{% bibliography -f preprints %}

<h1 id="publications">publications</h1>
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1 class="year" id="dissertations">theses</h1>
{% bibliography -f dissertations %}

</div>
