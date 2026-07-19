---
layout: default
title: Music
permalink: /music/
---

# Music

Music I have made and contributed to.

{% assign pieces = site.music | sort: "date" | reverse %}
{% for piece in pieces %}{% include work.html item=piece %}{% endfor %}
