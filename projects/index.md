---
layout: archive
title: "Projects"
date: 2014-05-30T11:39:03-04:00
modified:
excerpt: "Things I've designed, illustrated, developed, coded, and whatever."
tags: []
image:
  feature:
  teaser:
---

<div class="tiles">
{% for post in site.categories.projects %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
