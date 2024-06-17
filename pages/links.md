---
layout: page
title: Links
description: N/A
keywords: links
comments: true
menu: links
permalink: /links/
---


<ul>
{% for link in site.data.links %}
  {% if link.src == 'life' %}
  <li><a href="{{ link.url }}" target="_blank">{{ link.name}}</a></li>
  {% endif %}
{% endfor %}
</ul>

