---
layout: default
title: "📖 Stories"
hide_title: true
---

# 📖 Stories

<ul>
  {% for story in site.stories %}
      <li><a href="{{ story.url | relative_url }}">{{ story.title }}</a></li>
  {% endfor %}
</ul>