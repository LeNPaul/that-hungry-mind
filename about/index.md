---
layout: article
title: "About"
date:
modified:
excerpt: "Hi there! I'm Paul"
image:
  feature:
  teaser:
  thumb:
share: false
ads: false
---

#### Hi there! I'm Paul

I'm a recent university graduate in physics, and I love to learn. I spend my time reading, programming, and learning whatever comes across my way that interests me. You can find me around the web below:

<li style="display: inline;">
  <a href="mailto:l.nguyen.paul@gmail.com"><i class="fa fa-envelope fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://twitter.com/paululele"><i class="fa fa-twitter fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://instagram.com/paululele"><i class="fa fa-instagram fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://linkedin.com/in/lenpaul"><i class="fa fa-linkedin-square fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://github.com/lenpaul"><i class="fa fa-github-square fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
</li>

I started this website as a way to give back to people, and help other people learn. Below, you can find an archive of all the posts that I have written:

<div class="tiles">
{% for post in site.posts %}
	{% include post-list.html %}
{% endfor %}
</div><!-- /.tiles -->
