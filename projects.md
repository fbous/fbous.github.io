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
      <p class="post-meta"><em>Co-founder, Technical Lead · September 2026 - present</em></p>
      <p>With composer <a href="https://www.sachiekobayashi.com/">Sachie Kobayashi</a>, I develop audio instruments and creative technology for music and interdisciplinary projects.</p>
      <p>Our first commercial audio effect, <strong>Suspended 1.0</strong>, was released for Linux and macOS in October 2026. My work covers the engineering around it: QA for our AI-based development pipeline, the release pipeline, licensing and cloud infrastructure.</p>
      <p>I also developed a <strong>four-language phonetic relay prototype</strong> for an interactive installation, connecting speech recognition, language-model interpretation and speech synthesis with OSC control.</p>
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
