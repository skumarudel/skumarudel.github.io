---
layout: default
title: About me
---
<div class="about-top">
  <div class="about-profile">
    <img src="/assets/images/ProfilePic-v3.png" alt="Sajan Kumar">
  </div>
  <div class="about-intro">
{{ site.data.bio.intro | markdownify }}
    <div class="cta-box">
      <strong>{{ site.data.bio.seeking }}</strong>
      <a class="cta-btn" href="{{ site.data.bio.linkedin }}" target="_blank" rel="noopener">Connect on LinkedIn</a>
    </div>
  </div>
  <figure class="about-veritas">
    <img src="/assets/images/veritas_img.jpg" alt="One of the four VERITAS telescopes at night">
    <figcaption>A VERITAS telescope at night</figcaption>
  </figure>
</div>

<div class="stats">
{% for stat in site.data.bio.stats %}
  <div><span>{{ stat.value }}</span>{{ stat.label }}</div>
{% endfor %}
</div>

<h2 class="skills-heading">{{ site.data.bio.skills_intro }}</h2>

<div class="skills-grid">
{% for skill in site.data.bio.skills %}
  <div class="skill-card">
    <h3>{{ skill.icon }} {{ skill.title }}</h3>
    <div class="chips">
      {% for item in skill.items %}<span>{{ item }}</span>{% endfor %}
    </div>
  </div>
{% endfor %}
</div>
