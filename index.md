---
layout: default
title: Noticias
---

# 🗓️ Noticias

<ul>
{% for report in site.pages %}
  {% if report.path contains 'reports/' %}
    <li><a href="/news/{{ report.name | remove: '.md' }}.html">{{ report.name | remove: '.md' }}</a></li>
  {% endif %}
{% endfor %}
</ul>
