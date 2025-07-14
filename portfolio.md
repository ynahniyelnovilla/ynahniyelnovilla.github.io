---
layout: page
title: portfolio
permalink: /portfolio/
---

here are some of my projects :)

<div class="portfolio-grid">
  {% for project in site.projects %}
    <div class="project-card">
      {% if project.thumbnail %}
        <img src="{{ project.thumbnail }}" alt="{{ project.title }} thumbnail" class="project-thumb">
      {% endif %}
      <div class="project-info">
        <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
        <p class="description">{{ project.description }}</p>
        {% if project.tools %}
          <p class="tools"><strong>Tools:</strong> {{ project.tools }}</p>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
