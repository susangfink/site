---
layout: collection
title: Recipes
permalink: /site/recipes/
collection: recipes
entries_layout: grid
---

Welcome to my Recipes page! Here you'll find all my favorite recipes, organized by category.

{% for recipe in site.recipes %}
- [{{ recipe.title }}]({{ recipe.url }})
{% endfor %}
