---
layout: post
title:  "Getting into a different house, and making it smart"
date:   2017-03-31 15:06:42 -0400
categories: hass synology
---
After 18 years living in a turn of the (last) century farmhouse, we've moved closer to town and into a more modern house (built 1968). There are many amenities here that are new to us, like a dishwasher, central air and heating, and grounded outlets where grounded outlets should be.

One of the things I'd like to do with this house, given its more modernness, is to start to play around with smart home things, commonly referred to as the Internet of Things (IoT). This traditionally consists of putting devices on your home WiFi network that wouldn't ordinarily be on WiFi, like appliances, light bulbs, and power switches and outlets.

We're an Apple family, and exist in the Apple ecosystem almost exclusively. That makes HomeKit an obvious choice as a home automation system. However, HomeKit doesn't have the breadth of support on devices that the other competeting systems do, and there's the Apple Tax that must be paid. So, for this preliminary round, anyway, I'm looking at other choices. Amazon and Google, though, are not options for me, for mostly philisophical reasons and security-related concerns. Which leaves my old pal Open Source.

Doing a little digging in the OSS home automation landscape has lead me to [Home Assistant](https://home-assistant.io), known as HASS. HASS is a suite of software culminating in a web-based interface for doing home automation. HASS has lots and lots of integrations, as hackers beat on protocols and decode them and write little drivers to support them within HASS.

HASS, being Linux based, is also a great candidate for running in Docker on my Synology NAS. It was simple to get it up and running in a container on the Synology and start playing around with the kinds of integrations you can do with HASS without actually owning any IoT equipment. By default, it exposes its webUI running on port 8123.It can grab weather conditions and forecasts, 

With HASS up and running, I can turn my attention to another tantalizing tidbit of this new house. There's an old ADT system here, with a Simon XT keypad controller, and sensors on most of the doors and windows. Hooking these up to HASS will be a very interesting, and, if I can get it working, extremely rewarding tinkering project.
