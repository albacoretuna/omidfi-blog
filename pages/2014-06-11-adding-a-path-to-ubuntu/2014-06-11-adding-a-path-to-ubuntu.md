---
id: 43
title: Adding a path to Ubuntu
date: 2014-06-11T08:50:26+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/?p=43
permalink: /2014/06/adding-a-path-to-ubuntu/
geo_public:
  - 0
dsq_thread_id:
  - 4312972527
categories:
  - linux
tags:
  - linux
  - path
---
To run android studio from any folder, I had to add it&#8217;s bin directory to my Path variable.

    echo $PATH
    
    It shows the current situation.
    
    Now I must edit /etc/environment :
    
    

    gedit /etc/environment

    I should find PATH="$HOME/bin:$PATH" and change it to: 

    PATH="$HOME/bin:$PATH:/home/omid/anddev/android-studio/bin"
    
    After a log off / login it must work fine. 
    

     

     

<pre></pre>