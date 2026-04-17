---
layout: post
---

## Background

A [strain gage](https://en.wikipedia.org/wiki/Strain_gauge) is a device that measures the strain experienced by a part. Assuming a constant cross section, and a known Young's modulus, one can experiementally determine the stress a part experiences during testing. 

Purdue Baja Racing was hoping to find the torsional stress experienced by our axles (especially the front axles) during various situations. Knowing the actual maximum torque that the drivetrain would experience would allow us to size components accurately, likely saving weight in the process.

However, being on an axle, a wired strain gage would have been... difficult. And given the size of the axles, very few solutions within our size and budget range were available.

So we decided to build our own.

## System Overview

There are many parts of this system, including:

* The gage itself, attached to the axle
* The electronics, including a Wheatstone bridge, ADC, microcontroller, and battery
* The software for said microcontroller
* A compact waterproof enclosure for both the gage and electronics
* External communication to the electronics (the "wireless" part of the strain gage)
* Processing collected data

## The Strain Gages

<figure style="float:right; margin: 0 0 1em 1em; max-width: 50%; text-align: center;">
  <img src="/assets/img/wsg3_cropped.jpg"
       alt="Strain gage attached to axle"
       style="max-width: 100%; height: auto;">
  <figcaption>
    My first practice strain gage attachment took all day. Hopefully it doesn't take nearly as long next time…
  </figcaption>
</figure>

We used Vishay Torsional Strain Gages <!--TODO: Find the part number--> for the actual measurement itself.

For training ourselves to attach strain gages, we used a lot of low-cost strain gages for practice. 

To protect the strain gages, we placed a layer of RTV 3140 on it, something carried over from previous years' strain gages. 

For wiring to the strain gage, we recently got some bonded 26 AWG silicone-insulation wire, which should be able to resist the vibrations and shocks of being on the vehicle, plus keep the wiring clean. 

<div style="clear: both;"></div>

## Electronics

