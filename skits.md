---
layout: default
title: "🎭 Skits"
hide_title: true
---

# 🎭 Skits

<ul>
  {% for skit in site.skits %}
      <li><a href="{{ skit.url | relative_url }}">{{ skit.title }}</a></li>
  {% endfor %}
</ul>