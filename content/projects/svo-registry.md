---
title: "SVO Registry"
description: "Python web app being re-written with .NET Blazor"
date: 2023-01-16T21:07:59-06:00
draft: false
thumbnail: "/svo-stock-photo.jpg"
---

![Mustang SVO](/svo-stock-photo.jpg)

The SVO Registry was written in Python, using the Django framework, and using PostgreSQL as the data store. On the front end it has Bootstrap and a few jQuery plugins. It can be found at [svoregistry.com](http://svoregistry.com).

I am currently re-writing the site as a .NET Blazor Wasm project called **CollectorRegistry**, and I'm making it multi-tenant so that other types of vehicles or collector items can be hosted as their own registry. The GitHub repo is [here](https://github.com/srenner/CollectorRegistry).