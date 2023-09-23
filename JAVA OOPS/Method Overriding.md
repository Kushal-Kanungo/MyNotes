> In other words, If a **subclass(child class)** provides the specific implementation of the method that has been declared by one of its parent class, it is known as **method overriding**.

- Method overriding is used for **runtime polymorphism**

#### Condition for Overriding
1. The method must have the same name as in the parent class
2. The method must have the same parameter as in the parent class.
3. There must be an **IS-A** relationship (inheritance).


#### Covariant Return Type
```java
class Animal {
    Animal reproduce() {
        // Some code to reproduce
        return new Animal();
    }
}

class Dog extends Animal {
    @Override
    Dog reproduce() {
        // Some code specific to dog reproduction
        return new Dog();
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal = new Dog();
        Dog newDog = animal.reproduce(); // Covariant return type
    }
}

```

#### IMPORTANT QUESTIONS

### Can we override static method?

No, a static method cannot be overridden. It can be proved by runtime polymorphism, so we will learn it later.

### Why can we not override static method?

It is because the static method is bound with class whereas instance method is bound with an object. Static belongs to the class area, and an instance belongs to the heap area.

### Can we override java main method?

No, because the main is a static method.