---
layout: archive
title: "About"
date:
modified:
excerpt:
image:
  feature: #about-me.jpg
  teaser:
  thumb:
share: false
ads: false
---

#### Hi there! I'm Paul

I am a recent university graduate in physics, and I love to learn. I spend my time reading, programming, and learning whatever comes across my way that interests me. You can see some of the things I'm working on over at <a href="https://github.com/LeNPaul">GitHub</a> and <a href="http://codepen.io/LeNPaul/">Codepen</a>, which I also talk about in <a href="{{ site.url }}/projects/">Projects</a>. You can find me over at <a href="https://www.quora.com/profile/Paul-Le-2">Quora</a>, where I typically answer questions on physics, programming, personal development, and productivity. I also run a blog on self-improvement on Quora, <a href="https://hungryminds.quora.com/">Hungry Minds</a>.

I love to learn, and believe online learning is the future of education. You can see my progress on <a href="https://www.khanacademy.org/profile/LeNPaul/">Khan Academy</a>, <a href="https://www.duolingo.com/LeNPaul">Duolingo</a>, <a href="https://www.freecodecamp.com/lenpaul">Free Code Camp</a>, and <a href="https://www.codecademy.com/LeNPaul">Codecademy</a>. I also love reading, which I track using <a href="https://www.goodreads.com/user/show/54220411-paul-le">Goodreads</a>.

You can find me around the web below (feel free to tweet at me!):

<ul style="display: inline;">
  <a href="mailto:l.nguyen.paul@gmail.com"><i class="fa fa-envelope fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://twitter.com/paululele"><i class="fa fa-twitter fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://instagram.com/paululele"><i class="fa fa-instagram fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://linkedin.com/in/lenpaul"><i class="fa fa-linkedin-square fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
  <a href="https://github.com/lenpaul"><i class="fa fa-github-square fa-2x" aria-hidden="true" style="padding:10px;"></i></a>
</ul>

I started this website as a way to give back to people, and help other people learn. Below, you can find an archive of all the posts that I have written:

<div class="tiles">
{% for post in site.posts %}
	{% include post-list.html %}
{% endfor %}
</div><!-- /.tiles -->
