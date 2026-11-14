---
layout: default
title: Research
permalink: /research
---

# Research

I'm a researcher in sound and AI and co-founder and technical lead at
[Studio Cucurbits.](https://www.studiocucurbits.com/) My work centres on
controllable and interpretable generative models for voice, music and sound,
and on turning these ideas into audio tools and interactive artistic systems.

From August 2024 to August 2026, I was a Research Scientist at
[Supertone](https://supertone.ai), developing voice representations,
text-to-speech models and voice-editing tools. Before that, I worked at
[IRCAM](https://ircam.fr) and completed my PhD at Sorbonne Université on neural
voice transformation.

## Research interests

- Controllable and interpretable generative models
- Self-supervised representation learning
- Neural audio/speech codecs
- Music applications: MIR, singing voice synthesis, music generation models
- Speech applications: TTS, VC, ASR

## Recent publications and demonstrations

- **[RobustSpeechFlow: Learning Robust Text-to-Speech Trajectories via Augmentation-based Contrastive Flow Matching](https://arxiv.org/abs/2605.22083)** — Jinhyeok Yang, Hyeongju Kim, Yechan Yu, Joon Byun, Frederik Bous and Juheon Lee. Interspeech 2026.
- **[A neural voice editing tool for transforming pitch, subharmonics, and structural noise](https://ismir2025program.ismir.net/lbd_439.html)** — Frederik Bous, Jacob Morton, Joon Byun, Yechan Yu, Jinhyeok Yang, Hyeongju Kim and Juheon Lee. ISMIR 2025, late-breaking demo.
- **[SupertonicTTS: Towards Highly Efficient and Streamlined Text-to-Speech System](https://arxiv.org/abs/2503.23108)** — Hyeongju Kim, Jinhyeok Yang, Yechan Yu, Seunghun Ji, Jacob Morton, Frederik Bous, Joon Byun and Juheon Lee. arXiv preprint, 2025.

## Research projects

<div class="media-list">
{% assign topics = site.research | sort: "order" %}
{% for topic in topics %}
  <div class="media-item">
    {% if topic.image %}{% if topic.link %}<a class="media-thumb" href="{{ topic.link }}"><img src="{{ topic.image }}" alt="{{ topic.name }}"></a>{% else %}<div class="media-thumb"><img src="{{ topic.image }}" alt="{{ topic.name }}"></div>{% endif %}{% endif %}
    <div class="media-body">
      <h3>{% if topic.link %}<a href="{{ topic.link }}">{{ topic.name }}</a>{% else %}{{ topic.name }}{% endif %}</h3>
      {{ topic.short | markdownify }}
      {{ topic.content | markdownify }}
    </div>
  </div>
{% endfor %}
</div>

## Full publication list

- [ORCID](https://orcid.org/0000-0002-7477-7600)
- [Google Scholar](https://scholar.google.de/citations?user=Isec9tEAAAAJ&hl=en)
