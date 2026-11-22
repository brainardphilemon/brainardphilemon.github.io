---
layout: page
permalink: /blog/
title: blog
nav: true
nav_order: 2
---

<!-- post list markup from al-folio v0.13's _pages/blog.md -->
<ul class="post-list">
{% for post in site.posts %}
  {% assign read_time = post.content | strip_html | number_of_words | divided_by: 180 | plus: 1 %}
  {% assign year = post.date | date: "%Y" %}
  <li>
    <h3><a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.description }}</p>
    <p class="post-meta">
      {{ read_time }} min read &nbsp; &middot; &nbsp;
      {{ post.date | date: '%B %d, %Y' }}
    </p>
    <p class="post-tags">
      <a href="{{ year | prepend: '/blog/' | relative_url }}"> <i class="fa-solid fa-calendar fa-sm"></i> {{ year }} </a>
    </p>
  </li>
{% endfor %}
</ul>
