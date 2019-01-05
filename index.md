---
title: Home
layout: default
---
Browse the stones below:

{% for lifting_stone in site.lifting_stones %}
  <h2>{{ lifting_stone.title }}</h2>
  <p>{{ lifting_stone.content }}</p>
  <a href="{{ lifting_stone.source }}" target="_blank">Source</a>
{% endfor %}
