
### SOLID Principle

**S** => Single Responsibility Principle
> The Single Responsibility Principle states that **a class should do one thing and therefore it should have only a single reason to change**.

**O** => Open Closed Principle 
> The Open-Closed Principle requires that **classes should be open for extension and closed to modification.**

**L** => Liskov Substitution Principle
> Is rules says **Class B** and **Class C** are child of **Class A** and If our implementation excepts an **Class A** object then we can replace it with **Class B** or **Class C**. Means child classes can extend the functionality but not narrow it down.
> 

**I** => Interface Segregation Principle
> It says it is better to create multiple interface instead of general purpose interfaces. So that we do not implement unnecessary functions.

**D** => Dependency Inversion Principle
> The Dependency Inversion principle states that our classes should depend upon interfaces or abstract classes instead of concrete classes and functions.


-> On start we will design a **monolith system**. Because when a product is small it is better. But we should write the code in way that we can **decouple** it afterwards, it should not be entangled / tightly coupled.