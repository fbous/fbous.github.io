---
layout: default
title: CV
permalink: /cv
---

# Curriculum Vitae

**[📄 One-page résumé as PDF](/assets/cv.pdf)**

I'm looking for exciting new challenges at the intersection between machine learning, voice technology and art, between scientific theory and applications in creative domains.

---

## Research Interests

AI for voice, music, and sound: 
- Controllable and interpretable generative models
- Self-supervised representation learning
- Neural audio/speech codecs
- Music applications: MIR, singing voice synthesis, music generation models
- Speech applications: TTS, VC, ASR

Open to new challenges related to artistic media.


---

## Experience

{% for job in site.data.cv.experience %}
{% include cv_entry.html title=job.title organization=job.organization location=job.location date=job.date content=job.description %}
{% endfor %}

---

## Education

{% for degree in site.data.cv.education %}
{% include cv_entry.html title=degree.title organization=degree.organization location=degree.location date=degree.date %}
{% endfor %}

---

## Additional Education

{% for item in site.data.cv.education_extra %}
{% include cv_entry.html title=item.title organization=item.organization location=item.location date=item.date %}
{% endfor %}

---

## Skills

{% for skill in site.data.cv.skills %}
**{{ skill.category }}:** {{ skill.items }}
{% endfor %}

---

## Scholarships

{% for scholarship in site.data.cv.scholarships %}
{% include cv_compact_entry.html title=scholarship.name subtitle=scholarship.organization date=scholarship.date %}
{% endfor %}

---

## Activities

{% for activity in site.data.cv.activities %}
{% include cv_compact_entry.html details=activity.name date=activity.date %}
{% endfor %}

---

## Talks

{% for talk in site.data.cv.talks %}
{% include cv_compact_entry.html title=talk.title subtitle=talk.location date=talk.date %}
{% endfor %}

---

## Code

Checkout my [github page](https://github.com/fbous) for code examples, though, unfortunately, most of my actual code cannot be made available.

