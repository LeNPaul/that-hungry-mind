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

<div style="clear: both;">
  <h6 style="font-size:15px; float:left;margin:0px;border:0px;padding:0px">RECENT ITEMS</h6>
  <h6 style="width:100%;height:2px;background:black;float:right;margin-top:0px;"> </h6>
</div>

<div class="tiles">
{% for post in site.posts limit:12 %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

<div style="clear: both;">
  <h6 style="font-size:15px; float:left;margin:0px;border:0px;padding:0px">MORE</h6>
  <h6 style="width:100%;height:2px;background:black;float:right;margin-top:0px;"> </h6>
</div>

<div class="tiles">
{% for link in site.data.navigation %}
<article class="tile" itemscope itemtype="http://schema.org/Article">
  <a href="{{ site.url }}{{ link.url }}" title="{{ link.title }}" class="post-teaser">
    {% if post.image.teaser %}
      <img src="{{ site.url }}/images/{{ post.image.teaser }}" alt="teaser" itemprop="image">
    {% else %}
      <img src="{{ site.url }}/images/{{ link.home-image }}" alt="teaser" itemprop="image">{% endif %}</a>
  <h2 class="post-title" itemprop="name"><a href="{{ site.url }}{{ link.url }}">{{ link.title }}</a></h2>
  <p class="post-excerpt" itemprop="description">{{ link.excerpt }}</p>
</article><!-- /.tile -->
{% endfor %}
</div>
