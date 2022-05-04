---
layout: page
permalink: /category/
title: 📑
math: katex
---

{% for cgy in site.categories %}
  <div class="categroy-group">
  <div id="#{{ cgy[0] | slugize }}"></div>
    <h3>{{ cgy[0] }}</h3>
    <ul>
      {% for post in cgy[1] %}
        <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
        {{ post.date | date: "%b %-d, %Y" }}
        {{ post.excerpt }}
      {% endfor %}
    </ul>
  </div>
{% endfor %}
