# BetterReads web app
Companion code for the Java Brains code with me series.

# Non-functional Requirement
1. Fast and Performant
2. Handle large amount of data ( i.e. all books ever published in the world)
3. Reliable and Scaleable 
4. Back-end focused
5. Spring Boot & Spring MVC, Spring Security, NoSQL (Apache Cassandra, a distributed DB, multiple nodes and cluster keep sync), Spring Data Cassandra 
6. Searching books (for searching in Cassandra, a separate system needs for that, like, Apache Solr, Apache Lucene installation, some kind of Search Implementation that built on that DB for making search index). 
For seaching that adds a lot more complexity. So, let's depend on Open Library API for that.
7. Pre-Load the Large data set from Open Library Website (Load data on a scheduled manner to keep up-to-date the DB with latest data)
8. Stateless application so that multiple instance can run

# Steps:

* ER Diagram
![ER Diagram](ER-diagram.png)
* Data Modeling (Notes: Cassandra advanced data modeling. RDMS have their data modeling methodology and diagrams. What about Cassandra? Let's discover the key principles of Cassandra data modeling with the Chebotko methodology. Have a look at KDM, a Chebotko modeling tool. And finally, let's talk about the time dimension in Cassandra)
* Query Model
![Query Model](Query-Model.png)


# Prerequisites:
1. JDK and IDE installed on your machine
2. Register for a free hosted Cassandra instance: https://dtsx.io/2WQoLWk. You get a a DataStax Astra DB account with a generous free tier that you can use to follow along the code.
License: APL 2.0

# Technologies:
Application Tier: Spring Boot
Database: Apache Cassandra
Data Layer: Spring Data Cassandra
Security: Spring Security
View Layer: Thymeleaf