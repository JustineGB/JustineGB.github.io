---
layout: post
title:      "Floof Finder - React Routing"
date:       2019-11-16 11:18:11 -0500
permalink:  floof_finder_-_react_routing
---


I just stated building a React application, Floof Finder, that returns a list of large breed dogs that need to be adopted. I love dogs, and especially love large dogs. We have an Anatolian Shepherd who is the sweetest, fluffiest girl. I volunteer as a Foster parent for Big Dogs Huge Paws (BDHP) - a dog rescue group that specializes in large breed dogs such as Great Pyrenees, Saint Bernard, Great Dane, and Mastiffs. I utilize the PetFinder API to return this list specifying large breed dogs (Size = XL) with a status of adoptable. My plans are to create an application that returns not only this list, but a list of large breed dogs from the Adopt A Pet website as well. Then, you will be able to search for large breed dogs from both website in one spot. Making it faster and easier to help big dogs in need.

I decided to use React to build this application because I want it to be a seamless one-page application that creates an easy-to-use and fast user experience. As I fetch data from the rescue group APIs, I don’t want the user to have to wait while the entire page refreshes. I really enjoy working with React because it is easy to create organized efficient code with the reusable components. I also love using JSX, which is basically a combination of HTML and JavaScript.
To keep my UI in sync with the URL, I am going to use React Router, which will allow for dynamic route matching. What route you take it important, after all. 

![](https://media.giphy.com/media/l2Sq7u1pCBZNyvYGs/giphy.gif)

So, basically my index.js will control the base of what is going to be shown on my page and then the router will come in to determine which component is rendered to the page. This will allow for me to create a scalable application that handles the different URLs as my application grows and I add new features like saving a search list, looking at different rescue organizations, having a user account page with volunteer and rescue information, etc. I want to continue to develop this so volunteers and people can more easily rescue dogs and keep track of this process. It would also be cool to be able to use this data to see what descriptions and photos help dogs get rescued more and try to help market these dogs, especially the ones are have a hard time getting adopted. Maybe put those at the top of the list so when someone is searching for a dog they first see the dogs that need to be rescued the most (like the dogs that have been listed the longest on the website). I want to make sure the navigational flow on my website is intuitive and has a "natural flow" to it and that is why React router is so important. The flow of your website is so important and if it isn’t easy to use and doesn’t have good flow people wont want to use it. React Router is essentially just a state that you are passing an action (just an action of what the page is loaded like /dogs or /dogs/12345 (a dog’s ID). Selecting your URLs well will help you to have a fast website. React Router is a great solution to improving your application’s navigation and its just one of the many awesome libraries you can add to your React application to take it to the next level. 

