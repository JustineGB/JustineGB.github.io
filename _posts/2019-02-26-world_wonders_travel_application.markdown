---
layout: post
title:      "World Wonders Travel Application"
date:       2019-02-26 12:03:57 -0500
permalink:  world_wonders_travel_application
---


Flatiron School Rails Final Project 
By Justine Bricknell

For my Rails Final Project I created a travel application that allows a user to track past trips and future travel plans, as well as all of the countries and world wonders that he/she has visited. I decided to create this travel application because I love traveling and I wanted to be able to track all of this information in one spot.  

My application is set up with the following models: User, Trip, Tour, Country, Visit, and World Wonder. 

A user can create, edit, and delete his/her trips, and trips can have many details such as length, packing list, visited yet or not (and year visited, if visited), transportation, hotel info, and attractions. Trips can also have associated countries and world wonders added to them. It is a far-fetched goal of mine to visit all of the Howard Hillman’s Top 100 World Wonders of the World, so I used this list to seed my database: [Hillman's List](https://www.hillmanwonders.com). To seed my database with country information, I used this list that is available publically from data collected by the U.S. government: [Country List](http://www.statvision.com/webinars/countries%20of%20the%20world.xls).   

I set up the following associations: Users have many trips and Trips belong to Users. Trips have many Tours and they have many Countries through Tours. Tours is the join table for Trips and Countries. Countries have many Tours and have many Trips through Tours. Trips have many Visits and have many World Wonders through Visits. Visits is the join table between Trips and World Wonders. World Wonders have many Visits and have many Trips through Visits. Countries have many World Wonders and World Wonders belong to a Country. I found these associations to be quite challenging 
![](https://imgur.com/81ND7qc.jpg)

After establishing my models, associations, and database, I set up my controllers and views.  Because I seeded my database with all of the county and world wonder information, I did not create new/update/edit/delete actions or views for countries or world wonders. I want these lists to be static. Possibly in the future I will add in the ability for an admin to create or change these models. I set up a few AR validations to ensure that proper data is stored in my database. I provide for user authentication with password digest and Omniauth and for user authorization with methods such as current_user. 

Next, I created search features for my world wonder and country index pages to allow a user to filter by certain attributes to quickly find the world wonder or country he/she has in mind. Countries can be filter by region, climate, or searched for by name. World Wonders can be filtered by region, category (natural or man-made), or search for by name.
![](https://imgur.com/yPp0Jyh.jpg) 

