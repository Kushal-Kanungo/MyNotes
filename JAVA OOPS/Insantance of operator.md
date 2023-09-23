- Used to check the type of an instance of a class
- An object of a subclass is also **instance of** it parent class.

We cannot downcast a class in java without **instanceof**
```java
class Animal { }  
  
class Dog3 extends Animal {  
  static void method(Animal a) {  
    if(a instanceof Dog3){  
       Dog3 d=(Dog3)a;//downcasting  
       System.out.println("ok downcasting performed");  
    }  
  }  
   
  public static void main (String [] args) {  
    Animal a=new Dog3();  
    Dog3.method(a);  
  }  
    
 }  
```
