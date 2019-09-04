---
layout: blog
title: Blog
permalink: /blog/
---
{% for post in site.posts %}
  <h3><a href="{{ post.url }}">
 {{ post.title }}
  </a></h3>
  <p>
  <strong>{{ post.categories }}</strong> | {{ post.date | date_to_string }}
  <br>
  {{ post.description | truncate_words: 20 }}
</p>
<hr>
  {% endfor %}
