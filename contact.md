---
title: Contact
permalink: /contact/
layout: contact
---

## Email

{% if site.data.site.email %}
<p>
<a href="mailto:{{ site.data.site.email }}">{{ site.data.site.email }}</a>
</p>
{% endif %}

## Social Media

<div class="contact-social">

{% if site.data.site.facebook %}
<p>
<a href="{{ site.data.site.facebook }}" target="_blank">
Facebook
</a>
</p>
{% endif %}

{% if site.data.site.instagram %}
<p>
<a href="{{ site.data.site.instagram }}" target="_blank">
Instagram
</a>
</p>
{% endif %}

{% if site.data.site.bluesky %}
<p>
<a href="{{ site.data.site.bluesky }}" target="_blank">
Bluesky
</a>
</p>
{% endif %}

</div>
