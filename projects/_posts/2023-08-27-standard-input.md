---
layout: post
author: Brady Boettcher
title: Standard Input M4L Device
---
<img src="/images/stdinput.png" />

Standard Input (a.k.a std::input) is a free and open source Max for Live device that exposes mouse and trackpad signals as mappable modulators in Ableton Live. Mouse position, speed, and clicking status are included in this basic version, with more complex signals coming soon. I've been using this as a quick realtime modulator in my own projects, and it works great to inject some expression without needing external hardware (just use the standard inputs!).

It uses the same conventional mapping style from the LFO device, supporting custom destination ranges and range inversion. This project is related to my previous work on [Mouse Modulator]({% post_url 2022-07-05-mouse-modulator %}), which is a standalone equivalent of this built in Unity.


You can find the code repository and releases [here](https://github.com/StrangeLoopsAudio/StandardInput_M4L/releases/latest).