---
title: "CompostBuddy"
description: "ESP32 IoT device"
date: 2023-03-13T10:20:19-05:00
draft: false
---

![CompostBuddy IoT Device](/CompostBuddy.jpg)

This is a WiFi connected IoT project that monitors a home compost tumbler. The system monitors compost temperature and tumbling frequency. I built this primarily out of parts I bought at Adafruit, and I put the entire bill of materials in GitHub.

I wrote the code on the ESP32 in CircuitPython. CircuitPython is Adafruit's port of MicroPython, which is a lean implementation of Python 3. Data from the device is pushed to an API I wrote in Express. The data is saved to a Time Series Collection in MongoDB that I have running in Docker. To view the data, I wrote a small UI with Vue.js 3.

You can view the code at [github.com/srenner/compostbuddy](https://github.com/srenner/compostbuddy)