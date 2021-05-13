---
title: "Elves Lab - Publications"
layout: gridlay
excerpt: "Elves Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

<p> &nbsp; </p>

<b>Students advised by Dr.Liting Hu are identified by \"*\".</b> 

<h3>Conference Papers</h3>
<p> &nbsp; </p>
{% for publi in site.data.publications %}
  {% if publi.type == "main" %}
  <p>
  <b>[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf_short}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}

<p> &nbsp; </p>
<h3>Journal Articles</h3>
<p> &nbsp; </p>
{% for publi in site.data.publications %}
  {% if publi.type == "j" %}
  <p>
  <b>[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf_short}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}

<p> &nbsp; </p>
<h3>Workshop Papers</h3>
<p> &nbsp; </p>
{% for publi in site.data.publications %}
  {% if publi.type == "w" %}
  <p>
  <b>[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  In <em>{{ publi.conf_name }} (<b>{{ publi.conf_short}}</b>)</em>, {{ publi.conf_date }}.
  {% if publi.rate != 0 %}
  Acceptance Rate: {{ publi.rate }}
  {% endif %}
  </p>
  {% endif %}
{% endfor %}
