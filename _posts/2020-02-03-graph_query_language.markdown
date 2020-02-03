---
layout: post
title:      "Graph Query Language"
date:       2020-02-03 14:18:29 -0500
permalink:  graph_query_language
---


![](https://media.giphy.com/media/xT0xezPWsmgkpiGfkY/giphy.gif)

I decided to create a React app with a GraphQL back-end because I have not used GraphQL yet and wanted to learn a bit about it. GraphQL was developed by Facebook and released in 2015. It is an open-source data query and manipulation language for APIs. It allows you to send data over HTTP and you can think of it like a successor to REST. GraphQL is NOT a query language for databases, but for APIs. This is an important distinction. API (application program interface) just allows applications to communicate with one another. An API is not a database. Nor is it a server. It is the code that acts as the access point between the browser/client and the server. Your web application will send a request (via the internet) to the API and the API serves as the access point to get the info you need from the web server, which will have that info stored on a database. Then it will send your response back, often in JSON. A traditional webpage, an Apple mobile app, a Tablet App, and an Android app can all communicate via the API to retrieve the information they need. Because GraphQL is NOT a database, you can use it with any database or none at all. If you create a data graph (with nodes and lines connecting these nodes to represent relationships), you can then use GraphQL or Graph Query Language to query this data in your data graph.

GraphQL uses strong typed schemas. You are basically selecting fields on objects. The objects are formatted in a way that is easy-to-read. Schema Definition Language (SDL) is the syntax for writing schemas. You will run a basic query to retrieve the data from your schema. You can manipulate your data – create, update, and delete. These are called Mutations. GraphQL handles these queries just as they would be handled with REST endpoints and basic CRUD functionality. You can specific exactly what data you want from multiple sources and get back that back from a single endpoint. Thus, making it much more efficient and flexible. 

GraphQL is pretty popular and used by Airbnb, PayPal, and Lyft, to name a few. While I choose to use GraphQL with a React front-end (like Facebook), you do not have to use React as GraphQL will work with a variety of languages and frameworks. 

I added a few different dependencies to my project, one of them being the Apollo package. Apollo allows you to build a communication later that connects your React front-end application to your back-end. The Apollo platform comes with a client component and a CLI interface. Further, it will act as a single source of truth for your schemas. Not only does Apollo have a lot of built-in features, but also it is well maintained and has plenty of additional libraries so there is a lot you can do with it. With Apollo added onto your GraphQL application, your data fetching via the mutations and queries becomes declarative (versus imperative if you are only using GraphQL without the Apollo platform) which is nice for modern data handling. 

![](https://media.giphy.com/media/69mUSKBujnpgmxcqlg/giphy.gif)



