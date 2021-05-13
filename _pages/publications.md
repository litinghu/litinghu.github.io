---
title: "Elves Lab - Publications"
layout: gridlay
excerpt: "Elves Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

<p> &nbsp; </p>

{% for publi in site.data.publications %}

  <b>[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
  {{ publi.author }}<br />
  {{ publi.conf_name }} (<b>{{ publi.conf_short}}</b>) {{ publi.conf_date }}<br />
  {% if publi.rate != "" %}
  Acceptance Rate: {{ publi.rate }} <br />
  {% endif %}

{% endfor %}
