---
layout: default
title: Projects
permalink: /projects/
---

# Projects

Longer creative-technology works where I built the technology behind the piece.
See also the [Music](/music/) pieces I was involved in and
the [Films](/films/) I contributed to.

<div class="media-list">
  <div class="media-item">
    <a class="media-thumb" href="https://www.studiocucurbits.com/"><img src="/assets/studio-cucurbits-thumb.png" alt="Studio Cucurbits"></a>
    <div class="media-body">
      <h3><a href="https://www.studiocucurbits.com/">Studio Cucurbits &#8599;</a></h3>
      <p class="post-meta"><em>Creative-technology studio</em></p>
      <p>Ongoing collaboration with the composer <a href="https://www.sachiekobayashi.com/">Sachie Kobayashi</a>, designing
      sonic structures and AI audio for multi-disciplinary projects.</p>
    </div>
  </div>
{% assign projects = site.projects | sort: "order" %}
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
</div>
