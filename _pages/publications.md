---
layout: page
permalink: /publications/
title: research
description: 
years: [2021+, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006]
nav: true
heading: my papers
---

<div class="publications">

My research interests span the theory and practice of machine learning, network and data science, and optimization.<br><br>

My papers are listed below in reverse chronological order by year. Note that authors on all of my papers appear in alphabetical order. Paper tags are colored as follows:

<span class="badge badge-danger">journal article</span> <span class="badge badge-primary">conference article</span> <span class="badge badge-warning">editorial work</span> <span class="badge badge-light">manuscript</span> .


{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
