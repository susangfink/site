---
layout: page
title: Food
permalink: /categories/food/
collection: recipes
pagination:
  enabled: true
  categroy: food
  per_page: 3
---

{% for post in paginator.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}

<!-- Pagination links -->
<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">← Previous</a>
  {% endif %}

  {% for page_number in (1..paginator.total_pages) %}
    {% if page_number == paginator.page %}
      <span>{{ page_number }}</span>
    {% else %}
      <a href="{{ paginator.paginate_path | replace: ':num', page_number }}">{{ page_number }}</a>
    {% endif %}
  {% endfor %}

  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">Next →</a>
  {% endif %}
</div>
