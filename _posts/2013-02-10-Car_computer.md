---
layout: default
title: Car computer
category: carduino
---
# {{page.title}}
Me and my girlfriend recently purchased a car, a [2010 VW Polo](http://en.wikipedia.org/wiki/Vw_polo#Polo_Mark_V_.28Typ_6R.2C_2009.E2.80.93present.29), and as a engineer I have of course thought of things that is missing from the car, that I can add myself.

The first thing I would like to add to the car is some system that recognizes me or my girlfriend as we approach the car, and unlocks itself. The next step would be for the car to be able to start without the normal turn of the key, but that is a project for later.

After thinking this through I have realized that the most appropriate way probably would be to have a bluetooth-device in the car, and when a connection is detected the device sends a signal over the CAN-bus to unlock the doors. A similar project utilizing the CAN bus can be found here: [secuduino](http://secuduino.blogspot.com/) opening the doors is not performed, but I assume that will only be a slight modification in the command sent.

I was first thinking of using my [Raspberry PI](http://www.raspberrypi.org/) as the main-unit of my device, but soon realized that it consumed way to much power, about 500mA is the numbers I found, so I ordered a arduino instead: [Arduino Nano](http://www.aliexpress.com/item/Nano-V3-0-AVR-ATmega328-P-20AU-Module-Board-USB-Cable-for-Arduino-Blue-Black/728568814.html) and a bluetooth chip: [Arduino Bluetooth Module](http://www.aliexpress.com/item/Bluetooth-pass-through-modules-with-universal-mounting-with-Enable-and-state-output-wireless-serial-from-machine/658943620.html)

With these two I hope to be able to pair my phone and send a command once paired working, then I will have to find a chip for communicating to the CAN-bus, I have ordered [this](http://ww1.microchip.com/downloads/en/devicedoc/21801e.pdf) and will try use it when it arrives.
