---
title: Gallery
permalink: /gallery/
layout: page
---

Photos from rallies, vigils, meetings, and community events.

<div class="gallery-grid">
  {% assign photos = site.gallery | sort: "date" | reverse %}
  {% for item in photos %}
    <figure class="gallery-item">
      <img src="{{ item.image | relative_url }}" alt="{{ item.alt | default: item.title }}">
      <figcaption>
        <strong>{{ item.title }}</strong>
        {% if item.caption %}
          <div>{{ item.caption }}</div>
        {% endif %}
      </figcaption>
    </figure>
  {% endfor %}
</div>
