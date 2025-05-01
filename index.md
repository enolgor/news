---
layout: default
title: Noticias
---

# 🗓️ Noticias

<ul>
{% for report in site.pages %}
  {% if report.path contains 'reports/' %}
    <li><a href="{{ report.url }}">{{ report.name }}</a></li>
  {% endif %}
{% endfor %}
</ul>
