---
layout: default
title: Updates | Style.css {}
header: Updates
description: Updates relating to the Style.css project.
permalink: /updates
---

<ul class="post-list">
  {% for post in site.posts %}
  {% if post.category != "Notes" %}
    <li>
      <a href="{{ post.url }}">{{ post.header }}</a><br>
      <span class="post-description">{{ post.description }}</span><br>
      <span class="post-meta">📅 {{ post.date | date_to_string }}</span>
    </li>
  {% endif %}
  {% endfor %}
</ul>