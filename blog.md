---
layout: default
title: Blog | Kai Andresen
header: Blog
description: Kais tanker om livet og sånn
permalink: /blog/
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.date | date: "%d/%m-%Y" }} {{ post.title }}</a><br>
  {{ post.description }}<br>
  </p>
{% endfor %}
