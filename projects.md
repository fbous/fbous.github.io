---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Longer creative-technology works where I built the technology behind the piece.
See also the [Music](/music/) pieces made with my voice-transformation tools and
the [Films](/films/) I contributed to.

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
