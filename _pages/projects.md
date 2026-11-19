---
layout: page
title: Projects
permalink: /projects/
description: Research benchmarks and applied computer vision projects.
nav: true
nav_order: 2
---

<div class="projects">
  <div class="row row-cols-1 row-cols-md-2">
    {% assign sorted_projects = site.projects | sort: 'importance' %}
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
