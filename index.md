---
layout: home
permalink:
title:
image:
  feature: home.jpg
---
<div style="clear: both;">
  <h6 style="font-size:15px; float:left;margin:0px;border:0px;padding:0px">FEATURED ITEMS</h6>
  <h6 style="width:100%;height:2px;background:black;float:right;margin-top:0px;"> </h6>
</div>

<div class="tiles">
{% assign featured_posts = (site.posts|where:"featured","true") %}
{% for post in featured_posts limit:4 %}
    {% include feature-post-grid.html %}
{% endfor %}
</div>

<h6 style="width:100%;height:2px;background:black;float:right;margin-top:0px"> </h6>

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
