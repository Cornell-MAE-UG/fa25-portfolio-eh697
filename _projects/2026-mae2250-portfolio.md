---
layout: default
title: MAE 2250
image: /assets/images/spotted_lanternfly3.jpg
permalink: /projects/2250project
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      {% if project.group == "group1" %}
        <div class="gallery-item">
          <a href="{{ project.url | relative_url }}"> 
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" /> 
            <p>{{ project.title }}</p> 
          </a> 
        </div>
      {% endif %}
    {% endfor %}
</div>
</div>