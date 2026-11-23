---
layout: default
title: Untitled
---

Những bài viết nháp toán học của tôi.

<hr>

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a> 
    <span class="post-date">({{ post.date | date: "%Y-%m-%d" }})</span>
    
    {% if post.excerpt %}
      <p class="post-excerpt">{{ post.excerpt | strip_html }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>