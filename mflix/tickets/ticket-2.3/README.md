Ticket: User Management
=======================

**Problem:**

**User Story**

"As a user, I should be able to register for an account, log in, and logout."

---

**Task**

For this Ticket, you'll be required to implement all the methods in _UserDao.java_ that are marked for the **User Management** ticket. Specifically, you'll implement:

- **createUserSession**
- **getUser**
- **getUserSession**
- **deleteUserSession**
- **deleteUser**

Registering should create an account and log the user in, ensuring an entry is made in the **sessions** collection. There is a unique index on the **user_id** field in **sessions**, so we can efficiently query on this field.

---

**MFlix Functionality**

Once this ticket is completed, users will be able to register for a new account, log in, logout, and delete their account.

---

**Testing and Running the Application**

If the application is already running, **stop the application** and run the unit tests for this ticket by executing the following command:

```
mvn test -Dtest=UserTest
```

Once the unit tests are passing, run the application with:

```
mvn spring-boot:run
```

Or run the _Application.java_ from your IDE.

Now proceed to the status page to run the full suite of integration tests and get your validation code.

To have the application use the changes that you implemented for this ticket, make sure to **restart the application** after you completed those changes. Also, only refresh the status page to see the new results of the tests, after the application has been restarted.

<details> 
  <summary>After passing the relevant tests, what is the validation code for User Management?</summary>
   Answer: 5a8d8ee2f9588ca2701894be
</details>