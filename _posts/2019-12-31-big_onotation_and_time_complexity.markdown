---
layout: post
title:      "Big ONotation & Time Complexity"
date:       2019-12-31 17:01:02 +0000
permalink:  big_onotation_and_time_complexity
---

![](https://media.giphy.com/media/9G3xf3God7KFzYtLTx/giphy.gif)

Big O Notation and Time Complexity are concepts you must grasp in order to be an effective web developer. Time Complexity describes the amount of time taken to run a function. Basically, how time scales with a function - the amount of time it will take to do something like transfer data with respect to the input variables. As the input size grows, how does the function scale? 

Typically, big o notation is used to express time complexity (so coefficients and lower order terms are excluded). It is called big O because the letter o refers to the Order of the function. Big o is used in many fields, not just computer science, to provide an estimate on the potential time or space complexity of an algorithm. The time complexity or cost of a function can be calculated, broadly speaking, by the amount of lines of code needed to complete the function. 

Generally, the worst-case scenario is considered although sometimes the average case is used. For big o notation you will need to add up the steps of your algorithm, drop constants, understand that different inputs means different variables so you are looking at O(a*b) not O(n^2) as your inputs are not necessarily the same, and last, you will need to drop all non-dominant terms. 

Be sure to consider your algorithmic efficiency when you are writing a function or else you could end up with a very, very slow program as it scales. There are a ton of resources out there on big o and time complexity and lots of helpful videos if you would rather listen/watch a tutorial. I found this to be a helpful resource for seeing all of the time complexity of common algorithms: [Big O Cheat Sheet](https://www.bigocheatsheet.com).  

![](https://media.giphy.com/media/QBd2kLB5qDmysEXre9/giphy.gif)
