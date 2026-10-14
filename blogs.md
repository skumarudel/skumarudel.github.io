---
layout: default
title: Blogs
---

# Blogs

<p class="projects-intro">Articles on data science, machine learning, AI, and physics.</p>

<div class="projects-list">
{% for post in site.data.blogs %}
  <article class="project-card blog-card">
    {% if post.image %}
    <div class="project-card-image">
      <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
    </div>
    {% endif %}
    <div class="project-card-body">
      <h2 class="project-card-title">{{ post.title }}</h2>
      {% if post.date %}<p class="blog-card-date">{{ post.date }}</p>{% endif %}
      <div class="project-card-description">{{ post.description | markdownify }}</div>
      <div class="project-card-links">
        <a href="{{ post.link }}" class="project-card-link" target="_blank" rel="noopener noreferrer">Read on Medium →</a>
      </div>
    </div>
  </article>
{% endfor %}
</div>
