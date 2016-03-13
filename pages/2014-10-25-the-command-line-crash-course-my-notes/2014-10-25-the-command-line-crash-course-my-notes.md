---
id: 313
title: The Command Line Crash Course
date: 2014-10-25T02:07:58+00:00
author: Omid Hezaveh
layout: post
guid: http://gik.fi/wp/?p=313
permalink: /2014/10/the-command-line-crash-course-my-notes/
panels_data:
  - 'a:0:{}'
dsq_thread_id:
  - 3655798912
categories:
  - linux
---
<dl class="docutils">
  <dt>
  </dt>
  
  <dt>
  </dt>
  
  <dt>
    A quick review of command line
  </dt>
  
  <dt>
  </dt>
</dl>

<!--more-->

grep Hello *.txt

Looks for the word Hello in all the txt files in the current directory.

cat > omid.txt

Creates omid.txt and enteres whatever I type after that into it.

&nbsp;

<dl class="docutils">
  <dd>
    <pre><span class="gp">$</span> find . -name <span class="s2">"*.txt"</span> -print

</pre>
    
    <pre><span class="gp">$</span> apropos search</pre>
  </dd>
  
  <dd>
  </dd>
  
  <dd>
    print working directory
  </dd>
  
  <dt>
    hostname
  </dt>
  
  <dd>
    my computer&#8217;s network name
  </dd>
  
  <dt>
    mkdir
  </dt>
  
  <dd>
    make directory
  </dd>
  
  <dt>
    cd
  </dt>
  
  <dd>
    change directory
  </dd>
  
  <dt>
    ls
  </dt>
  
  <dd>
    list directory
  </dd>
  
  <dt>
    rmdir
  </dt>
  
  <dd>
    remove directory
  </dd>
  
  <dt>
    pushd
  </dt>
  
  <dd>
    push directory
  </dd>
  
  <dt>
    popd
  </dt>
  
  <dd>
    pop directory
  </dd>
  
  <dt>
    cp
  </dt>
  
  <dd>
    copy a file or directory
  </dd>
  
  <dt>
    mv
  </dt>
  
  <dd>
    move a file or directory
  </dd>
  
  <dt>
    less
  </dt>
  
  <dd>
    page through a file
  </dd>
  
  <dt>
    cat
  </dt>
  
  <dd>
    print the whole file
  </dd>
  
  <dt>
    xargs
  </dt>
  
  <dd>
    execute arguments
  </dd>
  
  <dt>
    find
  </dt>
  
  <dd>
    find files
  </dd>
  
  <dt>
    grep
  </dt>
  
  <dd>
    find things inside files
  </dd>
  
  <dt>
    man
  </dt>
  
  <dd>
    read a manual page
  </dd>
  
  <dt>
    apropos
  </dt>
  
  <dd>
    find what man page is appropriate
  </dd>
  
  <dt>
    env
  </dt>
  
  <dd>
    look at your environment
  </dd>
  
  <dt>
    echo
  </dt>
  
  <dd>
    print some arguments
  </dd>
  
  <dt>
    export
  </dt>
  
  <dd>
    export/set a new environment variable
  </dd>
  
  <dt>
    exit
  </dt>
  
  <dd>
    exit the shell
  </dd>
  
  <dt>
    sudo
  </dt>
  
  <dd>
    DANGER! become super user root DANGER!
  </dd>
  
  <dt>
    chmod
  </dt>
  
  <dd>
    change permission modifiers
  </dd>
  
  <dt>
    chown
  </dt>
  
  <dd>
    change ownership
  </dd>
</dl>

<!--more-->

<!--more-->

<pre><span class="gp">$</span> mkdir <strong>-p</strong> temp/stuff/things/frank/joe/alex/john
No error if existing, make parent directories as needed

- <tt class="docutils literal">ls -lR
  lists all the subdirectories </tt>

The <tt class="docutils literal">pushd</tt> command takes your current directory and "pushes" it into a list for later, then it <em>changes</em> to another directory. It's like saying, "Save where I am, then go here."</pre>