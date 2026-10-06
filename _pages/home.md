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
  <aside class="kc-home__sidebar" aria-label="Profile">
    <img class="kc-home__avatar" src="{{ '/images/profile.png' | relative_url }}" alt="Kimaya Chavan profile photo" />
    <h1 class="kc-home__name">Kimaya Chavan</h1>
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
  </aside>

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
    --kc-border: #d8dee4;
    margin-top: 0.5rem;
    display: grid;
    grid-template-columns: minmax(16rem, 28%) minmax(0, 72%);
    gap: 2rem;
    color: var(--kc-text);
    background: var(--kc-bg);
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }

  .kc-home__sidebar {
    border: 1px solid var(--kc-border);
    padding: 1rem;
    background: #fff;
  }

  .kc-home__avatar {
    display: block;
    width: 100%;
    max-width: 190px;
    height: auto;
    border: 1px solid var(--kc-border);
    margin-bottom: 1rem;
  }

  .kc-home__name {
    margin: 0;
    font-size: 1.55rem;
    font-weight: 620;
    color: var(--kc-text);
  }

  .kc-home__focus {
    margin: 0.65rem 0 1rem;
    color: var(--kc-muted);
    line-height: 1.5;
  }

  .kc-home__bio {
    margin: 0 0 0.9rem;
    color: var(--kc-text);
    line-height: 1.6;
  }

  .kc-home__bio--secondary {
    color: var(--kc-muted);
  }

  .kc-home__links {
    margin-top: 1.2rem;
    padding-top: 1rem;
    border-top: 1px solid var(--kc-border);
    display: grid;
    gap: 0.5rem;
  }

  .kc-home__links a,
  .kc-home__links span {
    color: var(--kc-text);
    text-decoration: none;
    width: fit-content;
  }

  .kc-home__links a:hover,
  .kc-home__links a:focus {
    color: var(--kc-accent);
  }

  .kc-home__links span {
    color: var(--kc-muted);
  }

  .kc-home__content {
    min-width: 0;
  }

  .kc-home__intro-label {
    margin: 0;
    font-size: 0.75rem;
    letter-spacing: 0.08em;
    color: var(--kc-accent);
    font-weight: 600;
  }

  .kc-home__intro h2 {
    margin: 0.45rem 0 0.7rem;
    font-size: 1.8rem;
    font-weight: 620;
    color: var(--kc-text);
  }

  .kc-home__intro p {
    margin: 0;
    color: var(--kc-muted);
    line-height: 1.6;
    max-width: 56ch;
  }

  .kc-home__tags {
    margin: 1rem 0 0;
    padding: 0;
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
  }

  .kc-home__tags li {
    border: 1px solid var(--kc-border);
    padding: 0.22rem 0.5rem;
    font-size: 0.74rem;
    letter-spacing: 0.06em;
    color: var(--kc-muted);
  }

  .kc-home__tabs {
    margin: 1.4rem 0;
    display: flex;
    flex-wrap: wrap;
    gap: 1.2rem;
    border-bottom: 1px solid var(--kc-border);
    padding-bottom: 0.35rem;
  }

  .kc-home__tabs a {
    color: var(--kc-muted);
    text-decoration: none;
    padding-bottom: 0.45rem;
    border-bottom: 2px solid transparent;
    font-weight: 500;
  }

  .kc-home__tabs a:hover,
  .kc-home__tabs a:focus,
  .kc-home__tabs a.is-active {
    color: var(--kc-text);
    border-bottom-color: var(--kc-accent);
  }

  .kc-home__projects h3 {
    margin: 0 0 1rem;
    font-size: 1.25rem;
    color: var(--kc-text);
  }

  .kc-home__project {
    border-top: 1px solid var(--kc-border);
    padding: 1rem 0;
  }

  .kc-home__project:last-child {
    border-bottom: 1px solid var(--kc-border);
  }

  .kc-home__project-number {
    margin: 0;
    color: var(--kc-accent);
    font-size: 0.73rem;
    letter-spacing: 0.08em;
    font-weight: 600;
  }

  .kc-home__project h4 {
    margin: 0.3rem 0 0.45rem;
    font-size: 1.08rem;
    color: var(--kc-text);
  }

  .kc-home__project p {
    margin: 0;
    color: var(--kc-muted);
    line-height: 1.6;
  }

  .kc-home__detail {
    margin-top: 0.45rem !important;
  }

  .kc-home__meta,
  .kc-home__position {
    margin-top: 0.4rem !important;
    font-size: 0.86rem;
  }

  .kc-home__meta {
    color: var(--kc-text) !important;
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
  }

  @media (max-width: 980px) {
    .kc-home {
      grid-template-columns: 1fr;
      gap: 1.25rem;
    }

    .kc-home__avatar {
      max-width: 150px;
    }

    .kc-home__tabs {
      gap: 1rem;
      overflow-x: auto;
    }
  }
</style>
