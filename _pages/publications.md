---
layout: page
permalink: /research/
title: Research
description: 
years-working-papers: [2025,2024]
years-accepted-papers: [2025,2024,2023,2022,2021,2018]
years-unpublished-papers: [2020,2016]

nav: true
nav_order: 2
---


<h1 class="post-title">
<font size="5.5">
Working Papers
</font>
</h1>

<div class="publications">

{% for y in page.years-working-papers %}
  {% bibliography -f working-papers -q @*[year={{y}}]* %}
{% endfor %}

</div>





<h1 class="post-title">
<font size="5.5">
Accepted Papers
</font>
</h1>

<div class="publications">

{% for y in page.years-accepted-papers %}
  {% bibliography -f accepted-papers -q @*[year={{y}}]* %}
{% endfor %}

</div>








<h1 class="post-title">
<font size="5.5">
Unpublished Papers and Technical Notes
</font>
</h1>

<div class="publications">

{% for y in page.years-unpublished-papers %}
  {% bibliography -f unpublished-papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
