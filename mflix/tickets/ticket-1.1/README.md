Ticket: Database Connection
===========================

**Problem:**

**Task**

MFlix will use MongoDB as a storage layer, so for this ticket you'll be required to perform some application setup.

1. First, make sure you've created a user on your Atlas cluster with read and write access to any database.

   - The user name should be **m220student** and the password should be **m220password**
   - Don't forget to whitelist your IP address!

2. Copy the connection string by clicking on **Connect** in the Atlas cluster. Select that you'd like to connect with **MongoDB Compass**, and select Compass 1.12 or later - this will give you the **srv** connection string. Make sure this URI string contains your username and password!

3. Locate the file called **src/main/resources/application.properties** within the **mflix** java project, and replace the information within with your own **mongodb uri srv** connection string, set in property value **spring.mongodb.uri**:

```
spring.mongodb.uri=mongodb+srv://YOUR_CLUSTER_URI
```

* It's highly recommended you also change the **jwtSecret** to some very long, very random string. While this application is only meant for local use during this course, software has a strange habit of living a long time:

```
jwtSecret=SUPER_SECRET_KEY_YOU_WANT_TO_REPLACE_THIS
```
---

**Testing and Running the Application**

In order to reinforce good development practices, everything asked of you in this course is backed up by unit tests. Reading through the tests for a specific exercise will tell you exactly what is expected.

If the application is already running, **stop the application** and run the unit tests for this ticket by executing the following command:

```
mvn test -Dtest=ConnectionTest
```

from the **mflix-java/mflix** directory, or running the Connection test from your IDE in the **src/test/java/mflix/api/daos** directory.

Once the unit tests are passing, run the application with:

```
mvn spring-boot:run
```

Or run it from your IDE.

Now proceed to the status page to run the full suite of integration tests and get your validation code.

To have the application use the changes that you implemented for this ticket, make sure to **restart the application** after you completed those changes. Also, only refresh the status page to see the new results of the tests, after the application has been restarted.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Connection?</summary>
   Answer: 5a9026003a466d5ac6497a9d
</details>

