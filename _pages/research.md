---
title: "Elves Lab - Research"
layout: textlay
excerpt: "Elves Lab -- Research"
sitemap: false
permalink: /research/
---

# Research Interests

- <span style="color:#DC143C">**Stream Processing Systems:**</span> SR3, FP4S, Governor, ELF, Project Hoover
- <span style="color:#DC143C">**Spam Detection in Online Social Networks:**</span> SpamHunter, Oases
- <span style="color:#DC143C">**Developing Machine Learning Techniques for Systems:**</span> Max Orientation Coverage, dpSmart, XPlacer
- <span style="color:#DC143C">**Container as a Service in the Cloud:**</span> Docman
- <span style="color:#DC143C">**Resource Management in Large-Scale Data Centers:**</span> RBay, v-Bundle, Net-Cohort, Look Who’s Talking, Monalytics, Live Migration of VMs, Magnet

# Research Projects

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}