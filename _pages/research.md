---
title: "Elves Lab - Research"
layout: textlay
excerpt: "Elves Lab -- Research"
sitemap: false
permalink: /research/
---

# Research Interests

- <span>**Stream Processing Systems:**</span> [DART](https://people.ucsc.edu/~lhu82/Biobibnet/21ATC_Dart.pdf ), [SR3](https://people.ucsc.edu/~lhu82/Biobibnet/20Middleware_SR3.pdf), [FP4S](https://people.ucsc.edu/~lhu82/Biobibnet/20IPDPS_FP4S.pdf), [Governor](https://people.ucsc.edu/~lhu82/Biobibnet/17ICAC_Governor.pdf), [ELF](https://people.ucsc.edu/~lhu82/Biobibnet/14ATC_ELF.pdf), [Project Hoover](https://people.ucsc.edu/~lhu82/Biobibnet/Workshop/12MBDS_ProjectHoover.pdf), [SpamHunter](https://people.ucsc.edu/~lhu82/Biobibnet/19Cloud_Exploiting.pdf), [Oases](https://people.ucsc.edu/~lhu82/Biobibnet/18Cloud_Oases.pdf)
- <span>**Machine Learning (ML) Systems and Systems for ML:**</span> [Totoro](https://people.ucsc.edu/~lhu82/Biobibnet/24Eurosys_Totoro.pdf), [Max Orientation Coverage](https://people.ucsc.edu/~lhu82/Biobibnet/20IROS_3D.pdf), [dpSmart](https://people.ucsc.edu/~lhu82/Biobibnet/19BigData_dpSmart.pdf), [XPlacer](https://people.ucsc.edu/~lhu82/Biobibnet/Workshop/19MCHPC_GPU.pdf)
- <span>**Systems Virtualization and Serverless Computing:**</span> [Docman](https://people.ucsc.edu/~lhu82/Biobibnet/18Cloud_DocMan.pdf), [Net-Cohort](https://people.ucsc.edu/~lhu82/Biobibnet/12ICAC_NetCohort.pdf), [Look Who’s Talking](https://people.ucsc.edu/~lhu82/Biobibnet/Workshop/10HotCloud_LookWho'sTalking.pdf), [Live Migration of VMs](https://people.ucsc.edu/~lhu82/Biobibnet/09HPDC_Livemigration.pdf)
- <span>**Resource Management in Large-Scale Data Centers:**</span> [RBay](https://people.ucsc.edu/~lhu82/Biobibnet/17ICDCS_Rbay.pdf), [v-Bundle](https://people.ucsc.edu/~lhu82/Biobibnet/12ICDCS_vBundle.pdf), [Monalytics](https://people.ucsc.edu/~lhu82/Biobibnet/11ICAC_Monalytics.pdf), [Magnet](https://people.ucsc.edu/~lhu82/Biobibnet/08Cluster_Magnet.pdf)

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
  <pubtit><a href="{{ site.url }}{{ site.baseurl }}{{ publi.link.permalink }}" target="_blank">{{ publi.title }}</a></pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="31%" style="float: left; margin-right: 30px; box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19); border-radius: 3%;" height="1100" />
  <p>{{ publi.description }} <a href="{{ site.url }}{{ site.baseurl }}{{ publi.link.permalink }}" target="_blank">{{ publi.link.display }}</a></p>
  {% if publi.authors %}
  <p><b>Selected Publications: </b>{{ publi.authors }}</p>
  {% endif %}
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