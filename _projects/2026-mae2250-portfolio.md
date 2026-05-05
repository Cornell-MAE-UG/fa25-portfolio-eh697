---
layout: default
title: MAE 2250
image: /assets/images/spotted_lanternfly3.jpg
permalink: /projects/2250project
---

This semester in MAE 2250 - Introduction to Mechanical Design, the class Open Design Project aimed to tackle the issues posed to grape farmers by the presence of invasive Spotted Lanternflies in the North American Northeast. This project provided students with the opportunity to iteratively design and test prototypes that were successively improved based on client feedback. Below are three reports marking several milestones in the development of my team's final prototype.

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