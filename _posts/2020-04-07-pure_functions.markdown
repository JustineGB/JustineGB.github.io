---
layout: post
title:      "Pure Functions"
date:       2020-04-07 14:27:24 +0000
permalink:  pure_functions
---

![](https://media.giphy.com/media/xT9IgzoKnwFNmISR8I/giphy.gif)

I have been reviewing old labs and taking a deeper look at certain topics, and just recently took a quick deep dive into Pure Functions. While I was not asked about Pure Functions in any of my job interviews, I wanted to be prepared in case it came up as I have heard from others that it is a common interview topic. Why are Pure Functions so important? Why are they so much better than impure functions? What sort of issues can you avoid by using Pure Functions?

Pure Functions are great because they are very predictable. They will always return same result given the same input. And highly predictable code is obviously much easier to manage then unpredictable code. You need to use Pure Functions in a variety of circumstances, especially with concurrency and within your React applications. 

Pure Functions product no side effects. Blocking any sort of chain reaction makes your code much cleaner, easier to read, and easier to debug. They are simple and reusable. By side effect, when the Pure Function returns a value, it does not modify any data outside of its own function scope – there is no side effect or alteration to any other data or functions.

![](https://media.giphy.com/media/l2JejHjYm3wb2GSC4/giphy.gif)

Pure Functions are fully independent from the outside state of your program, which makes them so great for concurrency and React. You do not have to worry about numerous side effects that could come up with a shared dynamic state. This makes your React application much easier to debug and change around as you can easily refactor and reorganizing your code with your independent Pure Functions. 

Overall, Pure Functions are simple, easy-to-use, and reusable functions that help you write clean and concise programs. If you defer to using Pure Functions, you will have a program that is easier to debug and one that does not produce unwanted side effects. 


![](https://media.giphy.com/media/KEYbcgR8oKQzwpwvLU/giphy.gif)


