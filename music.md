---
layout: default
title: Music
permalink: /music/
---

# Music

Pieces written using my voice-transformation software
[CIRCE](/projects/circe), newest first.

{% assign pieces = site.music | sort: "date" | reverse %}
{% for piece in pieces %}
<div class="post" id="{{ piece.slug }}">
  <h2><a href="{{ piece.url }}">{{ piece.title }}</a> <span class="post-year">({{ piece.year }})</span></h2>
  <p class="post-meta"><em>{{ piece.type }}</em>{% if piece.composer %} &middot; {{ piece.composer }}{% endif %}{% if piece.venue %} &middot; {{ piece.venue }}{% endif %}</p>
  {% if piece.video %}<video class="work-video" src="{{ piece.video }}" controls="controls"></video>{% endif %}
  {{ piece.description | markdownify }}
</div>
{% endfor %}
