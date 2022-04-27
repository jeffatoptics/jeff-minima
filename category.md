---
layout: page
permalink: /category/
title: category
---

{% for cgy in site.categories %}
  <h3>{{ cgy[0] }}</h3>
  <ul>
    {% for post in cgy[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {{ post.excerpt }}
    {% endfor %}
  </ul>
{% endfor %}
