---
layout: page
title:
---

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
<!-- site_tags: {{ site_tags }} -->
{% assign tag_words = site_tags | split:',' | sort %}
<!-- tag_words: {{ tag_words }} -->

<div id="tags">

  <ul class="tag-box inline">
    {% for tag in tag_words) %}
      <li><a href="#{{ tag | cgi_escape }}">{{ tag }} <span>{{ site.tags[tag] | size }}</span></a></li>
    {% endfor %}
  </ul>

  {% for item in (0..site.tags.size) %}{% unless forloop.last %}

    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}

    <h2 id="{{ this_word | cgi_escape }}">{{ this_word }}</h2>

    <ul class="posts">

      {% for post in site.tags[this_word] %}{% if post.title != null %}

      <li itemscope>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d, %Y" }} - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
      </li>

      {% endif %}{% endfor %}

  </ul>

  {% endunless %}{% endfor %}

</div>
