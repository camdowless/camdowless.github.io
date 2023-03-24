---
layout: page
title: An Attempt at Documenting My Life
permalink: /blog/
---

<div class="article-container">
  {% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.date | date: '%B %d, %Y' }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
</div>
