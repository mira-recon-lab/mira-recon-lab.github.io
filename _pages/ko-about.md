---
title: "소개"
layout: gridlay
sitemap: false
permalink: /ko/about/
lang: ko
alt_lang: /about/
---

## 소개

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ site.photo }}" class="pi-photo" alt="조재진" loading="lazy">
<div>
<h3 class="pi-name">조재진 (Jaejin Cho), Ph.D.</h3>
<p style="font-style: italic; color: var(--text-secondary);">조교수 · MIRA Lab, 세종대학교 인공지능로봇학과</p>
<div class="pi-links">
<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{% if site.links.cv contains '://' %}{{ site.links.cv }}{% else %}{{ site.url }}{{ site.baseurl }}/{{ site.links.cv }}{% endif %}" target="_blank" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
</div>
</div>
</div>
</div>
