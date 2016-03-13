---
id: 110
title: WordPress, useless instructions removed
date: 2014-07-10T08:47:29+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/2014/07/10/wordpress-useless-instructions-removed/
permalink: /2014/07/wordpress-useless-instructions-removed/
geo_public:
  - 0
dsq_thread_id:
  - 4003611438
categories:
  - Uncategorized
  - Wordpress
tags:
  - theme
---
I have these instructions under all my comment forms in my wordpress theme:

You can use these HTML tags&#8230;

I looked for a way to remove those and here it is:

Just add this code in functions.php and the instructions go away.

Though it shouldn&#8217;t be the best option because it goes away with every theme upgrade!

&nbsp;

    function mytheme_init() {
    	add_filter('comment_form_defaults','mytheme_comments_form_defaults');
    }
    add_action('after_setup_theme','mytheme_init');
    
    function mytheme_comments_form_defaults($default) {
    	unset($default['comment_notes_after']);
    	return $default;
    }