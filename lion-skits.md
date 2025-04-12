---
layout: default
title: Skits for Lions
---

<h1>Skits Suitable for Lions</h1>

<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Lion" %}
      <li><a href="{{ skit.url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
