---
id: 45
title: Making android studio faster
date: 2014-06-13T09:32:37+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=45
permalink: /2014/06/making-android-studio-faster/
geo_public:
  - 0
categories:
  - android
tags:
  - android
  - android studio
---
Android Studio looks nice but it&#8217;s slow. So looking for ways to improve its performance I found one tip which saves me 10 secs everytime:

> Just create gradle.properties in:
> 
>        /home/<username>/.gradle/ (Linux)
>     
> 
> Add this to the file:

       org.gradle.daemon=true
    I'll add to this post if I find out more.