---
layout: about
title: about
permalink: /
subtitle: Computer Science student at <a href='https://www.mff.cuni.cz/en'>Faculty of Mathematics and Physics, Charles University</a>

profile:
  align: right
  image: prof_transp.png
  image_circular: true # crops the image to make it circular

news: false  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

Hi, my name is Jan Bronec. I am a 3rd year Bachelor's degree student at [Faculty of Mathematics and Physics, Charles University](https://www.mff.cuni.cz/en).
My major is Computer Science but part of my studies is also focused on Artificial Intelligence and Machine Learning.

Besides AI and ML, my interests include computer vision, functional programming, parallel and distributed computing, and software engineering.
I am a fan of the Rust programming language and I'm a sucker for discrete maths.


You can read through my [CV]({{ site.baseurl }}{% link _pages/cv.md %}) or check out some of my projects:

<!-- pages/projects.md -->
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
