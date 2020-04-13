---
layout: post
title:      "Redux Review"
date:       2020-04-13 17:38:30 +0000
permalink:  redux_review
---


![](https://media.giphy.com/media/A06UFEx8jxEwU/giphy.gif)

While I have been working with React a lot, I have not spent much time using Redux lately, so I decided to do a quick review. Redux is a predictable state container for your JavaScript application. It Is predictable, centralized, debuggable, flexible, and open source. It is very lightweight. Redux allows your application to detect state changes and enforce this throughout the application via a pure function referred to as a reducer. The state is stored within a central store and all of the components can access this state as needed (or not needed, to prevent unnecessary changes). 

If you are programming a large, complex application, Redux can often come in handy to enforce state across your application with the reducers. For example, if you have many components and you are passing data between many different components, you will want to make sure the correct component is storing its correct state and passing information correctly as needed. This can get very complicated as your application grows and you are passing tons of information between many different components. This is where a central state comes in and becomes very, very handy. 

![](https://media.giphy.com/media/nGMnDqebzDcfm/giphy.gif)

Sometimes Redux is not always the best option or maybe you just want to try something else out. There are a number of alternatives to Redux’s state management. One of the simplest alternatives is just using React’s own this.setState(). This is a great option if you have a small, simple application and there is little information being transferred between components. You don’t always need to add Redux onto your React application, and often times, React is enough to handle your application and information transfer between components without introducing Redux. 

There are a few negatives or issues with using Redux. One of the major issues, in my opinion, is that you need to write a large amount of code even when you make a small change. Overall, I think Redux is a great option for state management in a large application, but if you are not building anything complex, just keep it simple and stick with React!

![](https://media.giphy.com/media/10bdAP4IOmoN7G/giphy.gif)

