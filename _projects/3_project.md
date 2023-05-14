---
layout: page
title: Black hole ray marcher
description: A ray marcher that renders a black hole written in Rust.
img: assets/img/blackhole_background.jpg
importance: 4
category: work
---

This was my first project I made when I started learning Rust. It is a ray marcher that renders a black hole.
The rays are propagated from the camera in fixed distance steps and at each step, the ray's direction is corrected by the gravitational field of the black hole.
All the calculations are done on the CPU. This project features my first attempt at parallelism in Rust, which with today's knowledge I would do differently.

The following image shows the final render of the black hole:

<div class="row">
    <div class="col-sm mt-12 mt-md-0">
        {% include figure.html path="assets/img/blackhole.jpg" title="rendered blackhole" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Final render of the black hole ray marcher.
</div>

You can check my code in the repository below. The code does not include the used textures.

<div class="repo p-2 text-center">
  <a href="https://github.com/XelfXendr/black_hole">
    <img class="repo-img-light w-100" alt="XelfXendr/black_hole" src="https://github-readme-stats.vercel.app/api/pin/?username=XelfXendr&repo=black_hole&theme={{ site.repo_theme_light }}&show_owner=true">
    <img class="repo-img-dark w-100" alt="XelfXendr/black_hole" src="https://github-readme-stats.vercel.app/api/pin/?username=XelfXendr&repo=black_hole&theme={{ site.repo_theme_dark }}&show_owner=true">
  </a>
</div>

