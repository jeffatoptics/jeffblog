---
layout: page
permalink: /category/
title: 📑
math: katex
---

<h6> {% for cgy in site.categories %} <a href="#{{ cgy[0] | slugify }}">{{ cgy[0] }} {%- if forloop.last == false %},{% endif -%}</a>{% endfor %}</h6>

{% for cgy in site.categories %}
  <h3 id="{{ cgy[0] | slugify }}">📑 {{ cgy[0] }}</h3>
  <ul>
    {% for post in cgy[1] %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {{ post.date | date: "%b %-d, %Y" }}
      {{ post.excerpt }}
    {% endfor %}
  </ul>
{% endfor %}
