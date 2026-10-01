---
layout: archive
title: "Projects"
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

Portfolio of projects and implementations in Computer Vision, Robotics, and AI.

{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
