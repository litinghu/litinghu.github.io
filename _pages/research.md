---
title: "Elves Lab - Research"
layout: textlay
excerpt: "Elves Lab -- Research"
sitemap: false
permalink: /research/
---

# Research Interests

- <span style="color:#DC143C">**Stream Processing Systems:**</span> [SR3](https://people.cs.vt.edu/~litinghu/doc/sr3.pdf), [FP4S](https://people.cs.vt.edu/~litinghu/doc/fp4s.pdf), [Governor](https://people.cs.vt.edu/~litinghu/doc/governor.pdf), [ELF](https://people.cs.vt.edu/~litinghu/doc/elf.pdf), [Project Hoover](https://people.cs.vt.edu/~litinghu/doc/projecthoover.pdf)
- <span style="color:#DC143C">**Spam Detection in Online Social Networks:**</span> [SpamHunter](https://people.cs.vt.edu/~litinghu/doc/spamhunter.pdf), [Oases](https://people.cs.vt.edu/~litinghu/doc/oases.pdf)
- <span style="color:#DC143C">**Developing Machine Learning Techniques for Systems:**</span> [Max Orientation Coverage](https://people.cs.vt.edu/~litinghu/doc/iros.pdf), [dpSmart](https://people.cs.vt.edu/~litinghu/doc/dpSmart.pdf), [XPlacer](https://people.cs.vt.edu/~litinghu/doc/mchpc.pdf)
- <span style="color:#DC143C">**Container as a Service in the Cloud:**</span> [Docman](https://people.cs.vt.edu/~litinghu/doc/Docman.pdf)
- <span style="color:#DC143C">**Resource Management in Large-Scale Data Centers:**</span> [RBay](https://people.cs.vt.edu/~litinghu/doc/rbay.pdf), [v-Bundle](https://people.cs.vt.edu/~litinghu/doc/vbundle.pdf), [Net-Cohort](https://people.cs.vt.edu/~litinghu/doc/netcohort.pdf), [Look Who’s Talking](https://people.cs.vt.edu/~litinghu/doc/look.pdf), [Monalytics](https://people.cs.vt.edu/~litinghu/doc/monalytics.pdf), [Live Migration of VMs](https://people.cs.vt.edu/~litinghu/doc/livemigration.pdf), [Magnet](https://people.cs.vt.edu/~litinghu/doc/magnet.pdf)

# Research Projects

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
<div class="well" style="height: 360px;">
      <pubtit>Scalable and Adaptive Edge Stream Processing</pubtit>
      <p><img src="/images/pubpic/edge.png" class="img-responsive" width="40%" style="float: left; margin-right: 20px;" height="1000"></p>
      <p>Internet-of-Things (IoT) applications such as self-driving cars, augmented reality, interactive gaming, and event monitoring have a tremendous potential to improve our lives. These applications generate a large influx of sensor data at massive scales. Under many time-critical scenarios, these massive data streams must be processed in a very short time to derive actionable intelligence. This CAREER project aims to support time-critical IoT applications by applying the stream processing paradigm to the Edge computing architecture in the dynamic, heterogeneous Edge environment. As an integral part of its research program, this CAREER project involves K-12, undergraduate and graduate level education in partnership with the local Public School system. <strong><a href="https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.013153">Read More</a></strong></p>
      <p><b>Selected Publications: </b>USENIX ATC’21</p>
      <p class="text-danger"><strong> </strong></p>
      <p> </p>
    </div>
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="40%" style="float: left; margin-right: 20px;" height="1100" />
  <p>{{ publi.description }} <strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
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