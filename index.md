---
layout: default
title: "Inicio"
---
<h1>Bienvenido a mi blog</h1>

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
  </li>
{% endfor %}
</ul>
