---
title: Home
layout: default
---
Browse the stones below:

{% for lifting_stone in site.lifting_stones %}
  <div class="stone-teaser clearfix">
    <div class="img-left teaser-image">
      <a href="{{ lifting_stone.url }}" alt="go to the detail page"><img src="{{ lifting_stone.image }}" alt="photo of {{ lifting_stone.title }}" /></a>
    </div>
    <div class="teaser-content">
      <h2><a href="{{ lifting_stone.url }}" alt="go to the detail page">{{ lifting_stone.title }}</a></h2>
      <p>{{ lifting_stone.content }}</p>
      <p><small>Weight category: <em>{{ lifting_stone.category }}</em></small></p>
      <p><a href="{{ lifting_stone.source }}" target="_blank">Source</a></p>
    </div>
  </div>
{% endfor %}