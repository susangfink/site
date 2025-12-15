---
layout: page
title: Categories
permalink: /categories/
---

Here you can browse all posts by category:

{% assign categories = site.categories | sort %}
<ul>
  {% for category in categories %}
    <li>
      <a href="{{ '/categories/' | append: category[0] | relative_url }}">
        {{ category[0] | capitalize }} ({{ category[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>
