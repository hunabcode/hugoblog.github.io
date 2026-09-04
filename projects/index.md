---
layout: default
title: Projects
permalink: /projects/
---

# Projects

<ul>
{% for p in site.projects %}
  <li>
    <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
    {% if p.date %} - <small>{{ p.date | date: "%Y-%m-%d" }}</small>{% endif %}
  </li>
{% endfor %}
</ul>
