---
layout: page
permalink: /publications/
title: Publications
description: All publications of the Lab.
years: [2022,2021,2020,2019,2018,2017,2016,2015,2014,2013,2012,2011,2010,2009,2008,2007,2006]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f labpapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
