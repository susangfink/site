---
layout: page
title: Recipes
permalink: /recipes/
collection: recipes
entries_layout: grid
---

Welcome to my Recipes page! Here you'll find all my favorite recipes, organized by category.

{% for recipe in site.recipes %}
- {{ recipe.url | relative_url }}
[{{ recipe.title }}]({{ recipe.url }})
{% endfor %}
