---
id: 130
title: Adding bread crumbs for SEO
date: 2014-07-26T15:13:08+00:00
author: Omid Hezaveh
layout: post
guid: http://geekypartofme.wordpress.com/2014/07/26/adding-bread-crumbs-for-seo/
permalink: /2014/07/adding-bread-crumbs-for-seo/
dsq_thread_id:
  - 4525982533
categories:
  - Wordpress
---
After installing the s[eo plugin,](https://yoast.com/wordpress/plugins/breadcrumbs/) I enabled the bread crumbs.

To show them on pages, I added this code:

<?php if ( function\_exists(&#8216;yoast\_breadcrumb&#8217;) ) {  
yoast_breadcrumb(&#8216;<p id=&#8221;breadcrumbs&#8221;>&#8217;,'</p>&#8217;);  
} ?>

 

to the header file in my template. right after:

<h1 class=&#8221;header-post-title-class&#8221;><?php echo spacious\_header\_title(); ?></h1>