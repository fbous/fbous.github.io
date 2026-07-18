---
layout: element
name: Voice editing software
type: Neural voice tools
order: 0
link: https://forum.ircam.fr/projects/detail/circe/
image: /assets/cauldron.png
short: >
  Software for editing and transforming the voice — from CIRCE, the neural
  auto-encoder built during my PhD at IRCAM, to the voice-editing tools I now
  develop at Supertone.
---

## CIRCE — IRCAM

![CIRCE screenshot](/assets/circe.png)

CIRCE — the **IRC**am neural auto-en**C**oder for voi**CE** — transforms the
pitch and intensity of a voice using the neural auto-encoder developed in my
thesis. Originally built to realise the voice transformations for the
[artistic residency of Judith Deschamps](/projects/judith), it has since been
used by composers such as [Omer Barash](/music/#gnz),
[Sachie Kobayashi](/music/#day0) and [Aïda Shirazi](/music/#neentrecorps).

CIRCE is available on the [IRCAM forum](https://forum.ircam.fr/projects/detail/circe/)
to any registered user (registration is free). The research and software were
developed as part of the ANR project
[*ARS* (ANR-19-CE38-0001-03)](http://ars.ircam.fr/).

## At Supertone

At [Supertone](https://supertone.ai) I build neural voice-editing tools on top
of our NANSY voice backbone. Presented at
[ISMIR 2025](https://ismir2025program.ismir.net/lbd_439.html), the latest tool
edits pitch, subharmonics and structural noise (jitter and shimmer): it
decomposes a voice into pitch, linguistic and speaker representations, and you
reshape it by redrawing the control-parameter curves in a web UI, on a computer
or tablet.

The same editing also ships as a VST plugin, bringing it directly into a DAW.
