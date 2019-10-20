---
layout: post
title:      "React Hooks "
date:       2019-10-20 03:00:05 +0000
permalink:  react_hooks
---


React Hooks are a newer feature, introduced in React 16.8. They allow you to use state and “hook into” React lifecycle methods without having to create a class component. I think they are a bit more efficient than classes as you will be able to create a function component much more quickly than a class component. They allow you to create smaller less complex components and they limit the amount of duplicate logic you might have needed in a class component. 

There are a few built-in Hooks, but you can also create your own. Two very useful built-in Hooks are useState and useEffect. Instead of having to write out componentDidMount and componentDidUpdate, you can handle side effects with the useEffect Hook. Both useState and useEffect allow you to access the component’s state and props. With the useState Hook, you will no longer need to create a class and write out a constructor and setState. 

There are a few simple rules to follow when using React Hooks. You cannot call them from a class component or a regular JavaScript function. They must be called from a React function component. The other significant rule is that you must call them on the top level of your components. This is because React will execute Hooks in the order in which they are called. 


![](https://media.giphy.com/media/l3vRfoKIouOdR8uHK/giphy.gif)

