---
title: "블로그"
layout: gridlay
sitemap: false
permalink: /ko/blogs/
published: false  # upstream template placeholder — hidden until real content exists
lang: ko
alt_lang: /blogs/
---

## 블로그

{% if site.posts.size > 0 %}
<div class="section-card" markdown="0">
{% for post in site.posts %}
<div class="news-item" style="padding: 1rem 0; border-bottom: 1px solid var(--border-color);">
<span class="news-date">{{ post.date | date: "%Y년 %-m월 %-d일" }}</span><br>
<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" style="font-weight: 600;">{{ post.title }}</a>
</div>
{% endfor %}
</div>
{% else %}
<p class="text-muted">아직 게시글이 없습니다.</p>
{% endif %}
