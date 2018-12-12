---
layout: post
title:      "Wine Tracker Application - Sinatra Final Project "
date:       2018-12-12 19:45:13 +0000
permalink:  wine_tracker_application_-_sinatra_final_project
---



For my final project within the Sinatra section for Flatiron School, I decided to create a Wine Tracker Application. After traveling to France in September, I became interested in good wine, and I found myself forgetting which bottles/styles I had tried and which I liked or disliked. So, I thought this application would be perfect for tracking all of that data so that I would know what to purchase next and to start getting a better understanding of my palate. 

Getting started on this project, I watched a few videos about setting up a Sinatra application (via the Learn.co video hub), researched the main concepts within the Sinatra section (via the checklist provided by DJ), reviewed my past labs, and attended a few of Howard’s study groups, which were very helpful! I used the Corneal Gem to set up my directory structure quickly and easily. 

After setting up my directory, I set up my models (Wines & Users) and associations (wines belong to users and users have many wines). The User is the parent in the relationship (and the wine is the child and children can inherit from their parents). Wines have a foreign key to relate the to the User (User_id column). I used Active Records validations to provide validations for emails and usernames (presence of and uniquenss) to make sure I didn’t have multiple users with the same name and/or email using the program because that would get confusing. I also used validations for a number of other fields to ensure that all of the data that persisted to my database is clean.

Next, I set up my databases with the Rake Gem and used the Bycrypt Gem to create a secure password. I seeded my database with data to make sure my application was working the way I wanted it to during my testing phase. Next, I set up my controllers (be sure to add all of your controllers to your config.ru or else your program won’t work!). While getting my controller routes working, I set up the views pages (erb). Using the Shotgun Gem, I was able to see exactly what I was creating as I was creating it. In addition to Shotgun, I used the Pry Gem to help work through bugs and get everything working ☺ 

To elaborate on the application itself: the application opens on a welcome page, directing the user to either sign up or log in. If the user is revisiting the page after she has already logged in (and not logging out) then when she selects the log in button, the application will immediately bring her to her user home page. This page will show her user details (email, name, etc.) and her wine reviews. The user is able to log out, visit the homepage (welcome page), visit a list of all other users, or visit a list of all of the wines added by any user. On the user list index, you can click on a user to see all of the wines and more details on that specific user and her wine reviews. And on the wine index page, you can click on a wine to see all of the details about that wine, including a link to the user who added the wine. When you view a wine details page, you can also see an edit or delete button if you are the user who added that wine and only if you are logged in. If you view another users wine detail page, you will not be able to see an edit or delete button (i.e. we would not want one user being able to edit or delete another users’ wine review). 

Overall, I thought this project was really fun. I feel much more confident in my coding abilities and I know how to deal with the roadblocks that come up with coding. I had a lot of “a-ha moments” and really took a lot away from this section. 


