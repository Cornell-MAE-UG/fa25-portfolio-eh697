---
layout: default
title: Elias Herrera Hernandez - Portfolio
permalink: /projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        {% if project.group != "group1" %}
          <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title }}</p>
        </a>
        {% endif %}
      </div>
    {% endfor %}
</div>
</div>