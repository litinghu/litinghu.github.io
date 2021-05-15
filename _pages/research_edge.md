---
title: "Elves Lab - Research_edge"
layout: textlay
excerpt: "Elves Lab -- Research_edge"
sitemap: false
permalink: /research_edge/
---

# Research Interests

- <span>**Stream Processing Systems:**</span> [SR3](https://people.cs.vt.edu/~litinghu/doc/sr3.pdf), [FP4S](https://people.cs.vt.edu/~litinghu/doc/fp4s.pdf), [Governor](https://people.cs.vt.edu/~litinghu/doc/governor.pdf), [ELF](https://people.cs.vt.edu/~litinghu/doc/elf.pdf), [Project Hoover](https://people.cs.vt.edu/~litinghu/doc/projecthoover.pdf)
- <span>**Spam Detection in Online Social Networks:**</span> [SpamHunter](https://people.cs.vt.edu/~litinghu/doc/spamhunter.pdf), [Oases](https://people.cs.vt.edu/~litinghu/doc/oases.pdf)
- <span>**Developing Machine Learning Techniques for Systems:**</span> [Max Orientation Coverage](https://people.cs.vt.edu/~litinghu/doc/iros.pdf), [dpSmart](https://people.cs.vt.edu/~litinghu/doc/dpSmart.pdf), [XPlacer](https://people.cs.vt.edu/~litinghu/doc/mchpc.pdf)
- <span>**Container as a Service in the Cloud:**</span> [Docman](https://people.cs.vt.edu/~litinghu/doc/Docman.pdf)
- <span>**Resource Management in Large-Scale Data Centers:**</span> [RBay](https://people.cs.vt.edu/~litinghu/doc/rbay.pdf), [v-Bundle](https://people.cs.vt.edu/~litinghu/doc/vbundle.pdf), [Net-Cohort](https://people.cs.vt.edu/~litinghu/doc/netcohort.pdf), [Look Who’s Talking](https://people.cs.vt.edu/~litinghu/doc/look.pdf), [Monalytics](https://people.cs.vt.edu/~litinghu/doc/monalytics.pdf), [Live Migration of VMs](https://people.cs.vt.edu/~litinghu/doc/livemigration.pdf), [Magnet](https://people.cs.vt.edu/~litinghu/doc/magnet.pdf)

<h1 id="research-projects" style="
    margin-bottom: 22px;
">Research Projects</h1>

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well"  style="height: {{publi.wellheight}}px; margin-bottom: 40px;">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="31%" style="float: left; margin-right: 30px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); border-radius: 3%;" height="1100" />
  <p>{{ publi.description }} <a href="{{ publi.link.url }}">{{ publi.link.display }}</a></p>
  <p><b>Selected Publications: </b>{{ publi.authors }}</p>
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