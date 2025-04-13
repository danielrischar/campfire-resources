---
layout: default
title: Content
---

<h1>Lion</h1>
<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Lion" %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Tiger</h1>
<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Tiger" %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Wolf</h1>
<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Wolf" %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Bear</h1>
<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Bear" %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Webelos</h1>
<ul>
  {% for skit in site.skits %}
    {% if skit.age_groups contains "Webelos" %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>


