---
layout: default
title: CV
---

<div class="cv-jump-bar">
  <a href="#cv" class="cv-jump-link">CV</a>
  <span class="cv-jump-sep">|</span>
  <a href="#resume" class="cv-jump-link">Resume</a>
</div>

<div class="cv-layout">
  <div class="cv-row" id="cv">
    <div class="cv-section">
      <h2>Full CV</h2>
      <p>Download or view my full academic CV.</p>
      <a href="{{ '/assets/documents/cv.pdf' | relative_url }}" class="download-button" download>Download CV (PDF)</a>
    </div>
    <div class="pdf-viewer">
      <iframe src="{{ '/assets/documents/cv.pdf' | relative_url }}#toolbar=1" width="100%" height="840" title="Full CV"></iframe>
    </div>
  </div>
  <div class="cv-divider"></div>
  <div class="cv-row" id="resume">
    <div class="cv-section">
      <h2>Short Resume</h2>
      <p>Download or view my short resume.</p>
      <a href="{{ '/assets/documents/resume.pdf' | relative_url }}" class="download-button" download>Download Resume (PDF)</a>
    </div>
    <div class="pdf-viewer">
      <iframe src="{{ '/assets/documents/resume.pdf' | relative_url }}#toolbar=1" width="100%" height="840" title="Short Resume"></iframe>
    </div>
  </div>
</div>
