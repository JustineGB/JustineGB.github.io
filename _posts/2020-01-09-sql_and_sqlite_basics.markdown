---
layout: post
title:      "SQL & SQLite Basics "
date:       2020-01-09 17:10:24 +0000
permalink:  sql_and_sqlite_basics
---

![](https://media.giphy.com/media/l4FGw4d101Sa0pGTe/giphy.gif)

SQL stands for Structured Query Language. There are many databases that use SQL, such as MySQL, SQL Server, Postgre SQL, and SQLite. Flatiron teaches SQLite as it is pretty simple to get set up and running quickly. It is self-contained, server-less, and requires zero-configuration. Further, the SQLite library is very small and it is a cross platform file. While you cannot write an entire web application with SQL, it is extremely important as it allows you to communicate with the database that will store all of the vital information pertinent to your website. Think about Facebook, LinkedIn, Amazon and vast amount of information they store in a database. Different databases will allow you to utilize different data types. Data categories in SQLite are text, integer (whole number), real (decimals), and blob (binary large object that can store any kind of data). 

SQLite is a relational database (versus a non-relational database such as Mongo DB). With a relational database your data is store in tables with rows (horizontal) and columns (rows). You will create your schema ahead of time and then can get started making your tables. Your schema encompasses your table names, row and column names, relationships between tables, etc.  Each row will have a primary key – a unique identifier for that row of data. If you have created relationships between tables, you will add in a foreign key to associate table A with table B. 

Getting set up with a SQLite database is simple and easy. First, you will want to download SQLite via your terminal. Then you can get started creating databases and adding tables to those databases. You can create, alter, and drop tables once they are created. You can make changes as you are developing your program so that you can interact easily with your data; you can create, select, update, and delete data. When you are storing a record, you do not need to assign it an index or primary key, as this will automatically be created. 

I used SQLite with my Ruby on Rails application and it made it super simple to retrieve and filter data as needed from the backend. Before I added a JavaScript front-end to my program, I was only using SQLite to search and filter through countries and cities on my travel application and I found that it worked very well; it was easy to write and it performed quickly. I came across one issue while using SQLite and that was storing images. Some people do not think you should store images in databases, but you can do it. For SQLite, you will need to store the image with the BLOB data type. You will need to return the img data as a string	`blob = SQLite3::Blob.new img `. And then you can create your new instance of this image as a blob data type and store it in your database `db.execute “INSERT INTO TableName VALUES (1, ?)”, blob`

SQL allows for complex joins and grouping/sorting data easily. When you are constructing a complex join, it is always easiest to think about a Venn Diagram. There is a full join which is the entirely of both circles, including the overlap. An Inner Join is just the overlap. A left join is the overlap plus the left circle. A right join is the overlap plus the right circle. I am a visual learner so I always write this out by hand before I construct my joins to make sure I am thinking about the joins correctly. For grouping and sorting you can use order by, group by, limit, having, and where, and you can also organize by ascending or descending. 

SQL and SQLite are pretty neat. SQLite is easy to use and set-up and SQL is a great tool to have in your back pocket if you have a general idea of how your want your data set up into tables and their relationships. If you have no idea what you want to do with your data and what relationships you will have or your think they will change frequently, I would not use SQL/SQLite (use a No-SQL db like Mongo).  



