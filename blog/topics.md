---
layout: page
title: Topics
permalink: /topics/
gallery:
  - image: /assets/images/topic-thumbnails/susangfink-topics-home-thumbnail.jpg
    alt: "Image AA"
    caption: "Home"
  - image: /assets/images/topic-thumbnails/susangfink-topics-health-gym-thumbnail.jpg
    alt: "Image BB"
  - image: /assets/images/topic-thumbnails/susangfink-topics-family-thumbnail.jpg 
    alt: "Image CC"
  - image: /assets/images/topic-thumbnails/susangfink-topics-food-thumbnail.jpg
    alt: "Image DD"
  - image: /assets/images/topic-thumbnails/susangfink-topics-reflection-thumbnail.jpg
    alt: "Image EE"
  - image: /assets/images/topic-thumbnails/susangfink-topics-travel-thumbnail.jpg
    alt: "Image FF"

excerpt_separator: "<!--more-->"   
---

<!--more-->

{% include posts-paginated.html %}

<!--
{% if page.gallery %}
<div class="photo-journal">
  {% for photo in page.gallery %}
    <figure>
      <a href="{{ photo.image | relative_url }}" data-lightbox="journal">
        <img
          src="{{ photo.image | relative_url }}"
          loading="lazy"
          alt="{{ photo.alt }}">
      </a>
    </figure>
  {% endfor %}
</div>
{% endif %}
-->
