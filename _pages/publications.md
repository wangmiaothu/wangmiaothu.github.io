---
title: "Publications | Miao Wang @ Beihang U."
layout: gridlay
excerpt: "Publications | Miao Wang"
sitemap: false
permalink: /publications/
---


<!-- ### **Publications** -->

<div><h3 style="font-family: 'Alegreya SC', Helvetica Neue,Source Sans Pro,Arial"><b>Publications</b></h3></div>
(in chronological order; see also my [Google Scholar Profile](https://scholar.google.com/citations?user=BaOhbFsAAAAJ&hl=en))

<br>

<!-- ### *Research Highlights*

(See full list [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=AAwLfKUAAAAJ&hl=en))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
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

<p> &nbsp; </p> -->


<!-- ### *Full List* -->


{% for publi in site.data.publist %}

{% if publi.year.show == 1 %}
{% if publi.year.line == 1 %}
<hr>
{%endif%}
<div><h4 style="font-family: 'Alegreya SC', Helvetica Neue,Source Sans Pro,Arial"><b>{{publi.year.note}}</b></h4></div> 
{%endif%}

<img src="{{ site.url }}{{ site.baseurl }}/images/paperpic/{{ publi.image }}" class="img-responsive" width="12%" style="float: left; margin-top: 0.5%" />
<!-- <img src="{{ site.url }}{{ site.baseurl }}/images/paperpic/{{ publi.image }}" class="img-responsive" width="10%" style="float: left" /> -->
{% if publi.new == 1 %}
  <b style="color:red">NEW! &nbsp;</b> <a href="{{ publi.link.url }}"><b>{{ publi.title }}</b></a><br>
  {{ publi.authors }}<br />
  {{ publi.link.display }}<br />
  {{ publi.news2 }} <br/> 
{%else%}
  <a href="{{ publi.link.url }}"><b>{{ publi.title }}</b></a><br> 
  {{ publi.authors }}<br />
  {{ publi.link.display }}<br />
  {{ publi.news2 }} <br/> 
{%endif%}


  

{% endfor %}




<!-- {% for publi in site.data.publist %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="10%" style="float: left" />
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br />
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %} -->


