---
layout: post
title:      "Search Your City "
date:       2019-08-20 22:41:20 +0000
permalink:  search_your_city
---


For my final project for Flatiron School, I created a Yelp Clone app called “Search Your City” with a Rails backend and a React/Redux front-end. The app allows a user to login or signup and then search via the Yelp API for places in a selected location. You can enter any search term and the Yelp API will return the top 10 “best matches” (their algorithm determines best matches with a combination of rating, number of reviews, and distance from the given location I believe). You can enter a zip code, a city, or a state/county for a valid location. If you do not enter anything for a location, you will get an error code. I plan on adding in the geolocator to this app in the near future and with that, a user will be able to either opt-in and use their current location or continue to manually input a location. I limited the search results to 10 because I figured that was a good amount of places to look through to determine your selection. From the search results, a user can add a place to their ‘favorite’ list. Or you can add a place to your favorite list entirely from scratch. All of the items on your list can be updated to change their info (like rating or price range) or they can be deleted.  
I used Create-React-App which was super easy to get the app started. And I have both stateless components (functional components) and container components (that deal with state and lifecycle methods like componentDidMount, etc.). Since it requires less code for a stateless component, that is normally preferred, but obviously some components must deal with state for you app to work. I ended up with about 4 container components and 9 stateless components. 
The backend has three controllers – users, sessions, and places. A user can login or signup and the currentUser function ensure the user stays the currentUser within the Redux store. The places model saves info for places such as name, location, review count, price, range, etc. 
This project was challenging and took longer than anticipated to complete, but I am happy to have I worked my way through the many obstcles, and I learned so much along the way. I look forward to continuing to work on this project as I enter my career search. 

