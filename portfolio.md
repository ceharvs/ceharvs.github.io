---
layout: page
title: portfolio
permalink: /portfolio/
---

{% for project in site.portfolio reversed %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}

<br/>
<hr/>
<br/>
<span class="contacticon center">
  <a href="https://orcid.org/0000-0002-3941-3895" target="_blank"><i class="fa fa-fingerprint"></i></a>
  <a href="https://github.com/ceharvs" target="_blank"><i class="fa fa-github-square"></i></a>
  <a href="https://www.linkedin.com/in/itsharveytime" target="_blank"><i class="fa fa-linkedin"></i></a>
  <a href="https://twitter.com/ItsHarveyTime" target="_blank"><i class="fa fa-twitter-square"></i></a>
  <a href="https://www.instagram.com/itsharveytime/" target="_blank"><i class="fa fa-instagram"></i></a>
</span>

<div class="col three caption">
  The best way to reach me is through e-mail or a LinkedIn message.
</div>
