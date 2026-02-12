---
layout: post
title: "Temp Fitness List"
permalink: /blog/2026-02-11-temp-fitness-list.html
header: false
thumbnail_url: "https://susangfink.github.io/site-images/assets/post1/susangfink-monday-weights-thumbnail.jpg"
gallery:
  - image: https://susangfink.github.io/site-images/assets/post1/susangfink-monday-weights.jpg
  - image: https://susangfink.github.io/site-images/assets/post1/susangfink-monday-weights-thumbnail.jpg
  - image: https://susangfink.github.io/site-images/assets/susangfink-cherry-blossom.jpg
excerpt_separator: "<!--more-->"  
categories: 
  - Health
---
<!--more-->

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
