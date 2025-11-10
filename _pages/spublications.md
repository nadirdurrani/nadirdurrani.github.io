---
layout: page
permalink: /spublications/
title: publications by area

areas: [Knowledge Editing, Arabic LLMs, Latent Concepts, Neuron Analysis, Representation Analysis, Transfer Learning, Evaluation and Benchmarking, Translation and Reordering, Decoding, Domain Adaptation, Transliteration, Word Segmentation, Medical, Misc, Demos and Tools,  Findings, System Descriptions, Surveys, Tutorials, Theses]
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
