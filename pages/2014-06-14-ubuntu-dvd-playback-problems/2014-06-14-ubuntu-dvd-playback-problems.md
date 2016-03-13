---
id: 55
title: Ubuntu dvd playback problems
date: 2014-06-14T23:19:00+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=55
permalink: /2014/06/ubuntu-dvd-playback-problems/
geo_public:
  - 0
categories:
  - linux
tags:
  - ubuntu
---
So I rented some movies on DVD from library but most of them couldn&#8217;t be read on my laptop. It was fine when I had windows 7 on it, so I guessed it must be from Ubuntu. I was right!

Following the instructions on this page, and then installing this package: <span class="comment-copy"><code>ubuntu-restricted-extras, and after that using VLC player</code>  resolved the issue totally. </span>

1. <span id="line-1" class="anchor"></span>sudo apt-get install libdvdread4<span id="line-31" class="anchor"></span>

<p class="line867">
   2. <span id="line-1-1" class="anchor"></span>sudo /usr/share/doc/libdvdread4/install-css.sh
</p>

  * Rebooting may be necessary.

3. sudo apt-get install ubuntu-restricted-extras

4. sudo apt-get install vlc

&nbsp;

&nbsp;