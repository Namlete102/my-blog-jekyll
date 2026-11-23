---
layout: default
title: Home
---
<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  </li>
{% endfor %}
</ul>