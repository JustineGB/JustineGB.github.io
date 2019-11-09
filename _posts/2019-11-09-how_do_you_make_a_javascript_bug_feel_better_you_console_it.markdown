---
layout: post
title:      "How do you make a JavaScript bug feel better? You console it!"
date:       2019-11-09 15:52:08 +0000
permalink:  how_do_you_make_a_javascript_bug_feel_better_you_console_it
---


JavaScript (along with HTML and CSS) is a core language to web development. Learning JavaScript, just like learning anything new, requires some patience and practice in the beginning. After you get the basics, it gets easier. JavaScript was developed in 1995 (that is pretty old in the web development timeline) so it is well known and established. That being said, there are many critics of JavaScript because of issues with design, debugging, etc.; however, even if you do not like it, you will still need to understand it. 

JavaScript is an object-based scripting language. You should make good use of objects, classes, and instances to use JavaScript at its full potential. It is case sensitive and each statement should be ended with a semicolon. JavaScript can manipulate the HTML DOM (tree of objects that JavaScript is able to select and change). You can change all of the HTML elements, attributes, and CSS styling on a page. You can add and remove elements and react to events (like a mouse click or a hoover). Native DOM manipulation with JavaScript really helps you understand the front-end of your application (although it is often ignored as developers will use jQuery instead). When you are making calls to the backend, you will need to use promises and aysnc/await for dealing with asynchrony so you do not run into any problems with your callbacks. 

In JavaScript, an important concept to understand is hoisting. A variable can be used before it has been declared. This is because all declarations (versus expressions) are given preference and read at the top of the scope (within the current script or function). “Var” is hoisted, but “let” and “const” are not hoisted. While declared variables are hoisted, initializations are not. You can declare “var X” at the top of your code but if you try to do something with the value of X before you have assigned a value to it, it will be undefined. The value initialization is not hoisted to the beginning, only the declared variable (X). Basically, it is saving some space for “var X” to be assigned to some value but the program does not know that value until it reaches that line of code. Clean efficient programs have variables decaled at the beginning or top of a scope because of hoisting. 

Debugging in JavaScript was difficult for me at first. Coming from Ruby, I was used to using binding.pry and inspecting the code at the exact point I needed to see. In JavaScript you can debug with console.log, debugger, and catch (error) to see what went wrong. I recommend using console.log to get started debugging and it can be used across a wide variety of issues. The debugger keyword works like binding.pry and will inspect the code at a certain breakpoint. In the Chrome Dev Tools you can look at Sources and then Scope to see what values are currently assigned to your variables. 

![](https://media.giphy.com/media/zOvBKUUEERdNm/giphy.gif)

