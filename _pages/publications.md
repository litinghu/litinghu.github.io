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

  <em>[{{ publi.conf }}]</em><a href="{{ publi.title }}">{{ publi.link }}</a><br />
  {{ publi.author }}<br />
  {{ publi.conf_name }}(<em>{{ publi.conf_short}}</em>) {{ publi.conf_date }}<br />
  {% if publi.rate != "" %}
    Acceptance Rate: {{ publi.rate }}
  {% endif %}

{% endfor %}
