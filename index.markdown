---
layout: default
---

{% assign about = site.pages | where: "title", "about" | first %}

<section class="one-page-section" id="about">
  <h1>about</h1>
  {{ about.content | markdownify }}
</section>

<section class="one-page-section" id="projects">
  <h1>projects</h1>
  <div class="project-grid">
    <a class="project-card" href="https://planner.harrisonku.com/" target="_blank" rel="noopener noreferrer">
      <span class="project-image">
        <img src="{{ '/assets/images/planner.png' | relative_url }}" alt="Financial Runway Planner interface">
      </span>
      <span class="project-copy">
        <span class="project-heading"><strong>planner</strong><span aria-hidden="true">↗</span></span>
        <span class="project-description">A browser-based Monte Carlo simulator for exploring long-term financial plans against historical market returns.</span>
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
</section>

<section class="one-page-section" id="music">
  <h1>music</h1>
  {% include music-list.html %}
</section>
