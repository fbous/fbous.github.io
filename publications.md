---
layout: page
title: "publications"
permalink: /publications
---

{% for pub in site.publications %}
  ## {{ pub.title }}

  {{ pub.content }}

  pub.link
{% endfor %}
