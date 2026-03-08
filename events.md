---
title: Events
permalink: /events/
layout: page
---

<ul class="event-list">
  {% assign sorted_events = site.events | sort: "date" | reverse %}
  {% for event in sorted_events %}
    <li class="event-list-item">
      <h2><a href="{{ event.url }}">{{ event.title }}</a></h2>
      <p>{{ event.date | date: "%A, %B %-d, %Y at %-I:%M %p" }}</p>
      {% if event.location %}<p>{{ event.location }}</p>{% endif %}
      <p>{{ event.excerpt | strip_html | truncate: 160 }}</p>
    </li>
  {% endfor %}
</ul>
