---
title: "구성원"
layout: gridlay
sitemap: false
permalink: /ko/team/
lang: ko
alt_lang: /team/
---

## 구성원

**함께할 연구원을 모집합니다!**

## 지도교수

<div class="section-card">
<div class="pi-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ site.photo }}" class="pi-photo" alt="조재진" loading="lazy">
<div>
<h3 class="pi-name">조재진 (Jaejin Cho), Ph.D.</h3>
<p style="font-style: italic; color: var(--text-secondary);">조교수, 세종대학교 AI로봇학과</p>
<div class="pi-links">
<a href="mailto:{{ site.email }}" class="icon-link" title="Email"><i class="fa-solid fa-envelope"></i></a>
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar"><i class="ai ai-google-scholar"></i></a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{% if site.links.cv contains '://' %}{{ site.links.cv }}{% else %}{{ site.url }}{{ site.baseurl }}/{{ site.links.cv }}{% endif %}" target="_blank" class="icon-link" title="CV"><i class="ai ai-cv"></i></a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub"><i class="fa-brands fa-github"></i></a>{% endif %}
{% if site.links.orcid and site.links.orcid != "" %}<a href="{{ site.links.orcid }}" class="icon-link" title="ORCID"><i class="ai ai-orcid"></i></a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>{% endif %}
</div>
</div>
</div>
</div>

{% if site.data.team_members.size > 0 %}
## 학부 연구생

<div class="team-grid">
{% for member in site.data.team_members %}
<div class="team-card">
<img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" class="team-photo" alt="{{ member.name }}" loading="lazy">
<h4 class="team-name">{{ member.name }}</h4>
<p class="team-info">{{ member.info_ko | default: member.info }}</p>
</div>
{% endfor %}
</div>
{% endif %}

{% if site.data.alumni.size > 0 %}
## 졸업생

<div class="section-card">
<table class="alumni-table">
<thead>
<tr><th>이름</th><th>기간</th><th>구분</th></tr>
</thead>
<tbody>
{% for member in site.data.alumni %}
<tr>
<td>{{ member.name }}</td>
<td>{{ member.duration }}</td>
<td>{{ member.info_ko | default: member.info }}</td>
</tr>
{% endfor %}
</tbody>
</table>
</div>
{% endif %}

연구실 합류에 관심이 있다면 조재진 교수([jaejincho@sejong.ac.kr](mailto:jaejincho@sejong.ac.kr))에게 편하게 이메일 주세요.
