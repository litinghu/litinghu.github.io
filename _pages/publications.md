---
title: "Elves Lab - Publications"
layout: gridlay
excerpt: "Elves Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

<p> &nbsp; </p>

<b>Students advised by Dr.Liting Hu are identified by</b> "*".

{% for publi in site.data.publications %}
  {% if publi.type == "main" %}
    ## Main Conference
    <b>[{{ publi.conf }}]</b> <a href="{{ publi.link }}">{{ publi.title }}</a><br />
    {{ publi.author }}<br />
    {{ publi.conf_name }} (<b>{{ publi.conf_short}}</b>), {{ publi.conf_date }}
    {% if publi.rate != "" %}
    Acceptance Rate: {{ publi.rate }}
    {% endif %}
  {% endif %}
{% endfor %}
