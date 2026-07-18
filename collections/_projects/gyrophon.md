---
layout: element
name: Gyrophon
subtitle: "DIY electronic instrument"
type: Electronic instrument
category: creative-tech
image: /assets/smartphone.png
short: >
  Electronic instrument which uses the smartphone's
  acceleration sensor and touch screen
  to control pitch and intensity.
link: https://github.com/fbous/gyrophon-desktop
---

The Gyrophon is an electronic instrument I invented during my time in college. The idea came out of my internship at Siemens where we used the sensor data from android phones. Then I had the idea to use this sensor data to control synthesizers.

I built the first prototype in pure python and the data was sent via bluetooth. In 2020 I rewrote the Gyrophon to use OSC over Wi-Fi and used a csound-expression backend.

<figure class="gyro-photo">
  <img src="/assets/gyrophon.jpeg" alt="The Gyrophon app running on a Samsung phone, showing the touch grid">
  <figcaption>The phone is the playing surface: a grid you slide across, tilting to change pitch.</figcaption>
</figure>

I've experimented a lot with it during my improvisation classes at Akademie für Tonkunst Darmstadt. The main idea is to use touch x-y positions for velocity and timbre and use the accelerometer data for pitch. Thus you can play melodies by tilting the phone.

<figure class="gyro-mixer">
  <img src="/assets/gyrophon-mixer.png" alt="The Gyrophon desktop mixer with three voices and an effects rack">
  <figcaption>The desktop synthesiser — three voices (cygnius, aquila, lyra) and a shared effects rack.</figcaption>
</figure>

Listen to an excerpt from my gyrophon sonata.

<iframe class="work-trailer" src="https://www.youtube-nocookie.com/embed/aucf0iRILBs" title="Gyrophon — playing demo" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The code is available on github. You need to install the gyrophon app and run the server on your desktop.

- App: [https://github.com/fbous/gyrophon-android](https://github.com/fbous/gyrophon-android)
- Server: [https://github.com/fbous/gyrophon-desktop](https://github.com/fbous/gyrophon-desktop)
