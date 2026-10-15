# TriivOS

Triiv: Estonian for drifting off course, which is exactly what the car shouldn’t do unless you ask it to.

pronounced "TREEV-OS".

**Flight-controller firmware, rebuilt for RC cars.**

TriivOS turns a small FPV flight controller into a car controller: a gyro steering assist,
an ESC-style throttle with brake and reverse, traction control and more, all set up from a
web app in your browser. It's based on Betaflight, with the flight code replaced by a car
core.

> **Coming soon.** TriivOS is in private testing on real cars. The repositories will open
> once it's ready for wider use.

## What's coming

**Firmware**
- **Steering assist:** classic gyro stabilisation, yaw-rate control that follows the steering
  angle, and a drift mode with automatic counter-steer
- **Steering auto-tune:** drive straight, flip a switch, and it measures the car and suggests gains
- **Throttle like a real car ESC:** forward, brake and reverse, crawler mode, drag brake, launch
  control, throttle hold
- **Stability control and torque vectoring**, plus traction control and ABS on cars with wheel rpm
- **Three drive profiles** on a switch, a gain knob, a steering trim knob and an arm button
- **Beginner / kid mode:** one switch makes the car slower and gentler
- **LiPo and ESC-temperature protection** that limits throttle instead of cutting it
- **Lights** on a WS2812 strip: headlights, brake lights, indicators, underglow
- **From Betaflight:** OSD with car elements, VTX control, blackbox logging, CRSF telemetry and
  GPS lap timing

**Configurator:** a web app that runs in Chrome or Edge, with nothing to install
- Guided setup wizard, presets for common cars, and a live top-down view of what the car
  is doing
- Connects over USB, Bluetooth or the simulator, or try it with a built-in demo board
- Firmware flashing, blackbox log viewer, lap timer and track map, full-screen dashboard

**Simulator:** car physics that runs against the real firmware, so the assists can be tested
and tuned on a PC before they reach the track.

**EdgeTX Lua script** to switch and tune drive profiles from the radio.

## Hardware

Runs on common STM32F405 and STM32H743 flight controllers. Works with cars that use a steering
servo plus an ESC, dual or four motors, tank / skid steer, or crawlers.

## Credits

TriivOS builds on [Betaflight](https://github.com/betaflight/betaflight), Cleanflight and
Baseflight, and is GPL-3.0 like them. Thanks to everyone who built that foundation.

⭐ **Follow TriivOS** to see when it goes public.
