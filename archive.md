---
bg: "tag.jpg"
layout: page
permalink: /posts/
title: "Projects"
crawlertitle: "Projects"
summary: "All projects I participated"
active: archive
---

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

  <h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>

  <ul class="year">
    {% for project in projects %}
      {% if project.tags contains t %}
        <li>
          {% if project.lastmod %}
            <a href="{{ post.url | relative_url}}">{{ project.title }}</a>
            <span class="date">{{ project.lastmod | date: "%d-%m-%Y"  }}</span>
          {% else %}
            <a href="{{ post.url | relative_url}}">{{ project.title }}</a>
            <span class="date">{{ project.date | date: "%d-%m-%Y"  }}</span>
          {% endif %}
        </li>
      {% endif %}
    {% endfor %}
  </ul>

{% endfor %}
