---
title: "CompostBuddy"
description: "ESP32 IoT device using CircuitPython"
date: 2023-03-13T10:20:19-05:00
draft: false
thumbnail: "/CompostBuddy.jpg"
---

![CompostBuddy IoT Device](/CompostBuddy.jpg)

With home composting, you want your material to break down in a thermophilic temperature range between about 135°F and 160°F. This is warm enough to kill pathogenic organisms and weed seeds, and ensures an efficient breakdown of organic material. The compost must be occasionally "turned" or tumbled to properly aerate the pile and ensure all the material is subjected to the heat.

To help keep track of my compost temperature and aeration, I built this WiFi connected IoT project. I wrote the code on the ESP32 microcontroller in CircuitPython, which is a lean implementation of Python 3 for embedded projects. Data from the device is pushed to an API I wrote in Express. The data is saved to a Time Series Collection in MongoDB that I have running in Docker. To view the data, I wrote a web UI with Vue.js 3.

I built this primarily out of parts I bought at Adafruit, and I put the [bill of materials](https://github.com/srenner/CompostBuddy/blob/master/iot/README.md) in GitHub.

You can view the code at [github.com/srenner/compostbuddy](https://github.com/srenner/compostbuddy)