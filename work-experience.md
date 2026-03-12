---
layout: default
title: Work
---

<section class="page-content">
  <div class="profile-container">
    <div class="profile-image">
      <img src="/assets/images/ProfilePic-v3.png" alt="Sajan Kumar">
    </div>
  </div>

  <div class="jobs">
  <!--  <p class="subtitle">Experience and Awards</p> -->
  <p>The Very Energetic Radiation Imaging Telescope Array System (<a href="https://veritas.sao.arizona.edu" target="_blank" rel="noopener noreferrer">VERITAS</a>) is a ground-based observatory in Arizona that studies powerful explosions and extreme events in the universe. Using four large Cherenkov telescopes, it detects very high-energy gamma rays during clear, dark nights.</p>

<p>The High-Altitude Water Cherenkov Observatory (<a href="https://www.hawc-observatory.org" target="_blank" rel="noopener noreferrer">HAWC</a>), located in Mexico, is a unique ground-based facility that observes gamma rays and cosmic rays from space. Instead of traditional telescopes, it uses a large array of water-filled detectors to continuously monitor the sky, helping scientists study some of the most energetic and dramatic events in the universe.</p>

    {% for job in site.data.work.experience %}
    <div class="job-item">
      <div class="job-left">
        <h3>{{ job.title }}</h3>
      </div>
      <div class="job-middle">
    <p>{{ job.period }} <span class="institution">({{ job.institution }})</span></p>
    </div>

      <div class="job-right">
        <ul>
          {% for detail in job.details %}
          <li>{{ detail }}</li>
          {% endfor %}
        </ul>
      </div>
    </div>

    {% unless forloop.last %}
    <div class="job-divider"></div>
    {% endunless %}
    {% endfor %}
  </div>
</section>

