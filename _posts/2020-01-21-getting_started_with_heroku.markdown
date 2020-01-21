---
layout: post
title:      "Getting Started With Heroku "
date:       2020-01-21 20:13:37 +0000
permalink:  getting_started_with_heroku
---

![](https://media.giphy.com/media/7srpeY4TZMrO8/giphy.gif)

Getting started with Heroku is a fairly straightforward and quick process. Let’s say you are creating a simple Ruby on Rails application that you would like to deploy. As you know, in order to deploy your application, your program will need to run on a server that responds to requests over the internet. Heroku will allow you to deploy, run, and manage your application with just a few simple steps. You can deploy your application right from your command line terminal via Git. Basically, you can think of your Heroku application as a grouping of all of the resources you would have needed (separately) to get your application up and running. It is highly cost-effective, efficicent, and convenient. Heroku will handle a lot for you all behind the scenes!

Heroku is a Platform as a Service (PaaS). While it started out as only supporting Ruby, it now supports several programming languages. The name Heroku is a nod to Ruby and Matz. Amazon’s EC2 cloud-computing platform currently hosts all of the Heroku services (i.e. it is built on AWS’ infrastructure). Heroku is utilized by Salesforce (and it was purchased by Salesforce in 2012). It is fully scalable and allows for a lot of flexibility. 

To get started, first make sure that you have Ruby, Rails, and Git installed on your computer. I would start by first installing [Homebrew](https://docs.brew.sh/Installation) before anything else. This will manage all of your packages for you, which is great. Then go ahead and install [Ruby](https://www.ruby-lang.org/en/documentation/installation/), [Rails](https://guides.rubyonrails.org/v5.0/getting_started.html), & [Git](https://www.atlassian.com/git/tutorials/install-git), as well as a local programming environment like [Atom](https://flight-manual.atom.io/getting-started/sections/installing-atom/).  Then you can create a new directory (and repository on your Github) and CD into that directly via your command line and then get started creating your new rails application! 

After all of that, you are ready to go to: [Heroku](https://signup.heroku.com/) and create an account to get set up using Heroku. I installed Heroku via Homebrew. Then, log into Heroku directly from the terminal with `heroku login –i.` Once you are ready to deploy the application, then type `heroku create` into the terminal, and Heroku will create a unique address for you. This will be displayed immediately and you can copy this info and paste it into your browser. You can push your code to Heroku directly through Git` git push heroku master`. You will just need to run `heroku open’`and navigate to that given address and your application will be there! Sweet as!

Heroku utilizes the container model and calls these containers [Dynos](https://www.heroku.com/dynos). Containers are great because they enable you to deploy your application in these lightweight, isolated containers, “Dynos”, rather than be burdened with managing complicated hardware. Your application is scalable and secure. Only you (or those with permission) can make changes to your application that can then be pushed up via Git to the Heroku deployment. If you do not have the login credentials, your changes will not be authorized, and not be pushed up to the deployed application. In terms of scalability, Heroku offers different Dyno sizes. If you are just learning to program and testing out applications for fun, you can use the free version. The free version will stop the Heroku connection after 30 minutes of inactivity. If your project were to grow and you wanted everyone to be able to access it 24/7, you would need to upgrade to the “Hobby Dyno” which allows you to have the permanent connection.  Pretty Neat! Good luck getting started with Heroku ☺ For more information on getting started with Heroku, head to: [Heroku - How It Works](https://devcenter.heroku.com/articles/how-heroku-works).

![](https://media.giphy.com/media/y3xjJsIg3Mq3K/giphy.gif)




