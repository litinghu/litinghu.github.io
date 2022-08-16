---
title: "Elves Lab - Outreach"
layout: textlay
excerpt: "Elves Lab -- Outreach"
sitemap: false
permalink: /Outreach/
---

<h1 id="Outreach Activities" style="
    margin-bottom: 22px;
">Outreach Activities</h1>

{% assign number_printed = 0 %}
{% for publi in site.data.outreach %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well"  style="height: {{publi.wellheight}}px; margin-bottom: 40px;">
  <pubtit><a href="{{ publi.link.url }}" target="_blank">{{ publi.title }}</a></pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="31%" style="float: left; margin-right: 30px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); border-radius: 3%;" height="1100" />
  <p>{{ publi.description }} <a href="{{ publi.link.url }}" target="_blank">{{ publi.link.display }}</a></p>
  <p><b>Organizer: </b>{{ publi.organizers }}</p>
  <p><b>Location: </b>{{ publi.location}}</p>
  <p><b>Date: </b>{{ publi.date }}</p>
  <p><b>Participants: </b>{{ publi.participants }}</p>
  <p><a [href="{{ publi.slides.url }}" target="_blank">{{ publi.slides.display }}]</a>   &emsp;<a [href="{{ publi.gallery.url }}" target="_blank">{{ publi.gallery.display }}]</a></p>
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
