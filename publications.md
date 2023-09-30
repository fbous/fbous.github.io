---
layout: page
title: "publications"
permalink: /publications
---

{% for pub in site.publications %}
  <h2>
    <a href="{{ pub.link }}">
      {{ pub.title }}
    </a>
  </h2>

  <p>{{ pub.content | markdownify }}</p>
{% endfor %}
