---
layout: default
title: "🎶 Songs"
hide_title: true
---

# 🎶 Songs

<ul>
  {% for song in site.songs %}
      <li><a href="{{ song.url | relative_url }}">{{ song.title }}</a></li>
  {% endfor %}
</ul>