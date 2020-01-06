---
layout: post
title:      "Asynchronous JavaScript"
date:       2020-01-06 13:53:37 +0000
permalink:  asynchronous_javascript
---

![](https://media.giphy.com/media/JSnKGLvrFvYU8/giphy.gif)

Understanding asynchronous programming is an important concept in JavaScript programming. Synchronous programming completes one task at a time. This is done sequentially; task A is started and completed before tasks B is then started and completed and so on. Asynchronous programming allows your browser to get started on one task and then move onto another task before that first task is completed. Basically, it allows your browser to start a bunch of tasks and continue to work on them until they are all complete. The browser is able to kind of multi-task and be more efficient, just like a chef getting started on multiple dishes all at once rather than working on only one dish at a time from its first step until completion.   

Some programming languages are multi-threaded, while JavaScript is single-threaded. Each thread can only do one task at a time. Most computers have multiple cores so that you are able to run multiple threads simultaneously on separate cores (if supported by the programming language you are using). But since JavaScript is single thread, you will only be able to do one task at a time on the main thread. JavaScript is run from top-to-bottom and left-to-right. Each line of code is executed sequentially. Working with this one main thread, you would not want to try to retrieve a large amount of information from a server synchronously as this would cause your program to appear to freeze if this took a long time or failed to retrieve the data. You do not want to make a synchronous call to a server to retrieve a ton of info and then lock out everything else that is going on, on your page. The browser can appear to be frozen as your processor is working on that intensive bit of code. This is called blocking. Your browser is blocked from doing anything else until that bit of code is completed. However, JavaScript has web workers, which allow you to run one task on the main thread, and then another task can be shipped off to a worker thread (like retrieving a ton of data). One downside with web workers is that they cannot access the DOM. Also, web workers are still running synchronously, so you will run into problems with them if you need your program to be asynchronous. 

Three important concepts of asynchronous programming are promises, callbacks, and Aysnc/Await. A promise represents the eventual completion (success or failure) of an asynchronous function. The promise is a proxy or sort of placeholder for a value you are trying to retrieve. A promise can be pending, fulfilled, or rejected. A callback is a function that is executed after another function is complete. They allow you to make sure certain code is executed after other code has completed. Aysnc/Await is a great way to work with promises. Aysnc ensures that your function returns a promise and Await tells JavaScript to wait until the promise is resolved. You cannot use Await in a non-Aysnc function. If you are using Aysnc/Await you rarely need to use Promise then/catch because Await handles the waiting for us. Await will return the result if the promise correctly resolves, or else it will throw an error.
With the popularity of single page applications and users expecting websites to respond immediately to their requests (even if that means the retrieval of very large amounts of data), asynchronous programming is extremely important. That being said, it is not always the best to use. If your program is very simple or you are running simple/short operations, you may not even need asynchronous code in your program and including could actually cost you more overhead. Just like anything you are including in your code, you want to make sure you do your research first and really think about what is needed or not. Considering the event loop, web APIs, and call stack all come into play.

![](https://media.giphy.com/media/UtzFhfHOSGAEkh7pAr/giphy.gif)






