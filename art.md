---
layout: default
title: Art
permalink: /art
---

# Art

I like working at the intersection of machine learning, signal processing and
art. Below are music pieces made with my voice-transformation tools, longer
creative-technology projects, and films I contributed to.

## Music collaborations

Pieces written at IRCAM using the voice-transformation software
[CIRCE](/projects/circe).

{% assign music = site.collaborations | where: "category", "music" | sort: "year" %}
{% for item in music reversed %}
<div class="post" id="{{ item.slug }}">
  <h3>{{ item.name }}{% if item.year %} ({{ item.year }}){% endif %}</h3>
  <p class="post-meta"><em>{{ item.type }}</em>{% if item.artist %} &middot; {{ item.artist }}{% endif %}{% if item.location %} &middot; {{ item.location }}{% endif %}</p>
  {{ item.short | markdownify }}
  {{ item.content | markdownify }}
</div>
{% endfor %}

## Creative technology

Longer projects where I built the technology behind the work. Each has its own
page.

<div class="media-list">
{% assign projects = site.projects | where: "category", "creative-tech" %}
{% for p in projects %}
  <div class="media-item">
    {% if p.image %}<a class="media-thumb" href="{{ p.url }}"><img src="{{ p.image }}" alt="{{ p.name }}"></a>{% endif %}
    <div class="media-body">
      <h3><a href="{{ p.url }}">{{ p.name }}</a></h3>
      {% if p.type %}<p class="post-meta"><em>{{ p.type }}</em></p>{% endif %}
      {{ p.short | markdownify }}
    </div>
  </div>
{% endfor %}
  <div class="media-item">
    <div class="media-body">
      <h3><a href="https://www.studiocucurbits.com/">Studio Cucurbits &#8599;</a></h3>
      <p class="post-meta"><em>Creative-technology studio</em></p>
      <p>Ongoing collaboration with the composer Sachie Kobayashi, designing
      sonic structures and AI audio for multi-disciplinary projects.</p>
    </div>
  </div>
</div>

## Film

Films I contributed to. These are generally not available to watch online.

<div class="media-list" id="film">
{% assign films = site.collaborations | where: "category", "film" | sort: "year" %}
{% for item in films reversed %}
  <div class="media-item" id="{{ item.slug }}">
    {% if item.image %}<a class="media-thumb" href="{{ item.link }}"><img src="{{ item.image }}" alt="{{ item.name }}"></a>{% endif %}
    <div class="media-body">
      <h3>{% if item.link %}<a href="{{ item.link }}">{{ item.name }}</a>{% else %}{{ item.name }}{% endif %}{% if item.year %} ({{ item.year }}){% endif %}</h3>
      <p class="post-meta"><em>{{ item.type }}</em>{% if item.artist %} &middot; {{ item.artist }}{% endif %}</p>
      {{ item.short | markdownify }}
    </div>
  </div>
{% endfor %}
</div>
