---
layout: element
name: Voice editing software
type: Neural voice tools
order: 0
link: https://forum.ircam.fr/projects/detail/circe/
image: /assets/cauldron.png
short: >
  Software for editing and transforming the voice: the neural tools I develop at
  Supertone and IRCAM.
---

## Supertone's pitch drawing tool

At [Supertone](https://supertone.ai) I build neural voice-editing tools on top
of our NANSY voice backbone. Presented at
[ISMIR 2025](https://ismir2025program.ismir.net/lbd_439.html), the latest tool
edits pitch, subharmonics and structural noise (jitter and shimmer): it
decomposes a voice into pitch, linguistic and speaker representations, and you
reshape it by redrawing the control-parameter curves in a web UI, on a computer
or tablet.

The pitch drawing tool is available for business customers at Supertone
and is used by audio engineers and movie directors.

<iframe class="work-trailer" src="https://drive.google.com/file/d/1NSiNdg2WGWrEliYMVqV5-eXYh0lBIpyR/preview" title="ISMIR 2025 demo — neural voice editing tool" allow="autoplay" allowfullscreen></iframe>

## IRCAM's CIRCE {#circe}

![CIRCE screenshot](/assets/circe.png)

CIRCE — the **IRC**am neural auto-en**C**oder for voi**CE** — transforms the
pitch and intensity of a voice using the neural auto-encoder developed in my
thesis. Originally built to realise the voice transformations for the
[artistic residency of Judith Deschamps](/projects/deschamps), I've refined the design in collaborations with composers such as [Omer Barash](/music/#gnz),
[Sachie Kobayashi](/music/#day0) and [Aïda Shirazi](/music/#neentrecorps).

The original app was a GTK standalone. With the help of our software engineer 
Pierre Guillot, we've ported the model into a VST plugin. The voice transformation runs in real time on modern computer hardware.

![The Circe live VST plugin](/assets/circe-live.png)

CIRCE is available on the [IRCAM forum](https://forum.ircam.fr/projects/detail/circe/)
to any registered user (registration is free). The research and software were
developed as part of the ANR project
[*ARS* (ANR-19-CE38-0001-03)](http://ars.ircam.fr/).
