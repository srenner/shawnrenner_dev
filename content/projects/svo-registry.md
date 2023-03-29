---
title: "SVO Registry"
description: "Python web app being re-written with .NET Blazor"
date: 2023-01-16T21:07:59-06:00
draft: false
thumbnail: "/svo-stock-photo.jpg"
---

![Mustang SVO](/svo-stock-photo.jpg)

I created the original SVO Registry several years ago. I was new to ASP.NET MVC, but at the time, the server-side frameworks I was more curious about were Ruby on Rails and Django. I settled on using Django, because I had been looking for a good reason to take a deeper dive into Python programming. Other tools in use are PostgreSQL, Bootstrap, a few jQuery plugins, and the Whoosh search engine. The site can be viewed at [svoregistry.com](http://svoregistry.com) and the code is on [GitHub](https://github.com/srenner/svoregistry-v2).

The basic premise of the site is to build a vehicle registry based on VIN that lets owners, prospective owners, and fans of the car to view history and information about each car. The SVO community was mired in controversy at the time, and a different registry went behind a members-only paywall. This prompted me to build the only publicly available registry for the Mustang SVO, which is a collector car I have personally owned since 2003.

I am currently re-writing the site as a .NET Blazor Wasm project called **CollectorRegistry**, and I'm making it multi-tenant so that other types of vehicles or collector items can be hosted as their own registry.

The code is on [GitHub](https://github.com/srenner/CollectorRegistry).