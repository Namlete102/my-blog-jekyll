---
layout: default
title: Untitled
---

Đây là nơi lưu trữ những bài viết, ghi chú của tôi, cũng như sưu tập về những bài viết được trình bày bởi các tác giả khác về lĩnh vực chuyên mà tôi yêu thích là toán học và đôi khi sẽ có cả vật lý, vì chúng cũng thật sự mang lại cảm giác thú vị, hấp dẫn và cảm hứng trong tôi.

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