---
title: "MegaSquirt"
description: "DIY EFI and Arduino CAN bus development"
date: 2023-01-16T16:47:58-06:00
draft: false
thumbnail: "/SVO_engine.jpg"
---

![Engine Bay](/SVO_engine.jpg)

[MegaSquirt](https://megasquirt.info/) is an aftermarket automotive ECU that controls a car's fuel injection and ignition system. I got started with it in 2009, and it's what initially got me interested in embedded programming and hobby electronics. Spiritually, MegaSquirt is to car ECUs what the Raspberry Pi is for computers. It's affordable, educational, and DIY friendly.

I am currently using a self-built MegaSquirt II to power my 1986 Mustang SVO. MegaSquirt is ideal for early fuel injection cars of the 1980s and 1990s. With a few modifications, I was able to make MegaSquirt work with the rest of the car's fuel system and also take control of the Ford TFI ignition system. I no longer have to rely on Ford's restrictive air metering device, as MegaSquirt defaults to using a speed density calculation to deliver the correct amount of fuel. This level of control can help someone tune their car to run better than it did when it was new.

I have a MegaSquirt III on my workbench that is almost ready to go in the car. For the new upgrade, I am utilizing the CAN bus capability of the ECU to integrate with my own Arduino projects. I have a series of projects I call AutoCAN that I'm excited to share.

* [AutoCAN_Meguinauge](https://github.com/srenner/AutoCAN_Meguinauge) - This project polls MegaSquirt to display useful gauges on a character display. I intentionally used older display tech to make it look more at home in the car.

* [AutoCAN_Epasuino](https://github.com/srenner/AutoCAN_Epasuino) - This project is a piggyback module for my car's aftermarket electric power assist steering (EPAS). It takes speed sensor data from the car to reduce steering assist at high speed, and has six user-selectable modes.

* [AutoCAN_SensorHub](https://github.com/srenner/AutoCAN_SensorHub) - This project allows me to add all manner of sensor inputs to the main ECU without modifying the car's main wiring harness. I have the following sensor inputs in mind for my car:
  * Fuel pressure sensor
  * Speed sensor from the car's transmission
  * 3-axis accelerometer
  * GPS
  * Compass heading
  * Reverse trigger wire from the car's transmission
  * Ambient temperature

