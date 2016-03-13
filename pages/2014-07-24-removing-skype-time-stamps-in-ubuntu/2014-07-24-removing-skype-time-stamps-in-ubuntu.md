---
id: 123
title: Removing skype time stamps in Ubuntu
date: 2014-07-24T19:50:03+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=123
permalink: /2014/07/removing-skype-time-stamps-in-ubuntu/
geo_public:
  - 0
categories:
  - Tips and tricks
tags:
  - libreoffice
  - linux
---
So when I copied and pasted my messages from Skype into Libre office, it brought also the annoying time stamps

For example:

**[14.56.53]** ZangeFarsi.Com: ylensaa ne kulkee aikataulon mukaan
  
**[14.57.19]** ZangeFarsi.Com: ne ei ole myöhässä

I googled around and around, with no results. Finally I decided to make a regular expression and using the Find and Replace feature in my word processor (Libre office) replace the time stamps with a space character.

Here&#8217;s the expression I made up reading the guide <a href="https://help.libreoffice.org/Common/List_of_Regular_Expressions" target="_blank">in here. </a>

\[[:digit:\]\[:digit:\].\[:digit:\]\[:digit:\].\[:digit:\]\[:digit:\]]

It works like a charm <img src="http://modestdeveloper.com/wp-includes/images/smilies/simple-smile.png" alt=":)" class="wp-smiley" style="height: 1em; max-height: 1em;" />