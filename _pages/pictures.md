---
title: "Allan Lab - Pictures"
layout: piclay
excerpt: "Allan Lab -- Pictures"
permalink: /pictures/
---

# Open Positions

Our lab aims to train students towards becoming first-class system researchers and system builders. If you enjoy building systems, I would love to have you join the lab.
**We are always looking for new group members with passion, talent, and grit!**

# Applications for Ph.D. and Postdoc positions

If you are interested in working with us as a Ph.D. student or postdoc, please feel free to contact me. State briefly why you are interested and attach a CV, including information about the grades you had as an undergraduate. No need for a separate cover letter or certificates. Important: please insert “PhD Application – Your Name” or “Postdoc Application – Your Name” in the subject line. If you are applying to a specific advertisement, note this in your email.

# Master projects for Virginia Tech students

If you are a Master student at Virginia Tech looking for a Master project, contact me (or any group member) per email or stop by my office.

#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

First advertisement.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageLeiden_red.jpg" width="60%" >
</figure>


## ETHZ
From the [group of Andreas Wallraff](http://www.qudev.ethz.ch/).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageETH_red.jpg" width="60%">
</figure>

## Cornell
From the [group of Seamus JC Davis](http://davisgroup.lassp.cornell.edu).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageCornell_red.jpg" width="60%">
</figure>

## St Andrews
From the [group of Felix Baumberger](http://dqmp.unige.ch/baumberger/) (now at University of Geneva).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageSTA_red.jpg" width="60%">
</figure>
