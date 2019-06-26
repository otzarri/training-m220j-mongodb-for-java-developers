# M220J: MongoDB for Java Developers

This repository is where I store source code and documentation used during the course [M220J - MongoDB for Java Developers](https://university.mongodb.com/courses/M220J/about).

This and all the README files under `tickets` directory are copied from [Carlan's repo](https://github.com/carlan/m220j/) who did a good work migrating them.

You can check the work made for each ticket in the corresponding tag, each ticket contains a user story to complete. There is only one commit per step containing all the changes and it's linked to a tag.

Modifications done in source code have a comment with the ticket id above, for example:

```properties
# BEGIN Ticket 1.1: Database Connection
spring.mongodb.uri=mongodb+srv://<username>:<password>@<hostname>/test
# END Ticket 1.1: Database Connection
```

or

```java
    // BEGIN Ticket 1.2: Projection > Implement the query and projection required by the unit test
    queryFilter = Filters.all("countries", country);
    List<Document> movies = new ArrayList<>();
    moviesCollection
        .find(queryFilter)
        .projection(fields(include("title")))
        .into(movies);
    // END Ticket 1.2: Projection
```

User stories within tickets provide a lot of information about which work was done and where.

| Title                             | User Story location                      |
| --------------------------------- | ---------------------------------------- |
| Ticket 1.1: Database Connection   | [tickets/ticket-1.1](tickets/ticket-1.1) |
| Ticket 1.2: Projection            | [tickets/ticket-1.1](tickets/ticket-1.2) |


## What You'll Learn

This course will teach you how to use MongoDB as the database for a Java application.

You'll play the role of a back-end developer for a Java application, and your job is to implement the application's communication with MongoDB. This includes:

- Reading and writing data
- Using the Aggregation Framework
- Managing the configuration of the database client through the Java driver
- Creating a robust application by handling exceptions and timeouts

**Prerequisites:**
We highly recommend taking M001 prior to taking this course. A basic understanding of **MongoDB's document model** as well as familiarity with **Java development environments** will help you get the most out of this course.

## What You'll Build

You'll build the back-end for a movie-browsing application called MFlix.

Using the MongoDB Java Driver, you will implement MFlix's basic functionality. This includes basic and complex movie searches, registering new users, and posting comments on the site.

You will also add more features to the MFlix application. This includes writing analytical reports, increasing the durability of MFlix's connection with MongoDB, and implementing security best practices.