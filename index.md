---
# index.md
layout: default
title: 首页
---

## 最新文章

<ul class="home-post-list">
  {% for post in site.posts %}
    <li>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <!-- <p>{{ post.excerpt }}</p> -->
      <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
    </li>
  {% endfor %}
</ul>