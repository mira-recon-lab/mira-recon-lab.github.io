---
layout: page
permalink: /publications/
title: Publications
description: Publications by MIRA Lab, grouped by category. Click each category to expand or collapse. * indicates equal contribution.
nav: true
nav_order: 4
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<details open class="pub-category">
  <summary>Journal articles</summary>
  {% bibliography -q @*[category=journal] %}
</details>

<details open class="pub-category">
  <summary>Peer-reviewed conference papers</summary>
  {% bibliography -q @*[category=conf_paper] %}
</details>

{% capture preprints %}{% bibliography -q @*[category=preprint] %}{% endcapture %}
{% assign preprints_content = preprints | strip_html | strip %}
{% if preprints_content != "" %}

<details class="pub-category">
  <summary>Preprints (arXiv)</summary>
  {{ preprints }}
</details>

{% endif %}

<details class="pub-category">
  <summary>Conference abstracts</summary>
  {% bibliography -q @*[category=conf_abstract] %}
</details>

</div>
