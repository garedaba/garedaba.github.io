---
layout: default
title: Projects
links:
  - title: View My GitHub Profile
    url: https://github.com/garedaba
---

# Projects

## [&mu;Brain](micro-brain/)
A 3D volumetric reconstruction of the mid-gestation fetal brain at micrometre scale, coupled with regional gene expression data.

Studies built on &mu;Brain:

<ul class="study-list">
{% for study in site.data.microbrain_studies %}
  <li><a href="{{ study.url | relative_url }}">{{ study.title }}</a>
    <small>{{ study.summary }} &middot; {{ study.venue }}</small></li>
{% endfor %}
</ul>
