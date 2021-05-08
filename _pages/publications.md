---
title: "Allan Lab - Publications"
layout: gridlay
excerpt: "Allan Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

<!-- ## Group highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.ch/citations?user=TqxYWZsAAAAJ), [ResearcherID](https://www.researcherid.com/rid/D-7763-2012)) -->

<p> &nbsp; </p>

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
