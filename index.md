---
layout: home
permalink:
title:
image:
  feature: home.jpg
---
<div style="clear: both;">
  <h6 style="font-size:15px; float:left">FEATURED ITEMS</h6>
  <h6 style="width:88%;height:4px;background:black;float:right;"> </h6>
</div>

<div class="tiles">
{% assign featured_posts = (site.posts|where:"featured","true") %}
{% for post in featured_posts limit:4 %}
    {% include feature-post-grid.html %}
{% endfor %}
</div>

<h6 style="width:100%;height:4px;background:black;float:right;"> </h6>

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid-list.html %}
{% endfor %}
</div><!-- /.tiles -->
