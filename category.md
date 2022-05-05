---
layout: page
permalink: /category/
title: Category
math: katex
---
<span> {% for cgy in site.categories %} <a href="#{{ cgy[0] | slugify }}">{{ cgy[0] }}</a> {% endfor %} </span>

{% for cgy in site.categories %}
  <h3 id="{{ cgy[0] | slugify }}">{{ cgy[0] }}</h3>
  <ul>
    {% for post in cgy[1] %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {% comment %}
      {{ post.date | date: "%b %-d, %Y" }}
      {{ post.excerpt }}
      {% endcomment %}
    {% endfor %}
  </ul>
{% endfor %}


