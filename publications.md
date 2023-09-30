---
layout: page
title: "second"
permalink: /second
---

{% for pub in site.publications %}
## {{ pub.title }}

{{ pub.content }}
