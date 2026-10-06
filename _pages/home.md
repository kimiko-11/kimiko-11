---
permalink: /
title: "Home"
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

{% assign github_profile = site.author.github | default: "kimiko-11" %}
{% assign linkedin_profile = site.author.linkedin %}

<div class="kc-home">
  <header class="kc-home__hero">
    <div class="kc-home__hero-inner">
      <div class="kc-home__photo-wrap" aria-label="Kimaya Chavan profile photo placeholder">
        <span class="kc-home__initials" aria-hidden="true">KC</span>
        <img class="kc-home__photo" src="{{ '/images/profile.png' | relative_url }}" alt="Kimaya Chavan profile photo" onerror="this.style.display='none'" />
        <!-- Replace the placeholder with the real photo later, keeping this path: {{ '/images/profile.png' | relative_url }} -->
      </div>

      <div class="kc-home__profile">
        <h1>Kimaya Chavan</h1>
        <p class="kc-home__focus">Physical AI · Computer Vision · Deep Learning · Robotics</p>
        <p class="kc-home__bio">I build intelligent systems that combine perception, learning, and robotics to interact with the physical world.</p>
        <p class="kc-home__bio kc-home__bio--secondary">My work spans computer vision, deep learning and robotics, with hands-on experience in embedded and connected systems.</p>

        <nav class="kc-home__links" aria-label="Profile links">
          <a href="https://github.com/{{ github_profile }}">GitHub</a>
          {% if linkedin_profile %}
          <a href="https://www.linkedin.com/in/{{ linkedin_profile }}">LinkedIn</a>
          {% else %}
          <span>LinkedIn</span>
          {% endif %}
          <a href="mailto:{{ site.author.email }}">Email</a>
          <a href="{{ '/cv/' | relative_url }}">Resume</a>
        </nav>
      </div>
    </div>
  </header>

  <main class="kc-home__content">
    <section class="kc-home__intro">
      <p class="kc-home__intro-label">PERCEIVE → LEARN → ACT</p>
      <h2>Building toward Physical AI</h2>
      <p>I’m interested in how machines perceive the world, learn from data, and turn that understanding into physical action.</p>
      <ul class="kc-home__tags" aria-label="Focus areas">
        <li>PHYSICAL AI</li>
        <li>COMPUTER VISION</li>
        <li>DEEP LEARNING</li>
        <li>ROBOTICS</li>
      </ul>
    </section>

    <nav class="kc-home__tabs" aria-label="Sections">
      <a href="{{ '/year-archive/' | relative_url }}">Notes</a>
      <a class="is-active" href="{{ '/portfolio/' | relative_url }}" aria-current="page">Projects</a>
      <a href="{{ '/publications/' | relative_url }}">Research</a>
      <a href="{{ '/cv/' | relative_url }}">Resume</a>
    </nav>

    <section class="kc-home__projects" id="selected-projects">
      <h3>Selected Projects</h3>

      <article class="kc-home__project">
        <p class="kc-home__project-number">01</p>
        <h4>Defense X-Ray Shell Detection &amp; Segmentation</h4>
        <p>A computer vision system for detecting, counting and segmenting shells in X-ray tray imagery for automated inspection.</p>
        <p class="kc-home__meta">Python · OpenCV · CVAT · YOLO</p>
        <p class="kc-home__position">Computer Vision · Perception · Physical AI</p>
      </article>

      <article class="kc-home__project">
        <p class="kc-home__project-number">02</p>
        <h4>Connected Vehicle</h4>
        <p>An IoT vehicle combining physical sensors, ESP32/Raspberry Pi hardware and cloud communication.</p>
        <p class="kc-home__detail">Architectures: (1) Raspberry Pi + ESP32 + Salesforce Platform Events; (2) ESP32 + MQTT + Salesforce.</p>
        <p class="kc-home__meta">ESP32 · Raspberry Pi · MQTT · Salesforce</p>
        <p class="kc-home__position">Robotics · Physical Systems · Embedded Systems</p>
      </article>

      <article class="kc-home__project">
        <p class="kc-home__project-number">03</p>
        <h4>ROS2 Robotics</h4>
        <p>Hands-on work with ROS2 communication, publishers, subscribers, nodes and robotic system architecture.</p>
        <p class="kc-home__meta">ROS2 Humble · Python · Linux</p>
        <p class="kc-home__position">Robotics · Physical AI</p>
      </article>

      <article class="kc-home__project">
        <p class="kc-home__project-number">04</p>
        <h4>Computer Vision &amp; AI Experiments</h4>
        <p>Experiments covering image processing, image representations, deep learning and computer vision.</p>
        <p class="kc-home__meta">Python · NumPy · OpenCV · Deep Learning</p>
        <p class="kc-home__position">Computer Vision · Deep Learning</p>
      </article>
    </section>
  </main>
</div>

<style>
  .kc-home {
    --kc-bg: #ffffff;
    --kc-text: #1f2328;
    --kc-muted: #656d76;
    --kc-accent: #f26a21;
    --kc-dark-orange: #d9561a;
    --kc-border: #d8dee4;
    margin-top: 0.5rem;
    color: var(--kc-text);
    background: var(--kc-bg);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }

  .kc-home__hero {
    width: 100vw;
    margin-left: calc(50% - 50vw);
    box-sizing: border-box;
    padding: 2.75rem 1.5rem;
    background: var(--kc-accent);
    color: #ffffff;
  }

  .kc-home__hero-inner {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    gap: 2rem;
  }

  .kc-home__photo-wrap {
    position: relative;
    flex: 0 0 200px;
    width: 200px;
    height: 200px;
    overflow: hidden;
    border: 2px solid #ffffff;
    border-radius: 6px;
    background: var(--kc-dark-orange);
    display: grid;
    place-items: center;
  }

  .kc-home__initials {
    color: #ffffff;
    font-size: 3rem;
    font-weight: 700;
    letter-spacing: 0.04em;
  }

  .kc-home__photo {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 4px;
  }

  .kc-home__profile {
    min-width: 0;
  }

  .kc-home__profile h1 {
    margin: 0;
    color: #ffffff;
    font-size: 2.1rem;
    line-height: 1.15;
    font-weight: 650;
  }

  .kc-home__focus {
    margin: 0.55rem 0 1.1rem;
    color: #ffffff;
    font-size: 1rem;
    line-height: 1.5;
  }

  .kc-home__bio {
    max-width: 70ch;
    margin: 0 0 0.7rem;
    color: #ffffff;
    font-size: 1rem;
    line-height: 1.6;
  }

  .kc-home__bio--secondary {
    margin-bottom: 0;
    color: #fff4ed;
  }

  .kc-home__links {
    margin-top: 1.25rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem 1.1rem;
  }

  .kc-home__links a,
  .kc-home__links span {
    color: #ffffff;
    font-size: 0.95rem;
    text-decoration: none;
  }

  .kc-home__links a:hover,
  .kc-home__links a:focus {
    text-decoration: underline;
  }

  .kc-home__links span {
    opacity: 0.78;
  }

  .kc-home__content {
    max-width: 1200px;
    margin: 0 auto;
    padding: 3rem 1.5rem 4rem;
    box-sizing: border-box;
  }

  .kc-home__intro-label {
    margin: 0;
    color: var(--kc-accent);
    font-size: 0.85rem;
    letter-spacing: 0.08em;
    font-weight: 650;
  }

  .kc-home__intro h2 {
    margin: 0.55rem 0 0.75rem;
    color: var(--kc-text);
    font-size: 2.1rem;
    line-height: 1.2;
    font-weight: 650;
  }

  .kc-home__intro > p:not(.kc-home__intro-label) {
    max-width: 68ch;
    margin: 0;
    color: var(--kc-muted);
    font-size: 1rem;
    line-height: 1.65;
  }

  .kc-home__tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin: 1.25rem 0 0;
    padding: 0;
    list-style: none;
  }

  .kc-home__tags li {
    padding: 0.3rem 0.55rem;
    border: 1px solid var(--kc-accent);
    color: var(--kc-muted);
    font-size: 0.85rem;
    letter-spacing: 0.06em;
  }

  .kc-home__tabs {
    display: flex;
    flex-wrap: wrap;
    gap: 1.35rem;
    margin: 2rem 0 2.4rem;
    border-bottom: 1px solid var(--kc-border);
  }

  .kc-home__tabs a {
    padding-bottom: 0.55rem;
    border-bottom: 2px solid transparent;
    color: var(--kc-muted);
    font-size: 0.9rem;
    text-decoration: none;
  }

  .kc-home__tabs a:hover,
  .kc-home__tabs a:focus,
  .kc-home__tabs a.is-active {
    color: var(--kc-text);
    border-bottom-color: var(--kc-accent);
  }

  .kc-home__projects h3 {
    margin: 0 0 1.35rem;
    color: var(--kc-text);
    font-size: 1.45rem;
    line-height: 1.25;
    font-weight: 650;
  }

  .kc-home__projects h3::after {
    display: block;
    width: 48px;
    height: 3px;
    margin-top: 0.7rem;
    background: var(--kc-accent);
    content: "";
  }

  .kc-home__project {
    padding: 1.25rem 0;
    border-top: 1px solid var(--kc-border);
  }

  .kc-home__project:last-child {
    border-bottom: 1px solid var(--kc-border);
  }

  .kc-home__project .kc-home__project-number {
    margin: 0;
    color: var(--kc-accent);
    font-size: 0.85rem;
    letter-spacing: 0.08em;
    font-weight: 650;
  }

  .kc-home__project h4 {
    margin: 0.35rem 0 0.5rem;
    color: var(--kc-text);
    font-size: 1.15rem;
    line-height: 1.35;
    font-weight: 650;
  }

  .kc-home__project p {
    margin: 0;
    color: var(--kc-muted);
    font-size: 1rem;
    line-height: 1.65;
  }

  .kc-home__detail {
    margin-top: 0.45rem !important;
  }

  .kc-home__meta,
  .kc-home__position {
    margin-top: 0.45rem !important;
    font-size: 0.85rem !important;
  }

  .kc-home__meta {
    color: var(--kc-text) !important;
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
  }

  @media (max-width: 759px) {
    .kc-home__hero {
      padding: 2.25rem 1.25rem;
    }

    .kc-home__hero-inner {
      align-items: flex-start;
      flex-direction: column;
      gap: 1.25rem;
    }

    .kc-home__photo-wrap {
      flex-basis: 160px;
      width: 160px;
      height: 160px;
    }

    .kc-home__content {
      padding: 2.25rem 1.25rem 3rem;
    }

    .kc-home__intro h2 {
      font-size: 1.85rem;
    }
  }
</style>
