---
layout: default
title: Image Archive
---

{% include nav.html %}

Photographs and images of the peacewalls and the changing landscape of art on them throughout time.

<div style="display:flex; flex-wrap:wrap; gap:20px;">
{% for img in site.data.archive %}
  <figure style="width:280px; margin:0;">
    <img src="images/{{ img.file }}" alt="{{ img.alt }}" style="width:100%;">
    <figcaption><strong>{{ img.title }}</strong><br>{{ img.date }}. Source: {{ img.source }}.</figcaption>
  </figure>
{% endfor %}
</div>
