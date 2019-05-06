---
bg: "tag.jpg"
layout: default
permalink: /projects/
title: "Projects"
crawlertitle: "Projects"
summary: "All projects I participated"
active: archive
---

{% for post in site.posts %}
{% if post.categories contains "projects" %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endif %}
{% endfor %}
