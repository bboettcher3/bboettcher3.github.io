---
layout: post
author: Brady Boettcher
title: Mouse Modulator
---
<img
  align="right"
  height="350"
  padding="50px"
  src="/images/mouse-modulator.gif" />

Mouse Modulator is a standalone program that exposes mouse and trackpad signals on the distributed *libmapper* signal mapping network, providing new opportunities for interaction between hardware devices and synthesizers/audio effects. One of the major difficulties in using *libmapper* as a new user is access to libmapper-comatible input devices. Mouse Modulator provides a number of gestural signals to the user related to mouse/trackpad direction, speed, clicks, scrolls and more. One common use case is to pair this program with [Mapper4Live](/mapper4live) to modulate Ableton Live parameters in real time.

As the program is built with Unity3D, the mouse is locked in place (similar to a game) while interacting to avoid collisions with other programs on the screen. (just press ESC to unlock). 


You can find the code repository [here](https://github.com/bboettcher3/MouseModulator).