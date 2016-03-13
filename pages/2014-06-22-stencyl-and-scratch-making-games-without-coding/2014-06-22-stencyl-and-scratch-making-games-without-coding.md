---
id: 64
title: 'Stencyl and Scratch: Making games without coding'
date: 2014-06-22T10:05:59+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=64
permalink: /2014/06/stencyl-and-scratch-making-games-without-coding/
geo_public:
  - 0
categories:
  - Game development
tags:
  - Stencyl
  - ubuntu
---
I started playing around with <a href="http://www.stencyl.com" target="_blank">Stencyl</a> today. First of all I had a hard time making it run on Ubuntu, hopefully this post helped me to get it running:

> You don&#8217;t need to install the ia32-libs, you only need to edit a bash file changing the route of java binaries like in this example.
  
> Original:
  
> #!/bin/bash
> 
> ./runtimes/jre-linux/bin/java -Xms64m -Xmx1024m -Djava.library.path=./lib -jar ./sw.jar
> 
> Change:
  
> #!/bin/bash
> 
> java -Xms64m -Xmx1024m -Djava.library.path=./lib -jar ./sw.jar
> 
> In this case, Stencyl use the local java installed in the OS.

I&#8217;ll write more about it later on, if I do something intresting with it.

I also tried <a href="http://scratch.mit.edu" target="_blank">Scratch</a>, the MIT project. It was funny.