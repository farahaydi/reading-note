# Reading Class 12

# How are query methods defined when using Spring Data JPA?
- Repository Interface
- Query Method Declaration
- Return Type
- Parameters
- Automatic Query Generation

# Which dependencies will you need in order to complete the Spring guide?
- Spring Data JPA
- H2 Database
- Java 17 or Later
- Gradle 7.5+ or Maven 3.5+
- A Text Editor or IDE
- Spring Tool Suite (STS), IntelliJ IDEA, or VSCode

# What annotations are used to specify an auto generated identification number for an Entity?
the annotations used to specify an auto-generated identification number for an entity in Spring Data JPA are as follows:
- @Id: This annotation is used to specify the primary key of an entity class. 
- @GeneratedValue: This annotation is used in conjunction with @Id to specify how the primary key should be generated automatically. 
  It takes a strategy parameter, which can have different values to control the generation strategy.

# Which of the Spring Data Repositories covered in the readings has the most methods available to it?
Among the Spring Data Repositories covered in the provided text, the JpaRepository has the most methods available to it. JpaRepository extends both PagingAndSortingRepository and CrudRepository, which means it inherits all the methods from both of these interfaces.


# Name a downstide of a Spring Data Repository.
one of a Spring Data Repository is that it can lead to tight coupling between your code and the specific abstractions provided by the repository, such as Page or Pageable.
Here's the downside explained:

Tight Coupling: When you extend a Spring Data Repository interface like CrudRepository or JpaRepository, you expose a complete set of persistence methods at once. While this is convenient in many cases, it can lead to tight coupling, where your application code becomes closely tied to the specific repository interface and its methods. 
This tight coupling can make it challenging to switch to a different persistence technology or framework in the future, as your code relies on Spring Data's abstractions.

# How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?
To define an operation to find a student based on their name in a repository named StudentRepository that extends JpaRepository, follow these steps:

Create a method in the StudentRepository interface.

Use the naming convention findBy<PropertyName> where <PropertyName> is the name of the property in the Student entity by which you want to perform the search.
In this case, you want to find students by their name, so use findByName.

Specify the parameter for the search criterion, which should be of the same type as the property you're searching for. In this example, 
you're searching by name, so the parameter is (String name).