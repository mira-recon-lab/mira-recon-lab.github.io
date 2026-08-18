---
title: "News"
layout: gridlay
sitemap: false
permalink: /allnews.html
lang: en
alt_lang: /ko/allnews.html
---

## News

<div class="section-card" markdown="0">
<div class="news-timeline">
{% for article in site.data.news %}
<div class="news-item" id="news-{{ article.date }}-{{ article.headline | slugify }}">
<span class="news-date">{{ article.date }}</span>
<span class="news-headline">{{ article.headline }}</span>
</div>
{% endfor %}
</div>
</div>
