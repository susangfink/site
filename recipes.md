---
layout: page
title: Recipes
permalink: /recipes/
---

Welcome to my Recipes page! Here you'll find all my favorite recipes, organized by category.

{% for recipe in site.recipes %}
- [{{ recipe.title }}]({{ recipe.url }})
{% endfor %}
