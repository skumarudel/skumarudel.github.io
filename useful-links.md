---
layout: default
title: Useful Links
---

# Useful Links

<div class="links-list">
{% for link in site.data.links.links %}
  <a href="{{ link.url }}" class="link-card" target="_blank" rel="noopener noreferrer">
    <span class="link-card-title">{{ link.title }}</span>
    {% if link.description %}
    <span class="link-card-desc">{{ link.description }}</span>
    {% endif %}
  </a>
{% endfor %}
</div>
