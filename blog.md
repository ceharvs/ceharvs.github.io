---
layout: default
permalink: /blog/
title: blog
description: Blog items
---

<ul class="post-list">
{% for b in site.blog reversed %}
    <li>
        <h2><a class="blog-title" href="{{ blog.url | prepend: site.baseurl }}">{{ blog.title }}</a></h2>
        <p class="post-meta">{{ blog.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>