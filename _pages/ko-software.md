---
layout: page
title: 소프트웨어
permalink: /ko/software/
lang: ko
alt_lang: /software/
description: MIRA Lab이 공개한 오픈소스 소프트웨어. 각 카드를 눌러 상세 내용과 코드를 확인하세요.
nav: true
nav_order: 5
display_categories: [Open Source, Customer-to-Producer]
horizontal: false
---

<!-- pages/ko-software.md -->
<div class="software-list">
{% for category in page.display_categories %}
  {% case category %}
    {% when 'Open Source' %}{% assign category_label = '오픈소스' %}
    {% when 'Customer-to-Producer' %}{% assign category_label = 'Customer-to-Producer' %}
    {% else %}{% assign category_label = category %}
  {% endcase %}
  <h2 class="category">{{ category_label }}</h2>
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
