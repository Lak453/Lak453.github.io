---
layout: page
title: About
description: N/A
keywords: Ho Wang Ho(Howard)
comments: true
menu: About
permalink: /about/
---

I am Ho Wang Ho (Howard), I love to study in programing language nice to meet you

## Contact

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

{% if condition %}
  <!-- Your content here -->
{% endif %}
