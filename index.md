---
layout: home
permalink: /
title: "Things that interest me"
image:
  feature: home.jpg
---

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
