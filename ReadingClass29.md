# Reading Class 29 
## What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?
Room is built on top of SQLite, which is a widely used database engine known for its efficiency and simplicity. This combination provides benefits like compile-time query verification, reduced boilerplate code, streamlined database migrations, and seamless integration with other Android components. Overall, using Room with SQLite is a good choice for managing local databases in Android apps due to its reliability and developer-friendly features. However, it's important to assess the specific needs of your application before choosing a database solution.
## Do Rooms have any similarities to JPA?
Room and JPA are similar because they both help with storing data in applications. Here's how they are alike:

Object-Relational Mapping (ORM): They both convert data between Java/Kotlin objects and database tables.

Annotations: They both use special labels in code to show how objects and tables relate.

Entity Classes: Both use classes to represent data objects, which are linked to database tables.

Query Languages: They have their own special languages (JPQL for JPA) to interact with the database.

Relationships: They both support defining connections between data objects.

DAO Pattern: They both recommend a way to keep data access separate from the rest of the code.
## Describe a DAO in your own words
A DAO, or Data Access Object, is a design pattern used in software development to provide a clean and organized way to interact with a database. It acts as an intermediary between the application's code and the database itself.

In simple terms, a DAO encapsulates all the database-related operations (like querying, inserting, updating, and deleting data) into a set of methods. This separation of concerns helps keep the database logic separate from the rest of the application's code, making it easier to maintain, test, and manage.