---
title: "소식"
layout: gridlay
sitemap: false
permalink: /ko/allnews.html
lang: ko
alt_lang: /allnews.html
---

## 소식

<div class="section-card" markdown="0">
<div class="news-timeline">
{% for article in site.data.news %}
<div class="news-item">
<span class="news-date">{{ article.date }}</span>
<span class="news-headline">{{ article.headline_ko | default: article.headline }}</span>
</div>
{% endfor %}
</div>
</div>
