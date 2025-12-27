---
layout: post
title: Photo Gallery

gallery:
  - image: /assets/images/washDC_gallery/washDC-1.jpg
    alt: "Image AA"
  - image: /assets/images/washDC_gallery/washDC-2.jpg
    alt: "Image BB"
  - image: /assets/images/washDC_gallery/washDC-3.jpg 
    alt: "Image CC"
  - image: /assets/images/washDC_gallery/washDC-4.jpg
    alt: "Image DD"
  - image: /assets/images/washDC_gallery/washDC-5.jpg
    alt: "Image EE"
  - image: /assets/images/washDC_gallery/washDC-6.jpg
    alt: "Image FF"

excerpt_separator: "<!--more-->"  
categories: 
- Photography
- Travel Pictures
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
