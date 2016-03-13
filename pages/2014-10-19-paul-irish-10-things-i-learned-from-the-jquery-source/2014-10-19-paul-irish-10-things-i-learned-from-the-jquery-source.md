---
id: 240
title: 'Paul Irish : 10 Things I Learned from the jQuery Source'
date: 2014-10-19T05:00:13+00:00
author: Omid Hezaveh
layout: post
guid: http://gik.fi/wp/?p=240
permalink: /2014/10/paul-irish-10-things-i-learned-from-the-jquery-source/
panels_data:
  - 'a:0:{}'
dsq_thread_id:
  - 3656816900
categories:
  - Uncategorized
---
Here come my notes from <a href="http://vimeo.com/12529436" target="_blank">this nice screencast.</a>

<pre class="lang:js decode:true " >(function() {})() simply means the function is going to execute itself right away. I always had trouble understaning the jquery statements. (function (window, undefined ) {})(window); . And the first paranthesis is optional!


(function(window,document,udefined){
        })(this, document);
 
//setInterval is bad, because it doesn't wait for the doStuff function to finnish its business.
        setInterval(function(){
        doStuff();
        },100);</pre>