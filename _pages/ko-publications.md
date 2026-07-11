---
title: "출판"
layout: gridlay
sitemap: false
permalink: /ko/publications/
lang: ko
alt_lang: /publications/
---

## 출판

<input type="text" class="pub-search" id="pubSearch" placeholder="제목·저자·연도로 검색...">

<div class="section-card" id="pubList">
<h3>학술지 논문</h3>

{% bibliography --query @article %}

<h3>학술대회 논문</h3>

{% bibliography --query @*[category=conf_paper] %}

<h3>학술대회 초록</h3>

{% bibliography --query @*[category=conf_abstract] %}
</div>
