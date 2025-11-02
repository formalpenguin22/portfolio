---
layout: post
title: Haptic Smart Dial
author: Oliver Hansen
description: I created a haptic smart dial as an embedded systems project.
date: 2025-11-02 12:25 -0800
category: Portfolio
image:
  path: /assets/img/formalpenguini.png
  alt: placeholder image
---

## Project Description

The smart dial is a haptic feedback twisting dial with a screen to connect to a computer system or operate fully standalone. The dial will have wireless and wired capabilities, and power on a lithium battery set into the base. It will be freely spinning on a bearing and also include a vibration motor to provide haptic feedback. The functionality is customizable, but it will include alarm features, computer support for scrolling and browsing documents, and macro functionality to skip songs or adjust volume settings. The embedded system will connect either an ESP32 or Photon 2 micro controller to the power management circuits, motor control modules, screen drivers, and the core functionality of a 14-Bit On-Axis Magnetic Rotary Position Sensor (AS5047P). This IC is going to be a key feature, because it will allow for high resolution tracking of the rotation of the dial. The device is going to be designed to interface like a HID (Human Interface Device) such that a PC will pair via Bluetooth and treat it like a scroll wheel, volume knob, etc depending on the setting. 

The key physical features of this device are the high torque 3-phase motor which provides programmable feedback of the turning motion. An LED ring at the top will provide some visual feedback of where the dial is currently engaged to.

The design is still a work in progress, and some implementation details are still being worked out. A couple buttons might be added into the base to allow for a user to actually control the device without a computer. Another design change would be to configure the dial to be a button itself and allow the user to press the entire dial down to engage a small tactile button.

## Block Diagram

![Desktop View](/assets/img/formalpenguini.png){: width="1216" height="1214" }

## Schematic

{% pdf "/assets/documents/haptic_smart_dial_schematic.pdf" no_link%}
