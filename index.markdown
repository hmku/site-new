---
layout: default
---

{% assign about = site.pages | where: "title", "about" | first %}

<section class="one-page-section" id="about">
  <h1>about</h1>
  <div class="section-content about-copy">
    {{ about.content | markdownify }}
    <nav class="about-links" aria-label="Social profiles">
      <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer">GitHub <span aria-hidden="true">↗</span></a>
      <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" rel="noopener noreferrer">LinkedIn <span aria-hidden="true">↗</span></a>
    </nav>
  </div>
</section>

<section class="one-page-section" id="projects">
  <h1>projects</h1>
  <div class="section-content">
    <div class="project-grid">
      <a class="project-card" href="https://planner.harrisonku.com/" target="_blank" rel="noopener noreferrer">
        <span class="project-image">
          <img src="{{ '/assets/images/planner.png' | relative_url }}" alt="Financial Runway Planner interface">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>planner</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">A financial planning simulator that dynamically recommends an SPX beta for each year and wealth level to minimize depletion risk.</span>
        </span>
      </a>
      <a class="project-card" href="https://cardfolio.harrisonku.com/" target="_blank" rel="noopener noreferrer">
        <span class="project-image">
          <img src="{{ '/assets/images/cardfolio.png' | relative_url }}" alt="Cardfolio portfolio overview">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>cardfolio</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">A private household credit-card tracker for accounts, annual fees, recurring benefits, and 5/24 status.</span>
        </span>
      </a>
    </div>
  </div>
</section>

<section class="one-page-section" id="music">
  <h1>music</h1>
  <div class="section-content">
    {% include music-list.html %}
  </div>
</section>
