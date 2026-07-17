---
layout: default
title: Art
permalink: /art
---

# Collaborations with artists

<div class="media-list">
  {% assign sorted = site.collaborations | sort: "year" %}
  {% for collaboration in sorted reversed %}
    <div class="media-item">
      <a class="media-thumb" href="{{ collaboration.url }}">
        <img src="{{ collaboration.image }}" alt="{{ collaboration.name }}">
      </a>
      <div class="media-body">
        <h2><a href="{{ collaboration.url }}">{{ collaboration.name }}{% if collaboration.year %} ({{ collaboration.year }}){% endif %}</a></h2>
        <i>{{ collaboration.type }}</i>
        {{ collaboration.short | markdownify }}
      </div>
    </div>
  {% endfor %}
</div>
