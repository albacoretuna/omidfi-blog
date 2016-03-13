---
id: 173
title: Using Ubuntu Without Mouse
date: 2014-09-01T03:23:36+00:00
author: Omid Hezaveh
layout: post
guid: http://gik.fi/wp/?p=173
permalink: /2014/09/using-ubuntu-without-mouse/
panels_data:
  - 'a:0:{}'
dsq_thread_id:
  - 3951076998
categories:
  - linux
tags:
  - MyUbuntuCostumizations
---
My current setting doesn&#8217;t allow me to use a mouse with my laptop, the table is too high. So I&#8217;m using a keyboard only. Here&#8217;s a way to use your Ubuntu without a mouse: (Ubuntu 14.04)

Settings > Universal Access > Pointing and Clicking > Mouse Keys

Turn it on. Now you can move your mouse pointer using the numerical pad arrows, instead of your mouse. If the pointer moves slowly, I found <a href="http://ubuntuforums.org/showthread.php?t=1977588" target="_blank">this post</a> to be useful for making it move faster:

> Firstly open a terminal window and type the following to install the xkbset package:
> 
> sudo apt-get install xkbset
> 
> A simple one line command can then be used to configure the acceleration:
> 
> xkbset ma \[delay\] \[interval\] \[time to max\] \[max speed\] [curve]
> 
> For those new to command-line interfaces, the brackets imply that they need to be replaced by a numerical value, tailored to suite a particular use. I have recently used the following for my configuration
> 
> xkbset ma 60 10 10 20 10