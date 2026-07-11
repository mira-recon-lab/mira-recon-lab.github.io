---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
lang: en
alt_lang: /ko/publications/
---

## Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h3>Refereed Journal Articles</h3>

{% bibliography --query @article %}

<h3>Peer-reviewed Conference Papers</h3>

{% bibliography --query @*[category=conf_paper] %}

<h3>Preprints</h3>

{% bibliography --query @unpublished %}

<h3>Conference Abstracts</h3>

{% bibliography --query @*[category=conf_abstract] %}
</div>
