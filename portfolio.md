---
layout: page
title: portfolio
permalink: /portfolio/
---

here are some of my projects :)

<ul>
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url | relative_url }}">
        {{ project.title }}
      </a> — {{ project.description }}
    </li>
  {% endfor %}
</ul>