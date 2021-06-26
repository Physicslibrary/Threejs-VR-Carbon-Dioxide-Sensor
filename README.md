# Threejs-VR-Carbon-Dioxide-Sensor (under construction)
A project to explore measurement of carbon dioxide concentration and presenting the numbers in virtual reality.<br>

It is about learning to interface a Sensirion SCD4x carbon dioxide sensor to a Raspberry Pi and an Oculus Quest to 3D map CO2 measurements.<br>

<img src="images/scd41.gif" width="360">

## Threejs-VR-Physics Pages

[https://physicslibrary.github.io/Threejs-VR-Carbon-Dioxide-Sensor/](https://physicslibrary.github.io/Threejs-VR-Carbon-Dioxide-Sensor/)

## System Requirements

Oculus Quest (tested Quest 1, no controllers)<br>

Oculus Browser >15.4 (Quest update 29.0)<br>

Not sure if Oculus Browser needs to be configured for WebXR like in the early days. If the simulation below does not work, type "chrome://flags" in Oculus Browser and search for "webxr". "WebXR experiences with hand and joints tracking" and "WebXR Layers" are enabled.<br>

Important - Javascript codes for this project are dependent on "WebXR Hand Input Module - Level 1", as of today, is an unstable API (https://www.w3.org/TR/webxr-hand-input-1/). Codes may stop working after Oculus Browser or threejs update. Oculus' WebXR hand tracking (released February 2020) and three.js support have been fantastic.<br>

## 1. Simulate measuring CO2 level with Sensirion SCD41<br>

Open Oculus Browser to link ("Enter VR" using hand, no controller):<br>

[https://physicslibrary.github.io/Threejs-VR-Carbon-Dioxide-Sensor/examples/threejs_vr_scd41sim.html](https://physicslibrary.github.io/Threejs-VR-Carbon-Dioxide-Sensor/examples/threejs_vr_scd41sim.html)

Code threejs_vr_scd41sim.html in ./examples simulates CO2 concentration as a function of distance from a point.<br>

With a real SCD41 sensor, one can map CO2 concentration in a room. CO2 in a room are dependent on ventilation, number of persons, time, diffusion, and other factors. Perhaps there will be a passthrough mode in VR in a browser to merge real and virtual views to visualize CO2 3D data. For now, "Passthrough Shortcut" (Guardian setting) by double tapping the headset or "Stationary Boundary: Passthrough" experimental feature. The AR glasses from Oculus would be a great application for this. Hope the AR browser will be just as fantastic as the one on the Quest.<br>

## 2. Interfacing SCD41 to Raspberry Pi

## Hardware

Raspberry Pi with wireless LAN (tested Pi Zero W).

Sensirion SEK-SCD41-Sensor evaluation kit

Oculus Quest (tested Quest One, update 29.0, Oculus browser 15.4)

Raspberry Pi OS Lite (tested May 7, 2021 release)

https://www.raspberrypi.org/software/operating-systems/

## Credits

https://threejs.org/

scd41.glb<br>
photogrammetry created from 18 images using AliceVision Meshroom<br>
(CC BY 4.0)<br>

https://alicevision.org/

## References

https://www.raspberrypi.org/

https://www.sensirion.com/en/environmental-sensors/evaluation-kit-sek-environmental-sensing/evaluation-kit-sek-scd41/

https://github.com/Sensirion/raspberry-pi-i2c-scd4x

https://www.sensirion.com/en/environmental-sensors/indoor-air-quality/correct-ventilation-helps-to-reduce-the-risk-of-virus-transmission/

https://montrealgazette.com/news/quebec/co2

Adafruit Industries' Youtube on SCD4x:<br>

https://www.youtube.com/watch?v=M_tFVNKgX04
