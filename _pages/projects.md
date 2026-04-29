---
layout: page
title: conferences
permalink: /conferences/
description: Conference presentations and academic events.
nav: true
nav_order: 3
display_categories: [conferences]
horizontal: false
---

<div class="projects">
  <div class="row row-cols-1 row-cols-md-3">
    {% assign conference_items = site.projects | where: "category", "conferences" | sort: "importance" %}
    {% for project in conference_items %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
