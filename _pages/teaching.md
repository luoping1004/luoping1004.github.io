---
layout: page
title: teaching
permalink: /teaching/
description: 
nav: true
nav_order: 4
display_categories: [computer science, bioinformatics]
horizontal: false
---

- COSC1046 - Introduction to Computer Science
- COSC2006 - Data Structure I
- COSC3306 - Introduction to Computer Graphics
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Algoma_1046W.jpg" title="COSC1046W24W" class="img-fluid rounded z-depth-1" %}
        {% include figure.html path="assets/img/OUF.jpg" title="COSC1046W24W" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- Guest Lecturer at Thomson River University

- Teaching Assistant at University of Saskatchewan

<!-- pages/teaching.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>