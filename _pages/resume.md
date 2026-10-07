---
layout: kc-page
title: "Resume"
permalink: /resume/
description: "Resume of Kimaya Chavan — education, projects, technical skills and research interests."
redirect_from:
  - /cv/
---

{%- assign cv_file = site.static_files | where: "path", "/files/Kimaya-Chavan-CV.pdf" | first -%}

<div class="kc-page">
<div class="kc-container">

<header class="kc-page__header">
<p class="kc-page__eyebrow">Curriculum Vitae</p>
<h1 class="kc-page__title">Resume</h1>
<p class="kc-page__intro">A concise overview of my education, projects, technical skills and research interests.</p>
{% if cv_file %}
<a class="kc-button" href="{{ cv_file.path | relative_url }}">Download PDF</a>
{% else %}
<a class="kc-button" href="mailto:{{ site.author.email }}?subject=Resume%20request">Request PDF by email</a>
{% endif %}
</header>

<section class="kc-section">
<h2>Education</h2>
<p><strong>B.Tech, Artificial Intelligence &amp; Data Science</strong><br>Dwarkadas J. Sanghvi College of Engineering — final year, CGPA 9.55</p>
<p>Building toward a career in physical AI, perception, computer vision, deep learning and robotics.</p>
</section>

<section class="kc-section">
<h2>Experience</h2>
<p>Perception Intern, Devise Electronics Pvt. Ltd. · Engineering &amp; AI Trainee, myEquation · Technical Committee and VCP Technical, DJS-ACM · Computer Vision Virtual Intern, YuvaIntern.</p>
</section>

<section class="kc-section">
<h2>Projects</h2>
<ul class="kc-tags">
<li>Defense X-Ray Shell Detection &amp; Segmentation</li>
<li>Connected Vehicle</li>
<li>ROS2 Robotics</li>
<li>Computer Vision &amp; AI Experiments</li>
</ul>
</section>

<section class="kc-section">
<h2>Technical skills</h2>
<p><strong>Languages:</strong> Python, C++, C, Embedded C, Java</p>
<p><strong>Libraries &amp; frameworks:</strong> ROS 2, OpenCV, NumPy, Pandas, scikit-learn</p>
<p><strong>Tools &amp; hardware:</strong> Git, Ubuntu, VS Code, CVAT, Arduino, ESP32/ESP8266, Raspberry Pi, MQTT, Salesforce</p>
</section>

<section class="kc-section">
<h2>Research interests</h2>
<p>Physical AI systems that can perceive, learn and act reliably in real-world environments.</p>
</section>

</div>
</div>
