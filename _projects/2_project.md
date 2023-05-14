---
layout: page
title: Train screen-saver
description: A Windows screen-saver with a train travelling between the screens of multiple computers.
img: assets/img/balazs-busznyak-El5zuQAtfeo-unsplash.jpg
importance: 3
category: work
---

I made this screen-saver for a school project.
On a single computer, it is a simple screen-saver that displays a train travelling between the screens.
The magic happens when you run the screen-saver on multiple computers on the same network, as the train will travel between the screens of all the computers.

The screen-saver is written in C# using WPF and .NET Core 3.1.
The communication between the computers is done in a client-server fashion.
The server is a simple console application written in Rust that listens for TCP connections on a specified port. It controls on which computer the train is currently located and keeps track of what part of the screen the train left from and where it should enter the next screen.

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        <video controls class="img-fluid rounded z-depth-1">
            <source src="{{ site.baseurl }}/assets/vids/VID_20201211_001113.webm" type="video/webm">
            Your browser does not support the video tag.
        </video>
    </div>
</div>
<div class="caption">
    The screen saver in action on two computers.
</div>

The code for this project is available in the repository below.

<div class="repo p-2 text-center">
  <a href="https://github.com/XelfXendr/Train-Screensaver">
    <img class="repo-img-light w-100" alt="XelfXendr/Train-Screensaver" src="https://github-readme-stats.vercel.app/api/pin/?username=XelfXendr&repo=Train-Screensaver&theme={{ site.repo_theme_light }}&show_owner=true">
    <img class="repo-img-dark w-100" alt="XelfXendr/Train-Screensaver" src="https://github-readme-stats.vercel.app/api/pin/?username=XelfXendr&repo=Train-Screensaver&theme={{ site.repo_theme_dark }}&show_owner=true">
  </a>
</div>