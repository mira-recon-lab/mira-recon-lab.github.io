---
layout: page
title: Software
permalink: /software/
description: Open-source software released by MIRA Lab. Click each card for details and code.
nav: true
nav_order: 5
display_categories: [Open Source, Customer-to-Producer]
horizontal: false
---

<!-- pages/software.md -->
<div class="software-list">
{% for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  {% for project in sorted_projects %}
    <div class="software-item">
      <div class="software-icon">
        <i class="fa-solid fa-code"></i>
      </div>
      <div class="software-body">
        <a class="software-title" href="{% if project.redirect %}{{ project.redirect }}{% else %}{{ project.url | relative_url }}{% endif %}">{{ project.title }}</a>
        <p class="software-desc">{{ project.description }}</p>
        {% if project.github %}
          <a class="software-github" href="{{ project.github }}"><i class="fa-brands fa-github"></i> Code</a>
        {% endif %}
      </div>
    </div>
  {% endfor %}
{% endfor %}
</div>
