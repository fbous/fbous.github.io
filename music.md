---
layout: default
title: Music
permalink: /music/
---

# Music

Pieces written using my voice-transformation software
[CIRCE](/projects/circe), newest first.

{% assign pieces = site.music | sort: "date" | reverse %}
{% for piece in pieces %}{% include work.html item=piece %}{% endfor %}
