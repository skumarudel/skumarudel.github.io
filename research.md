---
layout: default
title: Research
---

# My Research Projects

<section class="page-content">
  <div class="jobs">
    {% for topic in site.data.research.topics %}
      {% if topic.title == "Machine Learning" or topic.title == "Project Management & Leadership" %}
    <div class="job-item">
      <div class="job-left">
        <h3>{{ topic.title }}</h3>
      </div>
      <div class="job-middle">
        <p></p>
      </div>
      <div class="job-right">
        <ul>
          {% for detail in topic.details %}
          <li>{{ detail }}</li>
          {% endfor %}
        </ul>
      </div>
    </div>
      {% if topic.title == "Machine Learning" %}
    <div class="job-divider"></div>
      {% endif %}
      {% endif %}
    {% endfor %}
  </div>
</section>
