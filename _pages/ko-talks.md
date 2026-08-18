---
title: "발표"
layout: gridlay
sitemap: false
permalink: /ko/talks/
published: false  # upstream template placeholder — hidden until real content exists
lang: ko
alt_lang: /talks/
---

## 발표

<div class="section-card" id="pubList">
<h3>초청 강연</h3>

{% bibliography --query @incollection[keywords ^= invited] %}

<h3>일반 발표</h3>

{% bibliography --query @incollection[keywords != invited] %}
</div>
