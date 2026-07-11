---
layout: page
permalink: /ko/publications/
title: 출판
lang: ko
alt_lang: /publications/
description: MIRA Lab 논문 목록. 각 항목을 눌러 펼치거나 접을 수 있습니다. *는 동등 기여를 의미합니다.
nav: true
nav_order: 4
---

<!-- _pages/ko-publications.md — 논문 정보는 영문 그대로 표시됩니다. -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<details open class="pub-category">
  <summary>학술지 논문 (Journal articles)</summary>
  {% bibliography -q @*[category=journal] %}
</details>

<details open class="pub-category">
  <summary>학술대회 논문 (Peer-reviewed conference papers)</summary>
  {% bibliography -q @*[category=conf_paper] %}
</details>

{% capture preprints %}{% bibliography -q @*[category=preprint] %}{% endcapture %}
{% assign preprints_content = preprints | strip_html | strip %}
{% if preprints_content != "" %}

<details class="pub-category">
  <summary>프리프린트 (Preprints, arXiv)</summary>
  {{ preprints }}
</details>

{% endif %}

<details class="pub-category">
  <summary>학술대회 초록 (Conference abstracts)</summary>
  {% bibliography -q @*[category=conf_abstract] %}
</details>

</div>
