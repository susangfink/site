---
layout: page
title: Blog
permalink: /blog/
show_excerpts: true
entries_layout: list
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
