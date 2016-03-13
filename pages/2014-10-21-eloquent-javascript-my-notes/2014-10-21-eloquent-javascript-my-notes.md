---
id: 270
title: Eloquent JavaScript My Notes
date: 2014-10-21T08:02:54+00:00
author: Omid Hezaveh
layout: post
guid: http://gik.fi/wp/?p=270
permalink: /2014/10/eloquent-javascript-my-notes/
panels_data:
  - 'a:0:{}'
dsq_thread_id:
  - 4017983586
categories:
  - Javascript
---
Here are my notes from this wonderful book on Javascript: http://gik.fi/elj

> When you are struggling to follow the book, do not jump to any conclusions about your own capabilities. You are fine—you just need to keep at it. Take a break, re-read some material, and _always_ make sure you read and understand the example programs and exercises. Learning is hard work, but everything you learn is yours, and will make subsequent learning easier.
> 
> &nbsp;

<!--more-->

&nbsp;

>  This old days program:
> 
>     00110001 00000000 00000000
>     00110001 00000001 00000001
>     00110011 00000001 00000010
>     01010001 00001011 00000010
>     00100010 00000010 00001000
>     01000011 00000001 00000000
>     01000001 00000001 00000001
>     00010000 00000010 00000000
>     01100010 00000000 00000000
>     
>     
>     
>     Is the same as this one: 
>     
>     var total = 0, count = 1;
>     while (count <= 10) {
>       total += count;
>       count += 1;
>     }
>     console.log(total);
>     // → 55
>     
>     
>     

There is only one value in JavaScript that is not equal to itself, and that is NaN (which stands for &#8220;not a number&#8221;).

console.log(NaN == NaN)
  
// → false

&nbsp;

&nbsp;

console.log(false ? 1 : 2);
  
// → 2
  
This one is called the conditional operator (or sometimes just ternary operator since it is the only such operator in the language). The value on the left of the question mark “picks” which of the other two values will come out. When it is true, the middle value is chosen, and when it is false, the value on the right comes out.

The difference in meaning between undefined and null is an accident of JavaScript’s design, and it doesn’t matter most of the time. In the cases where you actually have to concern yourself with these values, I recommend treating them as interchangeable (more on that in a moment).

When you want to test whether a value has a real value instead of null or undefined, you can simply compare it to null with the ==

where you do not want any automatic type conversions to happen, there are two extra operators: === and !==. The first tests whether a value is precisely equal to the other, and the second tests whether it is not precisely equal. So &#8220;&#8221; === false is false as expected.

I recommend using the three-character comparison operators defensively to prevent unexpected type conversions from tripping you up. But when you’re certain the types on both sides will be the same, there is no problem with using the shorter operators.

The || operator, for example, will return the value to its left when that can be converted to true and will return the value on its right otherwise.
  
This functionality allows the || operator to be used as a way to fall back on a default value. If you give it an expression that might produce an empty value on the left, the value on the right will be used as a replacement in that case.

The && operator works similarly, but the other way around. When the value to its left is something that converts to false, it returns that value, and otherwise it returns the value on its right.

the expression to their right is evaluated only when necessary. In the case of true || X, no matter what X is—even if it’s an expression that does something terrible—the result will be true, and X is never evaluated. The same goes for false && X, which is false and will ignore X. This is called short-circuit evaluation.

do {
  
var name = prompt(&#8220;Who are you?&#8221;);
  
} while (!name);
  
console.log(name);
  
This program will force you to enter a name. It will ask again and again until it gets something that is not an empty string. Applying the ! operator will convert a value to Boolean type before negating it, and all strings except &#8220;&#8221; convert to true.

The continue keyword is similar to break, in that it influences the progress of a loop. When continue is encountered in a loop body, control jumps out of the body, and continues with the loop’s next iteration.

&nbsp;

## Chapter 1 Exercises

[Ang Demo](http://jsbin.com/sahixo/1/embed){.jsbin-embed}
  


[Ang Demo](http://jsbin.com/xeremu/1/embed){.jsbin-embed}
  


The solution in the book is amazing:

[Ang Demo](http://jsbin.com/hizuqe/1/embed){.jsbin-embed}
  


The way it has used console.log(output || n); and the empty string is neat!