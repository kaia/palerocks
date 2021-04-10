---
layout: default
title: Blog | Kai Andresen
header: Blog
description: Kais tanker om livet og sånn
permalink: /blog/
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.description }}<br>
  📅 {{ post.date | date_to_string }}</p>
{% endfor %}
