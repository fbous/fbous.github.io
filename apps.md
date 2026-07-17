---
layout: default
title: Apps
permalink: /apps
---

# Software

<div class="media-list">
  {% for software in site.software %}
    <div class="media-item">
      <a class="media-thumb media-thumb--lg" href="{{ software.url }}">
        <img src="{{ software.image }}" alt="{{ software.name }}">
      </a>
      <div class="media-body">
        <h2><a href="{{ software.url }}">{{ software.name }}</a></h2>
        {{ software.short | markdownify }}
      </div>
    </div>
  {% endfor %}
</div>

Discover more on my [Gitlab](https://gitlab.com/bous) page.
