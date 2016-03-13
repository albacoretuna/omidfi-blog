---
id: 37
title: Using Hardware Device for testing android
date: 2014-06-09T06:58:27+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=37
permalink: /2014/06/using-hardware-device-for-testing-android/
geo_public:
  - 0
categories:
  - android
  - linux
tags:
  - android
  - ubuntu
---
I managed to use my Galaxy Gio for testing purposes with my Ubuntu simply by creating a text file containing:

`SUBSYSTEM=="usb", ATTR{idVendor}=="<code>04e8`", MODE="0666", GROUP="plugdev"</code>

``I managed to use my Galaxy Gio for testing purposes with my Ubuntu simply by creating a text file containing:

`SUBSYSTEM=="usb", ATTR{idVendor}=="<code>04e8`", MODE="0666", GROUP="plugdev"</code>

`` 

`/etc/udev/rules.d/`

And then setting its permissions by:

chmod a+r /etc/udev/rules.d/51-android.rules

Then I can check if it is working by running this:

adb devices

I used [this page](http://developer.android.com/tools/device.html) as my guide.