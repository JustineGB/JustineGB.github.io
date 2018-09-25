---
layout: post
title:      "Best Hikes in Colorado - Ruby CLI Gem."
date:       2018-09-25 18:55:44 +0000
permalink:  best_hikes_in_colorado_-_ruby_cli_gem
---


! [] (https://imgur.com/a/3p4eUo7)

###Introduction:
For the final portfolio project in the Ruby section of Flatiron School students are asked to make their own Ruby CLI gem. I live in Colorado and I love hiking, so I thought, >why not >making a hiking gem for the best hikes here in Colorado? 
While challenging, creating this gem was extremely rewarding, and I learned so much through the entire process. As a hiker, I like to select my hikes depending on difficulty, length, and often, region. I do not want to waste my weekend driving if I can find a great hike in my backyard. So, I set my program up to first present the user with a list of regions. From a selected region, he/she is then presented with a list of hikes. And from that list of hikes, he/she can select one to find out more info. The program loops to allow the user to see the info on as many or as few regions and hike as he/she wishes, 

###Web Scraping:   
Web scraping is simply extracting data from a website to save and/or use within your program. I used OpenUri and Nokogiri get the information I needed from website. OpenUri is easy-to-use and can be thought of a wrapper; it allows you to grab data from a webpage (http/https/url) as though it were a file, allowing you to access and then manipulate the data in your program. Nokogiri allows you to parse html and xml (i.e. extract out the particular text you want to use). I found web scraping to be time-consuming in the beginning, but it gets easier with practice; it is a lot of trial and error. I tried a few different hiking websites before settling on thecohiker.com to scrape the data on hikes and their regions that I needed for my program. Based on the website you select, scraping can be much harder or much easier. After inspecting the page, I parsed it via the element that contains the regional hike categories as this was the first bit of information that is displayed to the user. I tried to be as specific; when parsing, you want to be as particular as possible so that your application will run faster (it will have less data to process).

###Ruby Basics:
Ruby is an object-oriented language. Basically everything is either an object or a method. For example: “2.even?” 2 is an object in Ruby that can be operated on via methods and here we are calling the “even?” method on the object “2”. Some refer to classes as ‘containers for methods’. Some also refer to classes as ‘object-creating factories’ because they create objects; they instantiate objects. 
There are instance methods and class methods. Instance methods operate on an individual instance of that class. For example, in a Dog class, you might have a particular instance of dog with the attribute of name set to “Etta,” the age set to “4” and the breed set to “Anatolian Shepard.” That instance of the Dog class would be just one object, just one instance, of that particular class. You can have many instances of a class and while they are all of the Dog Class, they all have their own unique attributes (or you could set them to have some/all shared attributes). A class method, on the other hand, can operate on the entire class. You do not need to instantiate an instance to call a class method. 
Understanding Accessibility & Scope: you can define local variables like “hike” that are only accessible within a particular method, or instance variables like “@hike” that are accessible within any instance method, or you can assign class variables that are accessible anywhere in that class “@@hike.” 
Self is a very important topic to understand while using Ruby. Self is the current object that Ruby is operating on. Within an instance variable, self will be that particular instance, and within a class variable, self can be the entire class. 
Last, understanding how objects collaborate is key to developing a good Ruby program. Because I decided to organize my gem via regions and then hikes per region, I set up a has many/belongs to relationship. Hikes belong to Regions, that is, a list of particular hikes belong to a particular region. One hike will not belong to multiple regions. Regions ‘have many’ hikes. Understanding this relationship helped me to get started on how I wanted to set up my program and classes. 
 
###My Classes/File Organization:
After determining the object relationships, I decided to separate my classes out via: 
*a Scraper class
*a Cli class
*a Regions class
*a Hikes class 
I separated out the functionality into these 4 classes because they all are responsible for different parts of the program. It doesn’t make sense to put the creation of regions in the CLI section; you want this logic to be contained within the Region class. I started by coding the Scraper class, then moved on to the Regions class, and coded the Cli and Hike classes last (with a lot of back and forth). It was difficult determining the instantiation of the hike objects as I did not want to program to instantiate all of the in the beginning of the program. Since they are not created at the beginning, there is some lag time when the user makes a selection. Because the hikes belong to the regions, I decided to instantiate them from a method within the regions class and then the array is cleared each time so that only that regions specific hikes are listed out to a user.


