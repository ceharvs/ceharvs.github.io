---
layout: default
permalink: /blog/
title: blog
description: Blog items
---

<div class="header-bar">
  <h1>Blog</h1>
  <!-- <h2>High Performance & Analytic Computing Engineer</h2>. -->
  <br/>
  <hr>
  <br/>
</div>


<ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>