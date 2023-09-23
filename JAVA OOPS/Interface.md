An **interface in Java** is a blueprint of a class. It has static constants and abstract methods.

- It **cannot be instantiated** just like abstract class.
- Interface can **extend** another interface
- Class can **implement** an interface.
- **Multiple Inheritance** is supported using interfaces in JAVA. 

Interface is made up of 
1. Abstract Methods (method without body)
2. Static Constants

#### Why use Java interface?

There are mainly three reasons to use interface. They are given below.

- It is used to achieve **abstraction**.
- By interface, we can support the functionality of **multiple inheritance**.
- It can be used to achieve **loose coupling**.

All the data member in Interfaces are converted to **static** & **final**. So we can call them **STATIC CONSTANTS**


#### FROM JAVA 8
- default methods can have have body also.
- static methods with methods body can be defined in interfaces.