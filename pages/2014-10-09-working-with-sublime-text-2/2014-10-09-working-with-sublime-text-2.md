---
id: 209
title: Working with Sublime Text
date: 2014-10-09T02:01:42+00:00
author: Omid Hezaveh
layout: post
guid: http://gik.fi/wp/?p=209
permalink: /2014/10/working-with-sublime-text-2/
panels_data:
  - 'a:0:{}'
dsq_thread_id:
  - 3817141725
categories:
  - Tips and tricks
tags:
  - editor
  - sublime
---
Getting used to an editor speeds up things greatly, so I&#8217;ve decided to know Sublime Text. Here are my notes.

&nbsp;

shortlink for this page: http://gik.fi/subshort

Adding a shortcut for auto indenting:

<pre class="lang-json prettyprint prettyprinted"><code>&lt;span class="pun">Preferences → &lt;code>Keybindings</code> → <code>User</code>
{&lt;/span> <span class="str">"keys"</span><span class="pun">:</span> <span class="pun">[</span><span class="str">"f12"</span><span class="pun">],</span> <span class="str">"command"</span><span class="pun">:</span> <span class="str">"reindent"</span><span class="pun">}</span>   &lt;/code>

<strong>Text Selections</strong>
<strong>Alt + arrow</strong> : Moves the cursor word by word instead of charachter by charachter. 
Ctrl + D : selects a word 
Ctrl + L : selects a Line
Ctrl Shift A : select a tag
Ctlr Shift M : select brackets 
Ctrl Shift J : select by indentation 
Ctrl Shift Space: Select by Scope (words with the same color)</pre>

Ctrl Home : to go the beginning of the file

Ctrl end: to go to the end

Ctrl Del: to delete the word after the cursor

Ctrl Backspace: del the word befor the cursor

Ctrl L: jump to address bar

<pre class="lang-json prettyprint prettyprinted">Edit Menu
Ctrl Shift T : transposes two letters, or two words
Ctrl Shift Up and down : swap line up and down 
</pre>

<table>
  <tr>
    <td>
      <strong>Ctrl+]</strong>
    </td>
    
    <td>
      indent current line(s)
    </td>
  </tr>
  
  <tr>
    <td>
      <strong>Ctrl+[</strong>
    </td>
    
    <td>
      un-indent current line(s)
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+⇧+↑</strong>
    </td>
    
    <td>
      move line (or selection) up
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+L</strong>
    </td>
    
    <td>
      select line (repeat to select next lines)
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+M</strong>
    </td>
    
    <td>
      jump to closing bracket for current code, repeat to jump to opening bracket
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+⇧+M</strong>
    </td>
    
    <td>
      select all contents of the current brackets (curly brackets, square brackets, parentheses)
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+ /</strong>
    </td>
    
    <td>
      comment/un-comment current line
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+⇧+/</strong>
    </td>
    
    <td>
      block comment current selection
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+⇧+V</strong>
    </td>
    
    <td>
      paste and indent correctly
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+Space</strong>
    </td>
    
    <td>
      select next auto-complete suggestion
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+U</strong>
    </td>
    
    <td>
      soft undo (somehow undoes your movements; it jumps to your last change before undoing it when you repeat this command)
    </td>
  </tr>
</table>

<pre class="lang-json prettyprint prettyprinted"></pre>

<table>
  <tr>
    <td>
      <strong>Ctrl+P</strong>
    </td>
    
    <td>
      quick-open files by name in your project (doesn’t seem to need an actual project set up, it just searches in the directories around the currently-opened file
    </td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <strong>Ctrl+⇧+P</strong>
    </td>
    
    <td>
      command prompt
    </td>
  </tr>
</table>

<pre class="lang-json prettyprint prettyprinted">Ctrl K B Hides the sidebar

Using double column interface:
Shift Alt 2 


Cltrl F2: sets a bookmark
F2 : goes to your bookmark 

<strong>Go To Anything</strong>
Ctrl P : go to any file 
Add a # it and it searches the files with fuzzy matching
Ex: inde#div 

<strong>:50</strong> : goes to line 50 
ex: ind:30 

@ : it finds ids in the file! 


<strong>Ctrl Shift P</strong> : brings the commands 

<strong>Autocompletion:</strong> 
    "auto_complete_commit_on_tab":true,
    "auto_complete": false

I had to change my userkeybindings files like this to enable Ctrl Space keybinding on linux:

[
    { "keys": ["f12"], "command": "reindent"},
    { "keys": ["ctrl+space"], "command": "auto_complete" },
{ "keys": ["ctrl+space"], "command": "replace_completion_with_auto_complete", "context":
[
{ "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
{ "key": "auto_complete_visible", "operator": "equal", "operand": false },
{ "key": "setting.tab_completion", "operator": "equal", "operand": true }
]
}
]

When I auto complete a tag, it's an snippet. So it puts my cursor on the first field. Then if I press
tab I can go to the next field! 

in command pallet, you can write snip and see all the snippets. 

<strong>Package Manager:</strong> 
Go to https://sublime.wbond.net/installation push install, get the code, go to sublime &gt; view &gt; show console
paset the command and push enter. Now we have a package manager! :O 

CTRL P &gt; packaging install &gt; readmeplease
installs a utility to read the readme files of all packages 

Colorpicker
Packaging install &gt; colorpicker 
Also line ending package is a good one. 
To change the theme, download soda and extract it to packages folder, rename it to:
Theme - Soda
Then add this line to user prefs: 
    "theme": "Soda Light.sublime-theme"



colorscheme
https://github.com/MarioRicalde/TextMate-Kuroir-Theme

Color Scheme - Kuroir</pre>