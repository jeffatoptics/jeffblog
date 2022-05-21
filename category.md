---
layout: page-simple
permalink: /category/
title: 📑
math: katex
---
![logo](./assets/logo.png){: width="150"}<br><br>
{% for cgy in site.categories %} <a class="post-list-heading" href="#{{ cgy[0] | slugify }}">{{ cgy[0] }} {%- if forloop.last == false %},{% endif -%}</a>{% endfor %}

{% for cgy in site.categories %}
  <h3 id="{{ cgy[0] | slugify }}">📑 {{ cgy[0] }}</h3>
  <ul>
    {% for post in cgy[1] %}
      <li><a class="post-link" href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {{ post.date | date: "%b %-d, %Y" }}
      {{ post.excerpt }}
    {% endfor %}
  </ul>
{% endfor %}
