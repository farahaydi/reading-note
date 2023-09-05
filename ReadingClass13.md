# Name a few real life examples of “One To Many” relatioships.
- Teacher and Students: A teacher can have many students in a classroom. Each student has one teacher
- Author and Books: An author can write many books, but each book is typically written by one author.
- Parent and Children: In a family, one or both parents can have multiple children. Each child, however, typically has two parents,
- Country and Cities: A country can have multiple cities within its borders, but each city is located in one specific country.

# Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

- Player as "Many," Team as "One": If you design the relationship so that each player can belong to only one team, then "Player" would be on the "many" side, and "Team" would be on the "one" side. In this scenario, each team can have multiple players, but each player is associated with only one team at a time.
- Team as "Many," Player as "One": Conversely, if you design the relationship so that each team can have multiple players, and each player can belong to only one team, then "Team" would be on the "many" side, and "Player" would be on the "one" side. In this case, each team can have multiple players, but each player is associated with only one team.

# Explain one to many relationships to a non-technical friend.
In a one-to-many relationship, imagine you have a room filled with boxes. Each box can hold different items.

The "one" side is like a special table in the room, representing a specific category (e.g., "Toys").
The "many" side includes all the boxes, each filled with items related to that category (e.g., toy cars, stuffed animals).
In this relationship, each category (the "one" side) can have multiple boxes (the "many" side) associated with it, but each box belongs to only one category. It's like organizing items into different boxes by category, where each category can have many boxes, but each box is linked to only one category.

# Describe the difference between a unit test and an integration test.
**Unit Test:**

Scope: Unit tests focus on testing individual components, functions, or methods in isolation, typically within a single module or class.
Isolation: They are isolated from the external dependencies of the code being tested. Mocks and stubs are often used to isolate the unit under test.
Purpose: The primary purpose of unit tests is to validate the correctness of specific code units and ensure that they work as expected.
Speed: Unit tests are usually fast to execute because they don't involve external systems or complex setups.
Dependencies: They don't rely on external databases, services, or network calls and are not affected by changes in these dependencies.
Example: Testing a single function or method within a class.
**Integration Test:**

Scope: Integration tests focus on testing the interactions and collaborations between multiple components, modules, or services in a larger system.
Integration Points: They often involve real external dependencies such as databases, web services, and third-party components.
Purpose: Integration tests ensure that different parts of a system work correctly when integrated together and that they can communicate and interact as expected.
Speed: Integration tests can be slower compared to unit tests due to their involvement with external systems.
Dependencies: They may be affected by changes in external dependencies or the configuration of the integrated components.
Example: Testing the end-to-end flow of a web application, including the database, web server, and user interface.

# What is the object that provides support for Spring MVC Testing?
MockMvc is part of the Spring Test framework and is designed specifically for testing Spring MVC controllers and their behavior without the need to start a real servlet container. It allows you to simulate HTTP requests and receive HTTP responses, enabling you to test your controllers and their interactions in an isolated environment.

Here's how you typically use MockMvc in Spring MVC testing:

You create a MockMvc instance by using MockMvcBuilders.webAppContextSetup() and passing in the WebApplicationContext for your application. This sets up a mock environment for your Spring MVC application.

You use the MockMvc instance to perform HTTP requests (e.g., GET, POST) on your controller methods.

You can then use various assertion methods to verify the responses and behaviors of your controllers.

# What does the “perform()” method do in a Spring integration test?

In a Spring integration test using the MockMvc framework, the perform() method is used to simulate an HTTP request to a specific endpoint or URL. This method sends an HTTP request to the specified endpoint and allows you to perform various actions on that request, such as specifying the HTTP method (e.g., GET, POST), adding request parameters, setting headers, and more. Additionally, it returns a ResultActions object, which enables you to make assertions on the HTTP response received from the simulated request.



