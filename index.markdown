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
          <img src="{{ '/assets/images/planner.png' | relative_url }}" alt="Financial Runway Planner overview: plan inputs, run-out risk and wealth metrics, and simulated current-dollar net worth paths">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>planner</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">A financial planning simulator that dynamically recommends an SPX beta for each year and wealth level to minimize depletion risk.</span>
        </span>
      </a>
      <a class="project-card" href="https://cardfolio.harrisonku.com/" target="_blank" rel="noopener noreferrer">
        <span class="project-image">
          <img src="{{ '/assets/images/cardfolio-harrison.png' | relative_url }}" alt="Cardfolio's Cards tab: my cardholder stats, a to-do list, and color-coded cards that need a decision or still owe a signup bonus">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>cardfolio</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">An open-source household credit-card tracker: color-coded cards that need a keep-or-close decision or still owe a signup bonus, per-card statement credits, product-change history, and 5/24 status.</span>
        </span>
      </a>
      <a class="project-card" href="https://fantasy.harrisonku.com/" target="_blank" rel="noopener noreferrer">
        <span class="project-image">
          <img src="{{ '/assets/images/fantasy.png' | relative_url }}" alt="Fantasy Desk's This week view: weekly win odds, a nine-category head-to-head scoreboard with each category's chance of winning by Sunday, and both teams' daily lineups">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>fantasy basketball</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">A fantasy basketball manager run by AI agents on top of a Python quant engine: projections, a draft optimizer, daily lineup optimization, and Monte Carlo matchup odds for each of the nine categories.</span>
        </span>
      </a>
      <a class="project-card" href="https://wayfarer.harrisonku.com/" target="_blank" rel="noopener noreferrer">
        <span class="project-image">
          <img src="{{ '/assets/images/wayfarer.png' | relative_url }}" alt="Wayfarer's unlock screen: a shared-key sign-in beside a photo of Venice's Grand Canal at sunset">
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>wayfarer</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">A private travel journal for two: places we've been and want to go, ranked by head-to-head comparisons into a shared score, with visit dates and notes. Installs on a phone's home screen.</span>
        </span>
      </a>
      <a class="project-card" href="https://github.com/vincentxu123/chord-ear-trainer" target="_blank" rel="noopener noreferrer">
        <span class="project-image project-image-text" aria-hidden="true">
          <span>I – V – vi – IV</span>
        </span>
        <span class="project-copy">
          <span class="project-heading"><strong>chord ear trainer</strong><span aria-hidden="true">↗</span></span>
          <span class="project-description">Practice hearing chord progressions as Roman numerals, using real songs, AI-generated clips, or piano. Built mostly by Vincent Xu (vincentxu.dev); I helped.</span>
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
