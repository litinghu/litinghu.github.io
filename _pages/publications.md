---
title: "Elves Lab - Publications"
layout: gridlay
excerpt: "Elves Lab -- Publications."
sitemap: false
permalink: /publications/
---


<h1 style="margin-bottom: 22px;">Publications</h1>

<b>Students advised by Dr.Liting Hu are identified by \"*\"</b> 

<h3 style="margin-top:22px; margin-bottom: 22px;">Conference Papers</h3>
{% for publi in site.data.publications %}
  {% if publi.type == "main" %}
  <p style="margin-bottom: 22px;">
  <b style="color:#DC143C">[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}

<h3 style="margin-bottom: 22px;">Journal Articles</h3>
{% for publi in site.data.publications %}
  {% if publi.type == "j" %}
  <p style="margin-bottom: 22px;">
  <b style="color:#DC143C">[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}

<h3 style="margin-bottom: 22px;">Workshop Papers</h3>
{% for publi in site.data.publications %}
  {% if publi.type == "w" %}
  <p style="margin-bottom: 22px;">
  <b style="color:#DC143C">[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}
