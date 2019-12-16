---
layout: post
title:      "Selecting a Database - MongoDB"
date:       2019-12-16 11:59:35 -0500
permalink:  selecting_a_database_-_mongodb
---


Throughout the Flatiron program I primarily used SQLite as my database, as it is the default database for rails and it is a lightweight server-less database that is great for development and testing. I have yet to use MongoDB, but I am excited to use it as the database for my next project. 

MongoDB is a NoSQL database. It is non-relational database. This is really great for scalability. You can even auto-scale. Instead of tables and rows, what you utilize in SQLite, your data is stored via collections. Not only is this scalable, it is very flexible. Because it is a NoSQL database, MongoDB does not allow you to search the database via SQL statements; they are read only. You do not have to create the table and all of the attributes ahead of time like you do with SQLite. If you need to save a newly created object then all you have to do is serialize that object and then save it into your MongoDB database. Your data is stored as BSON document and each document can have its own unique structure and attributes. BSON is a similar format to JSON; it is called BSON (Binary JSON). MongoDB created BSON in 2009 and it has both integer and string identifiers. All of the documents in your database could be completely unique if you wanted. You can very easily add or delete fields to your document object. You can even use the same key within multiple documents, although each document must have its own unique key.  

MongoDB supports a ton of different languages - like Ruby, JS, Python, Go, R, C++, C#. MongoDB is very fast. One of the reasons it is so fast is that you cannot do complex joins via SQL statements and these operations are very time consuming. Non-relational databases, like MongoDB, have become popular in recent years due to the increasing variety and volume of data we use and store. For example, Google, Cisco, and Facebook use MongoDB. Like SQLite, MongoDB uses indexes to search through documents quickly and return the document with the matching index.

It is a great idea to use a traditional SQL database if your data is structured and unchanging. If you have access to cloud computing and storage and you have a large volume of data with great variety, you will want to use a NoSQL database like MongoDB.


