---
layout: default
title: Start
lang: de
permalink: /de/
---

# Willkommen auf meinem Golfblog

Hier teile ich praxisnahe Notizen zu Training, Strategie und Platzmanagement – plus kleine digitale Tools rund um Golf.

## Themen
- Training (Range, Kurzspiel, Putting)
- Strategie & Course Management
- Platzberichte und Learnings
- Tools & digitale Produkte (z. B. Scorecards)

## Neueste Beiträge

{% assign posts_de = site.posts | where: "lang", "de" %}

<ul>
  {% for post in posts_de limit: 5 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> – {{ post.date | date: "%d.%m.%Y" }}</small>
    </li>
  {% endfor %}
</ul>

[Alle Beiträge ansehen]({{ '/de/blog/' | relative_url }})
