Ticket: Projection
===========================

**Problem:**

**User Story**

"As a user, I'd like to be able to search movies by country and see a list of movie titles. I should be able to specify a comma-separated list of countries to search multiple countries."

---

**Task**

Implement the **getMoviesByCountry** method in **MovieDao.java** to search movies by country and use projection to return the **title** field.

---

**MFlix Functionality**

Once you complete this ticket, the UI will allow movie searches by one or more countries.

---

**Testing and Running the Application**

Make sure to look at the tests in **ProjectionTest.java** to understand what is expected.

If the application is already running, **stop the application** and run the unit tests for this ticket by executing the following command:

```
mvn test -Dtest=ProjectionTest
```

Or run the tests from your IDE.

Once the unit tests are passing, run the application with:

```
mvn spring-boot:run
```

Or run the **Application.java** from your IDE.

Now proceed to the status page to run the full suite of integration tests and get your validation code.

To have the application use the changes that you implemented for this ticket, make sure to **restart the application** after you completed those changes. Also, only refresh the status page to see the new results of the tests, after the application has been restarted.

<details> 
  <summary>After passing the relevant unit tests, what is the validation code for Projection?</summary>
   Answer: 5a94762f949291c47fa6474d
</details>