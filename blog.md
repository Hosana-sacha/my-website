---
layout: default
title: Blog
permalink: 
---

<div class="blog-posts">
  {% for post in site.posts %}
    <div class="post-card">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">Read More</a>
    </div>
  {% endfor %}
</div>
