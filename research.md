---
layout: default
title: Research
permalink: /research
---

# Research

I'm a researcher in sound and AI, working on voice technology. I'm currently at
[Supertone](https://supertone.ai), where I maintain and develop our voice
backbone, NANSY, used for text-to-speech and voice conversion. Previously I was
at [IRCAM](https://ircam.fr), where I completed my doctoral thesis on neural
voice transformation. My work centres on controllable and interpretable
generative models for voice, music and sound.

## Research topics

<div class="media-list">
{% assign topics = site.research | sort: "order" %}
{% for topic in topics %}
  <div class="media-item">
    {% if topic.image %}<div class="media-thumb"><img src="{{ topic.image }}" alt="{{ topic.name }}"></div>{% endif %}
    <div class="media-body">
      <h3>{{ topic.name }}</h3>
      {{ topic.short | markdownify }}
      {{ topic.content | markdownify }}
    </div>
  </div>
{% endfor %}
</div>

## Full publication list

- [ORCID](https://orcid.org/0000-0002-7477-7600)
- [Google Scholar](https://scholar.google.de/citations?user=Isec9tEAAAAJ&hl=en)
