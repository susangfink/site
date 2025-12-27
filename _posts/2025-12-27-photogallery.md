---
layout: post
title: Photo Gallery

gallery:
  - image: /assets/images/washDC_gallery/washdc-1.jpg
    alt: "Image A"
  - image: /assets/images/washDC_gallery/washdc-2.jpg
    alt: "Image B"
  - image: /assets/images/washDC_gallery/washdc-3.jpg 
    alt: "Image C"
  - image: /assets/images/washDC_gallery/washdc-4.jpg
    alt: "Image D"
  - image: /assets/images/washDC_gallery/washdc-5.jpg
    alt: "Image E"
  - image: /assets/images/washDC_gallery/washdc-6.jpg
    alt: "Image F"

excerpt_separator: "<!--more-->"  
categories: 
- Photography
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
