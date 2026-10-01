---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% include base_path %}

Research papers, publications, and studies.

{% for post in site.publications %}
  {% include archive-single.html %}
{% endfor %}
