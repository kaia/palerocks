---
layout: default
title: Blog | Kai Andresen
header: Blog
description: Kais tanker om livet og sånn
permalink: /blog/
---

{% for post in site.posts %}
  <p>{{ post.date | date: "%d/%m-%Y" }} <a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.description }}<br>
  </p>
{% endfor %}
