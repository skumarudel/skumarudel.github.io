---
layout: default
title: Projects
---

# My Projects

<p class="projects-intro">Fun projects that convey data science ideas in an accessible way. This page is continuously updated and always in progress—new projects and demos are added as I build them.</p>

<div class="projects-list">
{% for project in site.data.projects %}
  <article class="project-card">
    {% if project.image %}
    <div class="project-card-image">
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
    </div>
    {% endif %}
    <div class="project-card-body">
      <h2 class="project-card-title">{{ project.title }}</h2>
      <div class="project-card-description">{{ project.description | markdownify }}</div>
      <div class="project-card-links">
      {% if project.liveLink %}
      <a href="{{ project.liveLink }}" class="project-card-link project-card-link--live" target="_blank" rel="noopener noreferrer">Live demo →</a>
      {% endif %}
      {% if project.githubLink %}
      <a href="{{ project.githubLink }}" class="project-card-link" target="_blank" rel="noopener noreferrer">View on GitHub →</a>
      {% endif %}
      </div>
    </div>
  </article>
{% endfor %}
</div>
