---
layout: page
permalink: /spublications/
title: publications by area

areas: [Latent Concepts, Neuron Analysis, Representation Analysis, Translation and Reordering, Decoding, Transfer Learning, Domain Adaptation, Transliteration, Word Segmentation, MT Evaluation,  COVID-19, Demos and Tools]
nav: false
nav_order: 1
---
<!-- _pages/spublications.md -->
<div class="publications">

{%- for y in page.areas %}
  <h2 style="color: green" class="area">{{y}}</h2>
  {% bibliography -f papers -q @*[area={{y}}]* %}
{% endfor %}

</div>
