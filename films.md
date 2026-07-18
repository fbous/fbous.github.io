---
layout: default
title: Films
permalink: /films/
---

# Films

Films I contributed to, newest first. These are generally not available to
watch online.

{% assign films = site.films | sort: "date" | reverse %}
{% for film in films %}
<div class="media-item" id="{{ film.slug }}">
  {% if film.poster %}<a class="media-thumb media-thumb--film" href="{{ film.url }}"><img src="{{ film.poster }}" alt="{{ film.title }}"></a>{% endif %}
  <div class="media-body">
    <h2><a href="{{ film.url }}">{{ film.title }}</a> <span class="post-year">({{ film.year }})</span></h2>
    <p class="post-meta"><em>{{ film.type }}</em>{% if film.director %} &middot; {{ film.director }}{% endif %}{% if film.venue %} &middot; {{ film.venue }}{% endif %}</p>
    {{ film.description | markdownify }}
  </div>
</div>
{% endfor %}
