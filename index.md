---
bg: "journal.jpg"
layout: default
crawlertitle: "Programmer's Toolkit"
title: "Home"
summary: ""
---

{% for post in site.posts limit: 6 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
