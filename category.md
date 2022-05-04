---
layout: page
permalink: /category/
title: 📑
math: katex
---

{% for cgy in site.categories %}
  <h3 id="{{ cgy[0] | slugize }}">{{ cgy[0] }}</h3>
  <ul>
    {% for post in cgy[1] %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {{ post.date | date: "%b %-d, %Y" }}
      {{ post.excerpt }}
    {% endfor %}
  </ul>
{% endfor %}


