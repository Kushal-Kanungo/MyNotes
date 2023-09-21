[[Object]]
Class
[[Constructor]]
[[Static]]
#### Inheritance
> When one object acquires all the properties and behaviors of a parent object, it is known as inheritance. It provides code reusability. It is used to achieve runtime polymorphism.

---
#### Polymorphism
> If one task is performed in different ways, it is known as polymorphism. For example: to convince the customer differently, to draw something, for example, shape, triangle, rectangle, etc.

In Java, we use method **overloading** and method **overriding** to achieve polymorphism.

1. **Method Overloading** => compile-time polymorphism
2. **Method Overriding** => runtime-time overriding  

---
#### Abstraction
> Hiding internal details and showing functionality is known as abstraction. For example phone call, we don't know the internal processing.
> 

---
#### Encapsulation
> Binding (or wrapping) code and data together into a single unit are known as encapsulation. For example, a capsule, it is wrapped with different medicines.

---
#### Coupling
> Coupling refers to the knowledge or information or dependency of another class. It arises when classes are aware of each other. If a class has the details information of another class, there is strong coupling. In Java, we use private, protected, and public modifiers to display the visibility level of a class, method, and field. You can use interfaces for the weaker coupling because there is no concrete implementation.


#### Cohesion

---
#### Association
> Association represents the relationship between the objects. Here, one object can be associated with one object or many objects. There can be four types of association between the objects:

- One to One
- One to Many
- Many to One, and
- Many to Many

---
#### Aggregation
- Aggregation represents a "has-a" relationship between classes, where one class contains a reference to another class, but **the contained class can exist independently**.
- The relationship is typically not exclusive, meaning that the contained class can be shared among multiple instances of the containing class.
- When the containing object is destroyed, the contained object can still exist.
- Aggregation is represented by a weaker association between classes, often implemented as a reference or pointer.

Example: A university can have multiple departments, and a department can exist independently of the university. This is an example of aggregation.
```java
class University {
    private List<Department> departments;
    // Other University methods and attributes
}

class Department {
    // Department methods and attributes
}

```

---
#### Composition
Composition represents a stronger "whole-part" relationship between classes, where one class is composed of one or more objects of another class.
    - The relationship is exclusive, meaning that the composed class cannot exist independently of the containing class. When the containing object is destroyed, the composed objects are also destroyed.
    - Composition is represented by a more tightly coupled relationship between classes and is often implemented by creating objects of the composed class within the constructor of the containing class.
    
Example: A car consists of an engine, wheels, and other components. When the car is destroyed, its components are also destroyed. This is an example of composition.
    
```java
class Car {
    private Engine engine;
    private List<Wheel> wheels;
    
    public Car() {
        this.engine = new Engine();
        this.wheels = new ArrayList<>();
        // Initialize wheels here
    }
    // Car methods and attributes
}

class Engine {
    // Engine methods and attributes
}

class Wheel {
    // Wheel methods and attributes
}

```

> **NOTE:** => In summary, *aggregation represents a looser relationship where objects can exist independently*, while composition represents a stronger relationship where objects are part of a larger whole and *cannot exist without it*. Your choice between aggregation and composition depends on the specific design requirements of your application.  