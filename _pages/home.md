---
permalink: /
title: "Home"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% assign github_profile = site.author.github | default: "kimiko-11" %}

<div class="kc-home">
  <section class="kc-home__hero">
    <p class="kc-home__eyebrow">Portfolio</p>
    <h1>Kimaya Chavan</h1>
    <p class="kc-home__subtitle">AI · Computer Vision · Robotics · Perception</p>
    <p class="kc-home__intro">
      I am an engineering student focused on intelligent systems and physical AI, with interests across computer vision, robotics, and perception-driven autonomy.
    </p>
    <div class="kc-home__actions">
      <a class="kc-home__button" href="{{ '/portfolio/' | relative_url }}">Projects</a>
      <a class="kc-home__button" href="{{ '/publications/' | relative_url }}">Research</a>
      <a class="kc-home__button" href="{{ '/year-archive/' | relative_url }}">Lab Notes</a>
      <a class="kc-home__button" href="{{ '/cv/' | relative_url }}">Resume</a>
      <a class="kc-home__button" href="https://github.com/{{ github_profile }}">GitHub</a>
    </div>
  </section>

  <section>
    <h2>What I Build</h2>
    <ul class="kc-home__pill-list">
      <li>Computer Vision</li>
      <li>Robotics &amp; ROS2</li>
      <li>Deep Learning</li>
      <li>Embedded / IoT Systems</li>
      <li>Perception Systems</li>
    </ul>
  </section>

  <section>
    <h2>Featured Projects</h2>
    <div class="kc-home__cards">
      <article class="kc-home__card">
        <h3>Defense X-Ray Shell Detection &amp; Segmentation</h3>
        <p>Detection and segmentation workflows for defense X-ray imagery in constrained operational settings.</p>
      </article>
      <article class="kc-home__card">
        <h3>Connected IoT Vehicle</h3>
        <p>Embedded sensing and cloud-connected telemetry for a remotely monitored and controlled vehicle platform.</p>
      </article>
      <article class="kc-home__card">
        <h3>ROS2 Robotics</h3>
        <p>Modular robotics experiments using ROS2 for control, coordination, and perception integration.</p>
      </article>
      <article class="kc-home__card">
        <h3>Computer Vision Projects</h3>
        <p>Applied vision work spanning detection, tracking, segmentation, and model deployment.</p>
      </article>
    </div>
  </section>

  <section>
    <h2>Research</h2>
    <p>
      My current research direction centers on confidence-aware perception and robustness under distribution shift, with a focus on reliable perception systems for real-world robotics.
    </p>
  </section>
</div>

<style>
  .kc-home {
    margin-top: 0.5rem;
    color: #dde5f3;
  }

  .kc-home section {
    margin: 0 0 3.2rem;
  }

  .kc-home__hero {
    padding: 1.25rem 1.5rem;
    background: #0f1422;
    border: 1px solid #202b45;
    border-radius: 14px;
  }

  .kc-home__eyebrow {
    margin: 0;
    letter-spacing: 0.09em;
    text-transform: uppercase;
    font-size: 0.78rem;
    color: #8fa3c4;
  }

  .kc-home h1 {
    margin: 0.5rem 0 0.45rem;
    font-size: clamp(2rem, 4vw, 2.8rem);
    line-height: 1.12;
    color: #f6f9ff;
  }

  .kc-home__subtitle {
    margin: 0;
    color: #a9bcdc;
    font-size: 1rem;
    letter-spacing: 0.03em;
  }

  .kc-home__intro {
    margin: 1.25rem 0 0;
    max-width: 48rem;
    color: #d5deed;
    line-height: 1.75;
  }

  .kc-home__actions {
    margin-top: 1.45rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
  }

  .kc-home__button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 0.54rem 0.88rem;
    border-radius: 999px;
    border: 1px solid #314162;
    background: #141c2f;
    color: #e9efff !important;
    text-decoration: none;
    transition: transform 0.2s ease, border-color 0.2s ease, background 0.2s ease;
  }

  .kc-home__button:hover,
  .kc-home__button:focus {
    transform: translateY(-1px);
    border-color: #4d638b;
    background: #1a2640;
  }

  .kc-home h2 {
    margin: 0 0 0.9rem;
    color: #edf3ff;
    font-size: 1.35rem;
  }

  .kc-home__pill-list {
    margin: 0;
    padding: 0;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 0.65rem;
  }

  .kc-home__pill-list li {
    border: 1px solid #2b3754;
    background: #121a2d;
    border-radius: 999px;
    padding: 0.45rem 0.82rem;
    color: #d9e4f8;
  }

  .kc-home__cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(14rem, 1fr));
    gap: 0.85rem;
  }

  .kc-home__card {
    padding: 1rem;
    border: 1px solid #25324f;
    border-radius: 12px;
    background: #11182a;
  }

  .kc-home__card h3 {
    margin: 0 0 0.4rem;
    color: #eff4ff;
    font-size: 1rem;
  }

  .kc-home__card p,
  .kc-home section p {
    margin: 0;
    color: #cdd7e8;
    line-height: 1.7;
  }

  @media (max-width: 680px) {
    .kc-home__hero {
      padding: 1rem;
    }
  }
</style>
