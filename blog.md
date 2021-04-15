---
layout: default
title: kaisunivers.org
header: kaisunivers.org
description: litt om hva jeg får med meg, og hva jeg får ut av det
permalink: /blog/
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.date | date: "%d/%m-%Y" }} {{ post.title }}</a><br>
  {{ post.description }}<br>
    {% if post.oppdatert %}
    <mark>Oppdatert: {{ post.oppdatert }}</mark>
    {% endif %}

    {% if post.emner %}
      Emner:
      {% for emne in post.emner %}
        <mark>{{ emne }}</mark>&nbsp;
      {% endfor %}
    {% endif %}
  </p>
{% endfor %}
