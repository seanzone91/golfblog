---
layout: default
title: Blog
lang: de
permalink: /de/blog/
---

# Blog (Deutsch)

{% assign posts_de = site.posts | where: "lang", "de" %}

<ul>
  {% for post in posts_de %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> – {{ post.date | date: "%d.%m.%Y" }}</small>
    </li>
  {% endfor %}
</ul>
