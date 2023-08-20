# Reading Class 06
> What is the difference between an Object and a Class in Java?
Object :An object is a software bundle of related state and behavior. Software objects are often used to model the real-world objects that you find in everyday life. This lesson explains how state and behavior are represented within an object, introduces the concept of data encapsulation, and explains the benefits of designing your software in this manner.
Class : A class is a blueprint or prototype from which objects are created. This section defines a class that models the state and behavior of a real-world object. It intentionally focuses on the basics, showing how even a simple class can cleanly model state and behavior.


> Explain to a non-technical friend the concept of inheritance in Java.
Imagine you have a recipe for a basic cake. Now, you want to make different types of cakes with unique flavors and decorations, but the basic cake batter remains the same. In Java, inheritance is like having a main cake recipe and then creating specialized recipes (classes) for different types of cakes (objects) that build upon the main recipe. This way, you don't have to rewrite the whole main recipe each time you make a new cake, but you can modify or add specific ingredients and decorations to create your delicious, customized cakes.


>Static methods are also called what? Why?
Static methods are also called class methods. It is because a static method belongs to the class rather than the object of a class.


> How can you access a variable of a class without instantiating an object from that class?
we can use the static keyword in Java. If we want to access class members without creating an instance of the class, we need to declare the class members static.



>What is a Design Pattern? Describe one or two with analogies from your previous work experience.
Design Pattern: A reusable solution to common software design problems. It's like using proven blueprints for solving challenges in software development.
Singleton Pattern, Observer Pattern
>What is a Singleton?

Singleton :In Java, Singleton is a design pattern that ensures that a class can only have one object.
